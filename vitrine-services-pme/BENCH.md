# Benchmark : site vitrine Brillance Pro (nettoyage B2B, Bordeaux, entreprise fictive)

Ce bench suit le brief client bloc par bloc : chaque référence retenue sert une exigence précise de [BRIEF-CLIENT.md](BRIEF-CLIENT.md), les autres sont rangées à côté avec leur raison.

## Limites, à lire en premier

- **Sites ouverts et capturés le 2026-11-12**, dans un navigateur Chrome piloté (viewport 1440×900, au-dessus de la ligne de flottaison, et 390×844 pour le mobile). Les couleurs et les polices citées ont été relevées dans la page (styles calculés), pas devinées. Les contrastes sont recalculés selon la formule WCAG 2.1.
- **14 références sur 16 vues et capturées**, plus 9 références de galerie. Les 2 pages Stratus (n° 9 et 10) sont **inaccessibles (protection anti-robots)** : un challenge Cloudflare « Verify you are human » s'affiche, et il n'a pas été contourné. Elles sont à côté, **non vérifiées**.
- **La première version se trompait sur plusieurs points**, corrigés ici. Lebontri est une plateforme d'annonces (intervenants vérifiés, acompte de 10 %), pas une entreprise de nettoyage. Aucun « {city} » n'est visible sur ses pages. Son « simulateur » n'a ni champ ni prix : l'estimation est floutée et demande un compte. L'« estimation instantanée » de Coverall exige les coordonnées avant le prix. Les titles « devis sous 24h » et la mention « free, no-obligation » d'Office Pride n'existent plus.
- **Refonte du 2026-11-12** :
  - Tri des 25 références : **11 inspirations** (et 1 capture mobile) dans [`captures/inspis/`](captures/inspis/), **14 références à côté** (et 2 captures mobiles) dans [`captures/a-cote/`](captures/a-cote/). Les numéros et les noms de fichiers n'ont pas changé.
  - Le bench est réorganisé par bloc de l'arborescence du brief (section 6), avec un tableau de couverture.
  - **Une seule direction** est gardée, car le brief prévoit « 1 piste et 2 allers-retours » (section 10). Les directions B et C sont retirées, la raison est dans « Directions ».
  - **Tokens corrigés** : le vert accent `#22C55E` ne sert plus pour les icônes porteuses de sens (2,3:1 sur blanc, sous le seuil de 3:1 du critère WCAG 1.4.11), seulement pour le décor. L'icône de la carte de prestation est précisée en `brand.blue`. L'exemple chiffré du bloc avis (« 4,8 sur 5, 37 avis ») est remplacé par un format, pour ne pas afficher d'avis qui n'existent pas.
  - **Aucune nouvelle référence retenue.** 5 recherches Dribbble pour la zone d'intervention et « Comment ça marche » n'ont rien donné de conforme au brief (détail en fin de bench).
- **Passe du 2026-11-13** : Brillance Pro est fictive et personne ne valide rien, donc les anciennes questions ouvertes deviennent des [arbitrages](#arbitrages). Les chiffres propres à l'entreprise (délai de devis, cibles de KPI, préavis, nombre d'avis) sont retirés. **Photos d'équipe** : Unsplash a renvoyé « Access Denied » et Pexels une vérification anti-robots Cloudflare, non contournée. Le site a donc un bloc « Qui sommes-nous » court, sans photo, et les exigences de photo d'équipe réelle sont retirées du bench.
- Aucun formulaire n'a été rempli ni envoyé. Les captures ne montrent pas de données personnelles (les signatures d'auteurs et les avatars ont été masqués avant la capture).

---

## Couverture du brief

| Exigence du brief | Inspirations | Manque |
|---|---|---|
| 1. Hero (H1 avec la ville et l'estimation en ligne, CTA « Obtenir mon estimation », téléphone, illustration au trait) | 1, 5, 17, 19 | Aucun H1 vu qui annonce une estimation en ligne. Pas de photo d'équipe : l'illustration au trait est à produire. |
| 2. Prestations (4 cartes : pour qui, fréquence) | 16, 18 | Aucune grille de 4 cartes avec « pour qui » et fréquence. Détail repris du n° 7 (à côté). |
| 3. Pourquoi nous (3 arguments, « Comment ça marche » en 3 étapes, « Qui sommes-nous » sans photo) | 4, 5 | « Comment ça marche » : aucune référence conforme (les shots vus sont B2C et hors marque). « Qui sommes-nous » : texte du brief, sans modèle. Détail repris du n° 20 (à côté). |
| 4. Zone d'intervention (carte légère statique ou SVG, communes en texte) | aucune | Onet (n° 3) charge une carte OpenStreetMap interactive d'office, et le seul shot Dribbble « Service Area Map » embarque une carte Google. Aucune liste de communes en texte vue. Le bloc est à dessiner sans modèle. |
| 5. Avant / après (curseur sur 3 à 4 paires d'illustration, clavier) | 22, 25 | Aucun site réel de nettoyage avec un curseur. |
| 6. Avis Google (note, nombre, 3 verbatims, lien vers la fiche ; gabarit dans la démo) | 18, 19 | Aucun site réel avec des verbatims datés et un lien vers la fiche. |
| 7. Devis en ligne en 3 étapes (type, surface et fréquence puis repère de prix, coordonnées) | 5, 21 | Aucun site réel n'affiche un prix avant les coordonnées (n° 6 et 7 le cachent). Détails repris des n° 6, 8, 11 et 14 (à côté). |
| 8. Contact (téléphone, e-mail, horaires, adresse, hors horaires) | 3 | La mention d'intervention hors horaires : aucune référence. |
| Pages SEO (bureaux, fin de chantier, vitres) | 16 | Aucune page vitres vue. Format de title repris du n° 2 (à côté). |
| Mobile : barre « Appeler » / « Devis » de 44 px minimum (critère WCAG 2.5.5), estimation sans aide | capture mobile Office Pride | Aucune barre fixe à 2 boutons vue. |
| Marque : blanc, bleu franc, accent vert, Figtree ou Nunito Sans | 17 | Aucune référence en Figtree ou Nunito Sans. |
| Accessibilité WCAG 2.1 AA (vert jamais en texte sur blanc, labels visibles, clavier) | 25 | Contre-exemples de contraste nombreux (n° 3, 7, 11), aucune référence de formulaire à labels visibles vérifiée. |
| Preuve « Local » (adresse, carte des communes, liste des communes en texte) | 1, 3, 19 | Liste des communes en texte : aucune. |
| Preuve « Estimation immédiate » (repère de prix avant les coordonnées) | aucune | Aucune référence ne montre un prix sans coordonnées ni compte. Companeo (n° 11) promet la vitesse de la demande, Lebontri (n° 2) a retiré « devis sous 24h ». |
| Preuve « Équipe salariée et assurée » (« Qui sommes-nous », attestation sur demande) | 5 | Aucun site ne nomme ses agents ni leur statut salarié. |
| Preuve « Sans engagement » (préavis écrit, remplacement, interlocuteur unique) | aucune | Aucun encart vu. Lebontri (n° 6) écrit « sans engagement » à côté de « compte requis ». |
| Preuve « Produits respectueux » et label | 4 | La démo n'affiche aucun logo de label (voir Arbitrages). |
| Preuve « Clients satisfaits » (note et 3 à 6 avis datés) | 18, 19 | Voir bloc 6. |

---

## Inspirations, bloc par bloc

### 1. Hero

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 1 | [Lebontri : Nettoyage de bureau à Bordeaux](https://lebontri.fr/nettoyage-bureau/bordeaux) (plateforme FR) | [capture](captures/inspis/01-lebontri-bordeaux.jpg) | Au-dessus du H1 « Nettoyage de bureaux à Bordeaux – Service sur mesure pour entreprises », une pastille « Bordeaux et alentours · intervenants vérifiés ». Sous le CTA (vert clair `#D1ED92`, texte `#12372A`, 10,1:1), la micro-ligne « Gratuit · 3 minutes · une photo suffit ». À éviter : le gabarit dupliqué d'une ville à l'autre (voir n° 2 et 6, à côté). | Sous-titre « Bordeaux Métropole et Gironde » en pastille, preuve « Local » ; micro-ligne pour « Estimation immédiate ». |
| 5 | [Office Pride : Colorado Springs Downtown](https://officepride.com/colorado-springs-downtown/) (site réel US) | [capture](captures/inspis/05-office-pride-colorado-springs.jpg) | La ville sous le H1 et un repère de lieu au-dessus. Le téléphone en bouton blanc à côté du CTA. Sous le formulaire, 3 réassurances (« Highly reviewed · Locally owned · Professional crews »). Sa photo d'équipe n'est pas reprise (pas de photo d'équipe, voir Arbitrages). À éviter : « Request a Quote » blanc sur `#00964D` (3,8:1). | Téléphone visible en CTA secondaire « Appeler le 05… ». |
| 17 | [PartnerPlus, Commercial Cleaning Service Website](https://dribbble.com/shots/27382820-PartnerPlus-Commercial-Cleaning-Service-Website) (Dribbble, Wavespace) | [capture](captures/inspis/17-dribbble-partnerplus.jpg) | Fond blanc, un bleu franc pour le seul CTA « Check Our Prices », le téléphone juste dessous en texte, une pastille « The standard for commercial » au-dessus du H1. L'illustration de bâtiments montre qu'un hero tient sans photo d'équipe. | Marque « blanc, bleu franc », un seul CTA primaire, téléphone sous le CTA, illustration au trait à la place d'une photo. |
| 19 | [Cleaning Lead Generation Landing Page](https://dribbble.com/shots/27223369-Cleaning-Lead-Generation-Landing-Page) (Dribbble, WPLanding) | [capture](captures/inspis/19-dribbble-cleanpolish.jpg) | La ville en couleur dans le H1 (« Cleaning for busy people in New York »), puis « 4.9/5 » avec étoiles sous les boutons. Pour Brillance Pro, « Bordeaux » en bleu, pas en orange ; la ligne de note n'est pas reprise dans la démo (aucun avis, voir Arbitrages). À éviter : les logos factices (« Logoipsum »). | SEO local « la ville dans le H1 ». |

### 2. Prestations

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 16 | [Lebontri : fin de chantier à Bordeaux](https://lebontri.fr/nettoyage-fin-chantier/bordeaux) (plateforme FR) | [capture](captures/inspis/16-lebontri-fin-chantier-bordeaux.jpg) | Un sous-titre propre au métier : « Poussières de plâtre, voiles de ciment, traces de peinture ». Une coche « Revêtements fragiles et date de livraison ». | Carte « Fin de chantier » qui parle à Nadia (salissures, date fixe), lien vers la page SEO dédiée. |
| 18 | [Polar, Commercial Cleaning Website Design](https://dribbble.com/shots/27768209-Polar-Commercial-Cleaning-Website-Design) (Dribbble, Systra Studios) | [capture](captures/inspis/18-dribbble-polar.jpg) | Sur fond blanc, un carrousel de prestations avec de vraies photos de lieux (cage d'escalier, bureaux), une prestation par carte. À éviter : le hero sombre, hors de la marque « blanc ». | Cartes illustrées par de vrais lieux, pas par des clichés. |

Détail repris d'une référence à côté : sous l'estimateur Coverall (n° 7), le périmètre en 5 tâches (sols, déchets, aspirateur, poussière, surfaces). Une liste aussi courte peut détailler « quelle prestation » dans chaque carte.

### 3. Pourquoi nous

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 4 | [Onet : agence du Mans](https://www.onet.fr/en/agencies/onet-proprete-et-services-le-mans/) (site réel FR, version anglaise) | [capture](captures/inspis/04-onet-le-mans.jpg) | Le label Qualipropre est dans une section « Certifications » avec son logo et une phrase d'explication, pas collé au CTA. | « Label Qualipropre si obtenu », « Produits écolabellisés si justifiés ». |
| 5 | [Office Pride : Colorado Springs Downtown](https://officepride.com/colorado-springs-downtown/) (site réel US) | [capture](captures/inspis/05-office-pride-colorado-springs.jpg) | Une ligne de 3 réassurances courtes avec une icône chacune. | Les 3 arguments (salariée et assurée, écolabellisés, sans engagement) en version courte. |

Détail repris d'une référence à côté : l'argument « Want the same team? » de Flatiron Maids (n° 20). Il rejoint l'option B du brief (« La même équipe, chaque semaine ») et le frein de Sophie (un agent différent chaque mois).

« Comment ça marche » en 3 étapes : aucune inspiration. À dessiner avec les 3 preuves du brief : préavis écrit dans le contrat, remplacement en cas d'absence, interlocuteur unique.

« Qui sommes-nous » : pas de photo d'équipe (Unsplash et Pexels bloqués le 2026-11-13, voir Limites). Le texte de 3 phrases du brief (section 6, bloc 3), le logo à gauche, sur fond `brand.blue-50`.

### 4. Zone d'intervention

Aucune inspiration. Onet (n° 3) affiche une carte OpenStreetMap interactive chargée d'office, et le shot « Service Area Map & Wide Coverage » (Dribbble, ouvert pendant la refonte) embarque une carte Google : les deux vont contre « sans Google Maps chargé d'office » et « image statique ou SVG ». À faire : un SVG léger de Bordeaux Métropole et de la Gironde, et la liste des communes en texte (utile au SEO local et à Thomas, à Pessac).

### 5. Avant / après

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 22 | [Before/After slider](https://dribbble.com/shots/27731233-Before-After-slider) (Dribbble, Diana Fabiańczuk) | [capture](captures/inspis/22-dribbble-before-after-slider.jpg) | Une ligne de séparation fine, une poignée ronde avec 2 flèches (elle dit qu'on peut glisser), 2 étiquettes en pilule « Before us » et « After us » dans les coins hauts. | Curseur de comparaison, étiquettes « Avant » et « Après » toujours visibles. |
| 25 | [img-comparison-slider](https://img-comparison-slider.sneas.io/) (composant open source) | [capture](captures/inspis/25-img-comparison-slider.jpg) | Testé dans la page : après un clic, les flèches du clavier déplacent la séparation (de 4 % à 95 % en maintenant la flèche droite). Composant web, compatible avec un site statique. L'élément n'expose pas de rôle ARIA. | « Accessible au clavier », générateur statique. Ajouter un `aria-label` (« Comparer avant et après, [type de local] ») et une légende visible. |

Aucun site réel de nettoyage avec un curseur n'a été trouvé (recherches web en anglais et en français, et une page Jan-Pro qui renvoie une erreur 403). Recommandations : 3 ou 4 cas au plus, chacun légendé « photo d'illustration » et le type de local, sans lieu ni date (voir Arbitrages).

### 6. Avis Google

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 18 | [Polar, Commercial Cleaning Website Design](https://dribbble.com/shots/27768209-Polar-Commercial-Cleaning-Website-Design) (Dribbble, Systra Studios) | [capture](captures/inspis/18-dribbble-polar.jpg) | « 5,0 basierend auf 36 Google-Bewertungen » en tête, puis des cartes d'avis avec étoiles, prénom et ancienneté de l'avis. La note revient aussi sous le CTA du hero. | La note, le nombre d'avis, 3 verbatims ; la date demandée par le Code de la consommation. Dans la démo, en gabarit marqué « Exemple de mise en page ». |
| 19 | [Cleaning Lead Generation Landing Page](https://dribbble.com/shots/27223369-Cleaning-Lead-Generation-Landing-Page) (Dribbble, WPLanding) | [capture](captures/inspis/19-dribbble-cleanpolish.jpg) | Une ligne compacte note et étoiles sous les boutons, qui renvoie vers le bloc avis. | Rappel de la note Google en haut de page, pour un déploiement avec de vrais avis ; absent de la démo. |

Détail repris d'une référence à côté : Coverall Fresno (n° 12) met la note et le nombre d'avis dans un titre. Son verbatim anonyme et non daté est à éviter.

### 7. Devis en ligne en 3 étapes

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 5 | [Office Pride : Colorado Springs Downtown](https://officepride.com/colorado-springs-downtown/) (site réel US) | [capture](captures/inspis/05-office-pride-colorado-springs.jpg) | Une carte « Step 1 of 3 » avec barre de progression et un bouton « Next » bleu nuit `#12345A`, visible dès le hero. À éviter : les coordonnées (nom, e-mail, société, téléphone) dès l'étape 1. | Formulaire en 3 étapes, barre de progression « Étape 2 sur 3 ». |
| 21 | [Multistep request quote form](https://dribbble.com/shots/24125199-Multistep-request-quote-form) (Dribbble, Amine) | [capture](captures/inspis/21-dribbble-multistep-quote-form.jpg) | Une barre d'étapes nommées (type, préférences, recommandation, coordonnées), des cartes à grande icône pour le type, et la recommandation affichée **avant** les coordonnées. | Ordre du brief : (a) type de local, (b) surface et fréquence puis repère de prix, (c) coordonnées. |

Détails repris de références à côté :
- les 4 facteurs de prix en cartes à icône (surface, fréquence, prestations, horaires) de Lebontri (n° 6), pour expliquer le repère de prix de l'étape (b) ;
- le type de local en cartes à icône à l'étape 1 de Companeo (n° 11) ;
- le paragraphe « How we determine your quote » de Coverall (n° 8), qui justifie la visite : il colle à la mention « indicatifs, confirmés après visite » ;
- le ton « questions à poser à votre prestataire » de l'article prix de Coverall (n° 14), en 3 ou 4 lignes sous l'estimateur.

### 8. Contact

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 3 | [Onet : agence de Lyon](https://www.onet.fr/en/agencies/onet-proprete-et-services-lyon/) (site réel FR, version anglaise) | [capture](captures/inspis/03-onet-lyon.jpg) | Plus bas dans la page : horaires (lundi au vendredi, 8 h-12 h et 14 h-17 h), adresse, téléphone, pastille « Open ». Les données `LocalBusiness` sont présentes. La carte OSM interactive n'est pas reprise (voir bloc 4). | Téléphone, horaires, adresse ; données structurées `LocalBusiness`. |

Détail repris d'une référence à côté : sur mobile, Coverall (n° 7) met le numéro en lien `tel:` dans le bandeau du haut.

### Pages SEO

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 16 | [Lebontri : fin de chantier à Bordeaux](https://lebontri.fr/nettoyage-fin-chantier/bordeaux) (plateforme FR) | [capture](captures/inspis/16-lebontri-fin-chantier-bordeaux.jpg) | Les salissures du métier et la date de livraison dans les premières lignes : c'est la partie qui n'est pas dupliquée d'une page à l'autre. | Page « Nettoyage fin de chantier en Gironde », contenu rédigé et non dupliqué. |

Détail repris d'une référence à côté : le title de Lebontri Tours (n° 2), « Nettoyage de bureaux Tours (37) : devis de pros \| LeBonTri ». Pour Brillance Pro : « Nettoyage de bureaux Bordeaux (33) : estimation en ligne \| Brillance Pro ».

---

## Mobile

| Site | Capture | Ce qu'on observe | Exigence du brief |
|---|---|---|---|
| Office Pride (inspiration) | [capture](captures/inspis/mobile-office-pride.jpg) | Dans le hero, 2 boutons de même largeur : « Request a Quote » vert et le téléphone en blanc. Le formulaire « Step 1 of 3 » suit. La barre fixe « Ready to get started? Request a Quote » reste visible même quand le formulaire est à l'écran, et le bouton d'accessibilité la chevauche. | « Appeler » et « Devis » au même niveau ; montre pourquoi masquer la barre quand le formulaire est visible. |
| Lebontri, Bordeaux (à côté) | [capture](captures/a-cote/mobile-lebontri-bordeaux.jpg) | Une barre fixe en bas, un seul bouton pleine largeur « Estimer mon nettoyage · Gratuit ». Pas de bouton d'appel. Au premier écran, le même CTA apparaît 2 fois. | Contre-exemple de la barre « Appeler » / « Devis ». |
| Coverall, janitorial (à côté) | [capture](captures/a-cote/mobile-coverall-janitorial.jpg) | Pas de barre fixe. Le numéro est en lien `tel:` dans le bandeau du haut. Le H1 en capitales prend 3 lignes et la photo occupe presque tout l'écran. | Contre-exemple pour le LCP mobile sous 2,5 s (seuil « bon » des Core Web Vitals) et une estimation rapide. |

**À retenir** : aucun des 3 ne met « Appeler » et « Devis » côte à côte dans une barre fixe. Pour servir les indicateurs du brief (complétion du devis sur mobile, estimation sans aide, boutons d'au moins 44 px) :
- une barre fixe en bas, en 2 boutons égaux de 56 px (« Appeler » en blanc bordé de bleu, « Devis » en bleu plein), masquée quand le formulaire est visible ;
- un formulaire en 3 écrans, avec une barre de progression, des boutons-cartes pour le type de local et des pastilles pour la fréquence ;
- l'estimation avant les coordonnées ;
- une illustration de hero légère (SVG au trait), pas une photo plein écran comme Coverall.

---

## Directions

Le brief prévoit **1 piste** de maquette (section 10). Une seule direction est donc gardée.

**Direction unique : « Net et lumineux »**
- Beaucoup de blanc, le bleu franc pour le seul CTA de chaque section, le vert en pastilles et en décor (« sans engagement » en texte encre sur pastille verte). Inspirations : n° 17 pour le blanc et le bleu.
- Pas de photo d'équipe : le logo, des illustrations et des icônes au trait (n° 17), et un bloc « Qui sommes-nous » court.
- La ville dans le H1 et une pastille de zone au-dessus (n° 1, 19), le téléphone sous le CTA (n° 17, 5).
- Le bloc avis en gabarit, sans ligne de note sous le CTA (n° 18).
- Le devis en 3 étapes nommées, le repère de prix avant les coordonnées (n° 21, 5).
- Le curseur avant/après au clavier (n° 22, 25).
- La carte des communes en SVG et la liste en texte, à dessiner (aucune inspiration).
- C'est la plus facile à décliner pour un autre métier : seuls les textes, les icônes et `brand.green` changent (critère de réussite du brief).

**Directions retirées**
- **B « Artisan de quartier »** : son fond teinté s'écarte du « blanc » de la marque, et elle se décline moins vite pour un autre métier, alors que le brief demande moins d'une journée. Son bon élément (carte des communes) est déjà exigé par le brief et passe dans la direction unique.
- **C « Le comparateur »** : l'estimateur dans le hero prend la place du message local du bloc Hero, et le brief place le devis en bloc 7. Elle s'appuyait sur Flatiron Maids (n° 20), hors de la marque.

---

## Palette, polices, design tokens, composants

Contrastes calculés selon la formule WCAG 2.1. Le fond de référence est `bg.default` (`#FFFFFF`). Toutes les valeurs ont été revérifiées contre la section 9 du brief (marque et accessibilité) ; les 3 corrections sont signalées.

### Palette

Les observations la confortent : les CTA verts des concurrents portent du texte blanc à 3,0:1 (Coverall, `#00AB48`) et 3,8:1 (Office Pride, `#00964D`), le bouton orange de Companeo tombe à 2,2:1. Garder le vert en décor et le bleu `#1D4ED8` (6,7:1) pour les CTA évite ce défaut.

| Rôle | Hex | Usage |
|---|---|---|
| Blanc | `#FFFFFF` | Fond principal |
| Bleu franc | `#1D4ED8` | CTA, liens, titres d'accent. Contraste de 6,7:1 sur blanc, blanc sur bleu : 6,7:1 |
| Bleu très clair | `#EFF6FF` | Fonds de section, cartes. Le bleu y garde un contraste de 6,2:1 |
| Vert frais | `#22C55E` | Pastilles, bordures et icônes décoratives. **Jamais du texte sur blanc** (2,3:1), ni une icône porteuse de sens (sous 3:1). Texte encre sur vert : 7,8:1 |
| Vert texte | `#15803D` | Mentions « ✓ » en texte et coches porteuses de sens sur blanc (5,0:1). Ce n'est pas le vert accent |
| Encre | `#0F172A` | Corps de texte (17,9:1) |
| Gris | `#475569` | Texte secondaire (7,6:1) |

### Polices Google Fonts

- **Figtree** (700 et 800) pour les titres, **Figtree** (400 et 500) pour le texte. Une seule famille, conforme au brief.
- Alternative : **Nunito Sans**.
- Relevé chez les concurrents : Bricolage Grotesque et Hanken Grotesk (Lebontri), Montserrat (Onet), Roboto Condensed en capitales (Coverall), CeraPro (Office Pride), Roboto (Companeo). Rien ne justifie de changer.

### Couleurs (tokens)

| Token | Hex | Usage | Contraste |
|---|---|---|---|
| `brand.blue` | `#1D4ED8` | CTA, liens, accents de titre, icônes porteuses de sens | 6,7:1. Blanc sur bleu : 6,7:1. Sur `brand.green-50` : 6,4:1 |
| `brand.blue-hover` | `#1E40AF` | Survol du CTA | 8,7:1 |
| `brand.blue-50` | `#EFF6FF` | Fonds de section, cartes | Le bleu y garde 6,2:1 |
| `brand.green` | `#22C55E` | Pastilles, bordures, icônes décoratives | **2,3:1 sur blanc, donc jamais en texte ni en icône porteuse de sens** (corrigé). Texte encre sur vert : 7,8:1 |
| `brand.green-50` | `#F0FDF4` | Fond des encarts « sans engagement » | sans objet |
| `semantic.success` | `#15803D` | Messages de succès, coches en texte | 5,0:1 (4,8:1 sur `brand.green-50`) |
| `semantic.error` | `#B91C1C` | Erreurs de formulaire | 6,5:1 |
| `semantic.warning` | `#B45309` | Avertissements (« estimation indicative ») | 5,0:1, et 4,6:1 sur `brand.blue-50` (encart d'estimation) |
| `neutral.900` | `#0F172A` | Corps de texte | 17,9:1 |
| `neutral.600` | `#475569` | Texte secondaire | 7,6:1 |
| `neutral.400` | `#7A8699` | Bordures de champs (≥ 3:1) | 3,7:1 |
| `neutral.200` | `#CBD5E1` | Séparateurs décoratifs | décoratif |
| `bg.default` | `#FFFFFF` | Fond | sans objet |

Déclinaison métier : seul `brand.green` change (par exemple un orange pour la maintenance, un vert plus profond pour les espaces verts). On recalcule alors le contraste.

### Typographie (Figtree)

| Token | Taille (mobile / desktop) | Graisse | Interligne |
|---|---|---|---|
| `h1` | 30 / 48 px | 800 | 1,15 |
| `h2` | 24 / 34 px | 700 | 1,2 |
| `h3` | 19 / 22 px | 700 | 1,3 |
| `body-lg` | 18 / 19 px | 400 | 1,6 |
| `body` | 16 / 17 px | 400 | 1,6 |
| `small` | 14 px | 500 | 1,5 |
| `price` (estimation) | 32 / 40 px | 800 | 1,1, chiffres tabulaires |

### Espacement, rayons, ombres, motion

| Catégorie | Tokens |
|---|---|
| Espacement (base 4) | `space.1`=4, `2`=8, `3`=12, `4`=16, `6`=24, `8`=32, `12`=48, `16`=64, `20`=80 px. Sections : 56 px en mobile, 80 px en desktop |
| Rayons | `radius.sm`=8 px (champs), `radius.md`=12 px (boutons), `radius.lg`=20 px (cartes, photos), `radius.full` (pastilles) |
| Ombres | `shadow.sm` = 0 1px 3px rgba(15,23,42,.08) ; `shadow.md` = 0 6px 20px rgba(29,78,216,.10) ; `shadow.focus` = 0 0 0 3px rgba(29,78,216,.45) |
| Motion | `duration.fast`=120 ms, `duration.base`=200 ms (changement d'étape du devis), `duration.slow`=300 ms (apparition de l'estimation). `ease.out` = cubic-bezier(.2,.8,.2,1). Respecter `prefers-reduced-motion` |

### Composants clés

**Bouton primaire** : fond `brand.blue`, texte blanc, `radius.md`, hauteur 48 px.
- Survol : `brand.blue-hover`.
- Focus : `shadow.focus`.
- Actif : translateY(1px).
- Désactivé : opacité 0,5 et `aria-disabled`.
- Chargement : spinner et libellé « Envoi… ».

**Bouton secondaire** : fond blanc, bordure de 1,5 px `brand.blue`, texte bleu. Survol : fond `brand.blue-50`. C'est le bouton « Appeler » de la barre mobile.

**Barre mobile fixe** : 2 boutons de largeur égale (secondaire « Appeler », primaire « Devis »), hauteur 56 px (au-dessus des 44 px du brief), `safe-area-inset-bottom` respecté. Elle est masquée quand le formulaire de devis est visible.

**Carte de prestation** : fond `bg.default`, bordure `neutral.200`, `radius.lg`, icône au trait `brand.blue` sur pastille `brand.green-50` (couleur de l'icône précisée). Elle contient un titre `h3`, une ligne « pour qui », la fréquence et un lien d'action (« Estimer le nettoyage de mes bureaux »). Au survol : `shadow.md`.

**Formulaire de devis en 3 étapes** :
- barre de progression « Étape 2 sur 3 », étapes nommées ;
- étape 1 : type de local en cartes radio ;
- étape 2 : surface en tranches ou champ numérique, fréquence en pastilles, puis « Voir mon estimation » et le repère de prix au m² dans un encart `brand.blue-50`, avec sa source (Companeo) et la mention `semantic.warning` « indicatif, confirmé après visite » ;
- étape 3 : nom, téléphone, e-mail, code postal et message facultatif, avec labels visibles, puis « Recevoir mon devis » et la mention RGPD sous le formulaire ;
- erreur sous le champ, en texte et avec icône, et `aria-describedby`.

**Bloc avis** : la note en grand (`price`), des étoiles avec un texte alternatif au format « [note] sur 5, [nombre] avis Google », 3 verbatims avec prénom, initiale, date et source, et un lien vers la fiche. Dans la démo, les crochets restent visibles et le bloc porte la mention « Exemple de mise en page » : Brillance Pro n'a pas d'avis.

| À faire | À ne pas faire |
|---|---|
| Un seul CTA primaire par section | « Devis », « Contact » et « Rappel » côte à côte au même poids |
| Le vert en pastilles, bordures et décor | Du texte ou une icône porteuse de sens en vert clair sur blanc (2,3:1) |
| L'estimation affichée avant de demander les coordonnées | Les coordonnées exigées dès l'étape 1 |
| Le téléphone en lien `tel:`, visible dans l'en-tête | Le numéro en image ou en pied de page seulement |
| Des images compressées (WebP/AVIF, SVG) avec dimensions fixées | Des photos de banque d'images lourdes qui décalent la mise en page |
| Les avis datés, sourcés, avec un lien vers la fiche Google | Des avis sans date ni source, ou un widget qui charge 500 Ko de JavaScript |
| Un focus visible et un curseur avant/après utilisable au clavier | Un curseur uniquement au glisser |
| Une carte des communes en SVG et la liste en texte | Une carte Google ou OSM chargée d'office |

---

## Arbitrages

Brillance Pro est fictive : nous décidons.

- **Pack local** : on suit la position sur les 2 requêtes nommées dans le brief (« nettoyage bureaux Bordeaux », « entreprise de nettoyage Mérignac »), sans cible chiffrée. Une cible serait inventée, et ces 2 requêtes couvrent déjà la ville-centre et la périphérie.
- **Vert accent** : on garde `brand.green` (`#22C55E`) en décor seulement (pastilles, bordures, icônes décoratives), parce qu'il fait 2,3:1 sur blanc, sous le 3:1 du critère WCAG 1.4.11. Les coches porteuses de sens passent en `semantic.success` (`#15803D`, 5,0:1), et chaque couleur d'accent d'une déclinaison métier repasse le même calcul.
- **Avis Google** : on n'affiche ni note, ni nombre, ni verbatim, parce que Brillance Pro n'a pas d'avis. Le bloc est livré en gabarit marqué « Exemple de mise en page », et la ligne de note sous le CTA du hero est retirée de la démo.
- **Photos d'équipe** : on fait un bloc « Qui sommes-nous » court, sans photo, avec le logo. Unsplash (« Access Denied ») et Pexels (vérification Cloudflare) ont bloqué la recherche le 2026-11-13, et on ne contourne pas.
- **Délai de devis** : le H1 devient « Nettoyage de bureaux à Bordeaux, estimation en ligne immédiate », parce que « devis en 24 h » était un délai promis par une entreprise qui n'existe pas. L'estimation immédiate, elle, est une fonction du site.
- **Prix** : l'étape 2 du devis affiche le repère public de [Companeo](https://www.companeo.com/nettoyage-de-locaux/FAQ/prix-prestation-nettoyage-bureaux-ou-locaux-professionnels) qui correspond au local (3 à 5 € HT par m² pour de petits bureaux ou commerces, 2 à 3,50 € HT par m² pour une PME, page mise à jour le 25/05/2026, vue le 2026-11-13), avec la source écrite dessous. On ne calcule pas de montant mensuel, car la page ne précise pas la période, et les cartes de prestations n'ont pas de « à partir de ».
- **Labels** : aucun logo de label (Qualipropre, Ecolabel européen), parce qu'un logo renvoie à une certification réelle. « Produits écolabellisés » reste en texte, comme les autres traits de l'entreprise fictive.
- **Fiche Google et indexation** : on ne crée pas de fiche Google Business Profile, ce serait la fiche d'une entreprise qui n'existe pas. Le livrable devient un modèle de contenu de fiche, et la démo est publiée en `noindex`.
- **Avant / après** : 3 ou 4 paires de photos à produire, légendées « photo d'illustration » et le type de local. Pas de lieu ni de date, qui seraient inventés.
- **Assurance et préavis** : « attestation d'assurance envoyée sur demande » en texte, sans fichier, et « préavis écrit dans le contrat » sans durée. On ne fabrique ni document ni délai.

---

## À côté

| # | Référence | Capture | Pourquoi à côté |
|---|---|---|---|
| 2 | [Lebontri : Nettoyage de bureau à Tours](https://lebontri.fr/nettoyage-bureau/tours) (plateforme FR) | [capture](captures/a-cote/02-lebontri-tours.jpg) | Page-ville dupliquée : seuls la ville, la fin du H1 et le département changent. Le brief interdit les « pages-villes générées en masse ». La promesse « devis sous 24h » a disparu du title. Seul le format du title est repris (voir Pages SEO). |
| 6 | [Lebontri : simulateur (Valenciennes)](https://lebontri.fr/nettoyage-bureau/valenciennes) (plateforme FR) | [hero](captures/a-cote/06-lebontri-valenciennes.jpg), [estimation](captures/a-cote/06-lebontri-valenciennes-estimation.jpg) | Pas de simulateur : ni champ ni prix, l'estimation est floutée (« ••• € ») et demande un compte, contre « l'estimation immédiate » du brief. Photo de techniciens dans une salle de bain moisie sur une page de bureaux, hors sujet. Seules les 4 cartes de facteurs de prix sont reprises (bloc 7). |
| 7 | [Coverall : estimateur janitorial](https://www.coverall.com/commercial-cleaning-services/janitorial/) (site réel US) | [hero](captures/a-cote/07-coverall-janitorial.jpg), [estimateur](captures/a-cote/07-coverall-janitorial-estimateur.jpg) | Une estimation « instantanée » de 10 champs qui exige les coordonnées avant la fourchette, contre l'ordre du devis du brief (fourchette à l'étape b, coordonnées à l'étape c). H1 en capitales condensées 80 px, CTA blanc sur `#00AB48` (3,0:1), contre WCAG AA. Seul le périmètre en 5 tâches est repris (bloc 2). |
| 8 | [Coverall : Get a Quote](https://www.coverall.com/get-a-quote/) (site réel US) | [capture](captures/a-cote/08-coverall-get-a-quote.jpg) | Photo de banque d'images cliché (4 agents souriants face à l'objectif, gants verts). 6 champs obligatoires dont les coordonnées. Seul le paragraphe « How we determine your quote » est repris (bloc 7). |
| 9 | [Stratus : Get a Quote](https://www.stratusclean.com/get-quote/) (site réel US) | inaccessible | **Non vérifié** : protection anti-robots (Cloudflare), non contournée. |
| 10 | [Stratus : devis Miami](https://www.stratusclean.com/locations/miami/get-quote/) (site réel US) | inaccessible | **Non vérifié** : protection anti-robots (Cloudflare), non contournée. Une page devis par implantation ne sert pas : Brillance Pro a une seule zone. |
| 11 | [Companeo : devis express nettoyage](https://www.companeo.com/nettoyage-de-locaux/devis-express) (plateforme FR) | [capture](captures/a-cote/11-companeo-devis-express.jpg) | Comparateur de 4 sociétés, pas une entreprise locale. H1 bleu `#00A3E4` à 2,8:1 et bouton blanc sur orange `#F89827` à 2,2:1, contre WCAG AA. Photo de banque d'images et carte de France à figurines 3D. Il promet la rapidité de la demande (« 60 secondes chrono »), pas de la réponse. Seules les cartes de type de local sont reprises (bloc 7). |
| 12 | [Coverall Fresno : plus de 100 avis Google 5 étoiles](https://www.coverall.com/in-the-news/coverall-of-fresno-reinforces-role-as-the-best-commercial-cleaning-provider-with-5-star-rating-and-over-100-google-reviews/) (site réel US) | [capture](captures/a-cote/12-coverall-fresno-avis.jpg) | Communiqué du 19 août 2026 en texte seul. Le seul verbatim est anonyme et non daté, contre la règle du brief « indiquer leur source et leur date ». Seule l'idée de la note dans un titre est reprise (bloc 6). |
| 13 | [Coverall Gainesville : 40e avis 5 étoiles](https://www.coverall.com/in-the-news/coverall-of-gainesville-celebrates-40th-5-star-review-and-perfect-5-star-google-rating-reinforcing-role-as-best-commercial-cleaning-service-in-gainesville-fl/) (site réel US) | [capture](captures/a-cote/13-coverall-gainesville-avis.jpg) | Contexte sectoriel seulement : communiqué du 2 septembre 2026, citation de la direction et pas d'un client. Il montre qu'un franchisé local fait une annonce de son 40e avis. |
| 14 | [Coverall : Pricing Commercial Cleaning Services](https://www.coverall.com/commercial-cleaning-services/pricing-commercial-cleaning-services-for-your-business/) (site réel US) | [capture](captures/a-cote/14-coverall-pricing.jpg) | Contexte sectoriel seulement : article de blog en texte seul, sans icônes ni estimateur. Il cite la surface, la fréquence et le nombre de tâches. Seul le ton est repris (bloc 7). |
| 15 | [Coverall : FAQ nettoyage commercial](https://www.coverall.com/faqs/commercial-cleaning/) (site réel US) | [capture](captures/a-cote/15-coverall-faq.jpg) | Pas de bloc FAQ dans l'arborescence du brief. Photo de foule de banque d'images, cliché. 14 questions en capitales, sans données FAQPage. |
| 20 | [Local Cleaning Service Website, Flatiron Maids](https://dribbble.com/shots/27650887-Local-Cleaning-Service-Website-Landing-Page-UI) (Dribbble, Jabel Ahmed) | [capture](captures/a-cote/20-dribbble-flatiron-maids.jpg) | Hors de la marque du brief (orange, fond turquoise, titres à empattements en capitales) et ménage à domicile. L'estimateur dans le hero remplace le message local du bloc Hero. Seul l'argument « Want the same team? » est repris (bloc 3). |
| 23 | [KD Enterprises, Commercial Cleaning & Facility Landing page](https://dribbble.com/shots/27818578-KD-Enterprises-Commercial-Cleaning-Facility-Landing-page) (Dribbble, Carlos Pessane) | [capture](captures/a-cote/23-dribbble-kd-enterprises.jpg) | Contre-exemple : femme en tablier avec éponge et gants rouges, étincelles dorées, « We provide Efficient Cleaning Services ». Rien ne dit qui, où ni à quel prix, contre le H1 local du brief. |
| 24 | [Cleaning Service Website Examples](https://onepagelove.com/tag/cleaning-service) (One Page Love) | [capture](captures/a-cote/24-onepagelove-cleaning-service.jpg) | URL mortes : 4 exemples de 2012-2013, tous hors ligne. Mascottes (super-héros « Schluss mit Schmutzig », chapeau haut-de-forme), hors du ton « simple, professionnel » du brief. |

**Clichés croisés** : agents souriants face à l'objectif avec gants colorés (n° 8, 23), femme à l'éponge et étincelles (n° 23), mascotte (n° 24), foule de banque d'images (n° 15), carte de France à figurines 3D (n° 11), photo spectaculaire hors sujet (n° 6), logos factices (n° 19). Le secteur a peu de références soignées : une vitrine nette se démarque vite.

---

## Galeries : requêtes lancées

| Date | Plateforme | Requête | Résultat |
|---|---|---|---|
| 2026-11-12 | Dribbble | « cleaning service website », « commercial cleaning landing page », « office cleaning website » | Retenus : n° 17, 18, 19 (inspirations), n° 20, 23 (à côté) |
| 2026-11-12 | Dribbble | « multi step quote form » | Retenu : n° 21 |
| 2026-11-12 | Dribbble | « before after slider » | Retenu : n° 22 |
| 2026-11-12 | One Page Love | tag « cleaning-service » | n° 24 (à côté) |
| 2026-11-12 | Web | curseur avant/après d'un vrai site de nettoyage (anglais et français) | Aucun site réel ; page Jan-Pro en erreur 403. Composant n° 25 retenu |
| 2026-11-12 | Behance | | Inaccessible, erreur HTTP 400 renvoyée au navigateur automatisé |
| 2026-11-12 | Pinterest | « cleaning business website design blue » | Fenêtre de connexion obligatoire, aucun lien de pin lisible |
| 2026-11-12 | Land-book | | Inaccessible (protection anti-robots, challenge Cloudflare persistant) |
| 2026-11-12 | Lapa Ninja | | Inaccessible (protection anti-robots, page « Sorry, you have been blocked ») |
| 2026-11-12 | Awwwards | « cleaning » | Sites d'agences et de portfolios sans rapport, aucun retenu |
| 2026-11-12 | Godly | | godly.website redirige vers recent.design, sans recherche et sans site de services locaux |
| 2026-11-12 (refonte) | Dribbble | « service area map » | 1 shot ouvert (« Service Area Map & Wide Coverage ») : carte Google intégrée, contre le brief. Non retenu |
| 2026-11-12 (refonte) | Dribbble | « areas we serve », « service area », « locations we serve » | Sites d'artisans américains (plomberie, déménagement, élagage) et hors sujet. 1 shot plomberie ouvert, section zone non lisible dans la capture. Non retenu |
| 2026-11-12 (refonte) | Dribbble | « how it works cleaning » | 3 shots ouverts : Gala Cleaning (photos de banque d'images, gants jaunes), CleaniX (banque d'images, logos de marques, ménage à domicile), Bella Cleaning (magenta et empattements, ton luxe B2C). Hors marque ou clichés. Non retenus |
| 2026-11-13 | Unsplash | « office cleaning » (photos d'équipe) | Page « Something went wrong », « Access Denied ». Rien retenu |
| 2026-11-13 | Pexels | « office cleaning » (photos d'équipe) | Vérification anti-robots Cloudflare persistante, non contournée. Rien retenu : bloc « Qui sommes-nous » sans photo |
