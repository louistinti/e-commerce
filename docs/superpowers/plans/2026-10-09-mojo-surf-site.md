# Mojo Surf site, plan d'implémentation

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Livrer `mojo-surf/index.html`, un one-page statique pour une école de surf itinérante, avec une carte SVG illustrée où un camion rouge glisse de spot en spot au rythme d'un carrousel.

**Architecture:** Un seul fichier HTML qui contient le CSS (variables de thème, clair/sombre, mobile) et le JS (données des spots, carrousel, camion, prix saisonnier, formulaire). Les données modifiables (spots, prix, dates de saison) sont regroupées en tête de script. Pas de dépendance, pas de build.

**Tech Stack:** HTML, CSS, JavaScript vanilla, Google Fonts, images Unsplash temporaires. Test manuel dans le navigateur via `npx http-server mojo-surf -p 5179`.

Spec : `docs/superpowers/specs/2026-10-09-mojo-surf-site-design.md`.

---

## Fichiers

- Create: `mojo-surf/index.html` : la page complète.
- Create: `mojo-surf/README.md` : comment lancer, quoi remplacer avant mise en ligne (photos, croquis de carte, contacts à vérifier, Formspree).
- Create: `.claude/launch.json` : config du serveur de preview (`npx http-server mojo-surf -p 5179`) pour vérifier dans le navigateur intégré.

Le fichier HTML est organisé en blocs commentés, dans cet ordre : variables et base, nav, hero, concept, spots (carte + carrousel), cours, tarifs, questions, réserver, footer, mobile, puis le script.

---

### Task 1 : Squelette, thème, nav, hero

**Files:** Create `mojo-surf/index.html`, `mojo-surf/README.md`, `.claude/launch.json`

- [ ] Écrire le `<head>` : `lang="fr"`, viewport, titre « Mojo Surf », meta description, police Google Fonts (une typo ronde pour les titres, par exemple « Fredoka » ou « Nunito », et une lisible pour le texte).
- [ ] Variables CSS sur `:root` : `--bg` sable, `--fg` brun foncé, `--accent` terracotta, `--ocean` bleu, `--van` rouge, `--line`, `--bg-2`. Redéfinir sous `@media (prefers-color-scheme: dark)` avec `:root:not([data-theme="light"])` et sous `:root[data-theme="dark"]`. `body` avec background explicite.
- [ ] Nav collante : nom « Mojo Surf », liens Spots, Cours, Tarifs, Questions, bouton Réserver. Liens masqués sous 720 px.
- [ ] Hero : h1 « Du surf toute l'année, là où sont les vagues », paragraphe de présentation, boutons Réserver et Voir les spots, trois repères (Toute l'année / 4 spots / Tous niveaux), grande photo Unsplash.
- [ ] README avec la commande de lancement et la liste des choses à remplacer.
- [ ] `.claude/launch.json` : `{"version":"0.0.1","configurations":[{"name":"mojo-surf","runtimeExecutable":"npx","runtimeArgs":["http-server","mojo-surf","-p","5179","-c-1"],"port":5179}]}`
- [ ] Vérifier dans le navigateur : la page s'affiche, pas d'erreur console. Commit `Add Mojo Surf skeleton with hero and nav`.

### Task 2 : Concept, cours, tarifs saisonniers, questions, footer

**Files:** Modify `mojo-surf/index.html`

- [ ] Section Concept : trois blocs (On se déplace selon les conditions / On surfe toute l'année / Débutants et intermédiaires bienvenus), chacun avec un titre court et 2 phrases.
- [ ] Section Cours : trois cartes. Cours collectif ; Perfectionnement, 4 personnes max ; Cours privé + vidéo-analyse. Chaque carte : titre, pour qui, durée indicative, prix. Le prix du collectif porte la classe `js-price-collectif`, la mention de saison la classe `js-price-season`.
- [ ] Section Tarifs : tableau avec les trois formules, puis bloc Options matériel (combi 5 €, gants 1 €, chaussons 1 €). Le prix du collectif utilise aussi `js-price-collectif`.
- [ ] Prix saisonnier en JS :

```js
const PRICING = {
  collectif: { offSeason: 20, season: 25 },
  season: { fromMonth: 4, fromDay: 1, toMonth: 9, toDay: 30 } // avril à fin septembre inclus
};
function isHighSeason(d = new Date()) {
  const m = d.getMonth() + 1, day = d.getDate();
  const s = PRICING.season;
  const afterStart = m > s.fromMonth || (m === s.fromMonth && day >= s.fromDay);
  const beforeEnd = m < s.toMonth || (m === s.toMonth && day <= s.toDay);
  return afterStart && beforeEnd;
}
function applySeasonPrice(d) {
  const high = isHighSeason(d);
  document.querySelectorAll('.js-price-collectif').forEach(el => { el.textContent = high ? PRICING.collectif.season : PRICING.collectif.offSeason; });
  document.querySelectorAll('.js-price-season').forEach(el => { el.textContent = high ? "tarif saison, d'avril à fin septembre" : "tarif hors saison, d'octobre à mars"; });
}
applySeasonPrice();
window.mojoApplySeasonPrice = applySeasonPrice; // pour tester depuis la console
```

- [ ] Section Questions : `<details>` pour niveau requis, âge minimum, quoi apporter, lieu du rendez-vous (annoncé la veille), mauvaises conditions (report), paiement.
- [ ] Footer : téléphone `+33 6 14 26 36 42`, email `mojosurf360@gmail.com`, lien Facebook, les 4 communes.
- [ ] Vérifier dans la console : `mojoApplySeasonPrice(new Date(2026,6,1))` affiche 25, `mojoApplySeasonPrice(new Date(2026,10,1))` affiche 20, date du jour (9 octobre) affiche 20. Commit `Add concept, courses, seasonal pricing, FAQ and footer`.

### Task 3 : Carte SVG, camion rouge et carrousel des spots

**Files:** Modify `mojo-surf/index.html`

- [ ] Données des spots en tête de script. Les coordonnées `x`, `y` sont dans le repère du SVG (viewBox `0 0 400 600`) :

```js
const SPOTS = [
  { id: 'saint-gilles', name: 'Saint-Gilles-Croix-de-Vie', place: 'Grande Plage', x: 150, y: 110,
    text: 'Plage de sable large et accessible, vagues douces à marée montante. Le spot idéal pour un premier cours.',
    photos: ['https://images.unsplash.com/...', '...'] },
  { id: 'sauzaie', name: 'La Sauzaie', place: 'Bretignolles-sur-Mer', x: 175, y: 230, text: '...', photos: [] },
  { id: 'dunes', name: 'Les Dunes', place: 'Bretignolles-sur-Mer', x: 190, y: 320, text: '...', photos: [] },
  { id: 'sables', name: "Les Sables-d'Olonne", place: 'Grande Plage', x: 240, y: 500, text: '...', photos: [] }
];
```

- [ ] SVG en ligne : fond mer (`--ocean` très clair), trait de côte en `<path>` doux orienté nord-sud, terre côté droit, une route pointillée reliant les 4 spots dans l'ordre. Les points et étiquettes sont générés en JS à partir de `SPOTS` (un `<g>` par spot avec `<circle>` et `<text>`, rendu comme bouton : `role="button"`, `tabindex="0"`, `aria-pressed`).
- [ ] Camion : `<g id="van">` avec un pictogramme de van (corps rectangle arrondi, fenêtres, deux roues), couleur `var(--van)`. Positionné par `style.transform = translate(x, y)` ; transition CSS `transform .7s cubic-bezier(.16,1,.3,1)`, désactivée sous `prefers-reduced-motion: reduce`.
- [ ] Carrousel : conteneur `.spot-track` avec un panneau par spot généré depuis `SPOTS` (nom, lieu, description, 2-3 photos). Un seul panneau visible à la fois (`transform: translateX(-index*100%)`). Flèches précédent/suivant, compteur « 1 / 4 », `aria-live="polite"` sur le panneau actif.
- [ ] Fonction unique `setSpot(index)` : met à jour le panneau actif, `aria-pressed` des points, position du camion, compteur. Appelée par les flèches, les points de la carte, les touches flèche gauche/droite sur le carrousel, et un balayage tactile (touchstart/touchend, seuil 40 px).
- [ ] Disposition : grille 5/7 (carte à gauche, carrousel à droite) au-dessus de 900 px ; empilé en dessous, carte limitée à 320 px de haut.
- [ ] Vérifier dans le navigateur : les 4 spots se succèdent avec les flèches, le camion glisse, le clic sur un point de la carte change le panneau, balayage mobile en 375 px, clavier fonctionne. Commit `Add spot map with moving van and carousel`.

### Task 4 : Formulaire Réserver et version mobile

**Files:** Modify `mojo-surf/index.html`, `mojo-surf/README.md`

- [ ] Formulaire : formule (3 choix radio), nombre de personnes (number 1-8), niveau (select : Jamais surfé / Déjà pratiqué / Autonome), date souhaitée (date), nom, email, téléphone, message. `novalidate`, validation JS : formule, nom et au moins un moyen de contact ; messages d'erreur sous les champs ; message de confirmation fictif à la soumission, sans envoi.
- [ ] Mobile : menu plein écran (bouton hamburger, liens en grand, fermeture au clic), barre « Réserver » fixe en bas qui se masque quand la section Réserver est visible (IntersectionObserver), gouttière 16 px, aucune largeur fixe dépassant l'écran.
- [ ] README : ajouter le paragraphe « Brancher Formspree » (mettre `action="https://formspree.io/f/XXXX" method="POST"` et retirer le `preventDefault`).
- [ ] Vérifier à 375, 768 et 1280 px, clair et sombre, pas d'erreur console, pas de défilement horizontal. Commit `Add booking form and mobile layout`.

### Task 5 : Finition et vérification complète

- [ ] Passer la checklist de vérification du spec (navigation, carrousel, camion, questions, formulaire, prix selon date, 3 largeurs, 2 thèmes, console vide).
- [ ] Captures d'écran desktop et mobile pour le compte rendu.
- [ ] Commit final si des retouches ont été faites.
