# Mojo Surf, site one-page

Date : 2026-10-09

## Contexte

Mojo Surf est une école de surf itinérante en Vendée, tenue par un moniteur indépendant. Il surfe toute l'année et choisit chaque jour le spot selon les conditions, entre Saint-Gilles-Croix-de-Vie, Bretignolles-sur-Mer (La Sauzaie), les Dunes (Bretignolles) et Les Sables-d'Olonne. Public : tous niveaux, surtout débutants et intermédiaires.

Le site doit mettre en avant deux choses : il surfe toute l'année, et il se déplace pour trouver les meilleures vagues. Le gros plus attendu est une carte illustrée avec un camion qui se déplace de spot en spot au rythme d'un carrousel.

## Périmètre

- Un dossier `mojo-surf/` dans ce repo, un seul fichier `index.html` (HTML, CSS, JS, sans dépendance), plus un `README.md` sur le modèle de `larralde-surf/`.
- Police via Google Fonts, mode clair et sombre selon le système, version mobile dédiée.
- Textes en français uniquement.
- Photos : images Unsplash temporaires, à remplacer. Pas de logo : le nom « Mojo Surf » est composé en typo.
- Le formulaire n'envoie rien tant qu'il n'est pas branché sur Formspree (ou équivalent). Le README le rappelle.

Hors périmètre : réservation en ligne avec paiement, multilingue, blog, location de matériel seule.

## Direction visuelle

Chaleureux, esprit van et road trip côtier. Palette sable, terracotta, bleu océan ; typo ronde et amicale pour les titres ; coins arrondis modérés ; illustrations SVG simples (trait de côte, camion). Le ton rassure un débutant : simple, concret, sans jargon.

## Structure de la page

1. **Navigation** : nom, liens d'ancre (Spots, Cours, Tarifs, Questions), bouton Réserver. Sur mobile : menu plein écran et barre « Réserver » fixe en bas, comme sur Larralde.
2. **Ouverture** : accroche du type « Du surf toute l'année, là où sont les vagues », une phrase de présentation, bouton Réserver et lien vers les spots, trois repères (toute l'année, 4 spots, tous niveaux), une grande photo.
3. **Le concept** : trois arguments courts. On se déplace selon les conditions ; on surfe toute l'année, combi fournie ; adapté aux débutants et intermédiaires.
4. **Les spots** : carte illustrée + carrousel (détaillé ci-dessous).
5. **Les cours** : quatre formules. Cours collectif ; perfectionnement en petit groupe de 4 maximum ; cours privé avec vidéo-analyse ; stand-up paddle sur le lac du Jaunay, sur demande.
6. **Tarifs** : grille ci-dessous, plus un bloc options matériel.
7. **Questions** : liste dépliable. Niveau requis, âge minimum, quoi apporter, comment on connaît le lieu du rendez-vous (annoncé la veille selon les conditions), que se passe-t-il si les conditions sont mauvaises (report), comment payer.
8. **Réserver** : formulaire. Champs : formule (choix), nombre de personnes, niveau (débutant / déjà pratiqué / autonome), date souhaitée, nom, email, téléphone, message. Validation côté client, message de confirmation fictif.
9. **Pied de page** : téléphone et email relevés sur la page Facebook (`+33 6 14 26 36 42`, `mojosurf360@gmail.com`), à faire vérifier par le moniteur avant mise en ligne ; lien vers la page Facebook ; mention des 4 communes.

## Grille tarifaire

| Formule | Prix |
|---|---|
| Cours collectif, hors saison (octobre à mars) | 20 € par personne, planche incluse |
| Cours collectif, saison (avril à fin septembre) | 25 € par personne, planche incluse |
| Perfectionnement, groupe de 4 maximum | 60 € par personne |
| Cours privé avec vidéo-analyse | 80 € |
| Stand-up paddle, lac du Jaunay | sur demande |

Options matériel, en plus de chaque formule : combinaison 5 €, gants 1 €, chaussons 1 €.

## La carte des spots

Composant central de la page, sans dépendance externe.

- **Dessin** : un SVG en ligne représentant un trait de côte stylisé, orienté nord-sud, avec les 4 spots du nord au sud : Saint-Gilles-Croix-de-Vie, La Sauzaie (Bretignolles), Les Dunes (Bretignolles), Les Sables-d'Olonne. Chaque spot est un point cliquable avec son nom. Le dessin est volontairement simple : il sera remplacé par le croquis que le propriétaire du site fournira plus tard, donc les coordonnées des spots sont centralisées dans un petit tableau JS, pas dispersées dans le SVG.
- **Camion** : un pictogramme SVG de van. Il est positionné sur le spot actif et glisse d'un spot à l'autre (transition CSS sur `transform`, environ 700 ms, désactivée avec `prefers-reduced-motion`).
- **Carrousel** : un panneau par spot avec le nom, une description de 2-3 phrases (type de vague, pour qui, ambiance) et 2-3 photos placeholder. Navigation par flèches, par clic sur un point de la carte, et par balayage sur mobile. Les panneaux et les points de la carte partagent le même index actif.
- **Disposition** : sur desktop, carte à gauche et carrousel à droite ; sur mobile, carte en haut (réduite en hauteur) et carrousel en dessous.
- **Accessibilité** : les points de la carte sont des boutons avec `aria-pressed`, le panneau actif est annoncé via `aria-live="polite"`, les flèches sont au clavier.

## Comportement et robustesse

- Aucune requête réseau hors Google Fonts et images Unsplash. Si une image ne charge pas, le cadre garde une couleur de fond.
- Le formulaire valide les champs requis (formule, nom, email ou téléphone) et affiche un message de confirmation sans rien envoyer. Le `README.md` explique comment brancher Formspree.
- Mode sombre : variables CSS redéfinies sous `prefers-color-scheme: dark`.
- Largeur mobile : gouttière 16 px minimum, pas de défilement horizontal.

## Vérification

- Ouvrir la page en local (`npx http-server mojo-surf -p 5179`) et vérifier : navigation par ancres, carrousel (flèches, clic sur la carte, balayage mobile), déplacement du camion, dépliage des questions, validation du formulaire.
- Vérifier aux largeurs 375 px, 768 px et 1280 px, en clair et en sombre.
- Vérifier qu'il n'y a aucune erreur console.
