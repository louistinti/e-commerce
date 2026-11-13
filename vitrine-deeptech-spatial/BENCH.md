# Benchmark visuel : Strate Orbital (entreprise fictive)

Ce bench suit le brief client bloc par bloc : chaque référence retenue sert un bloc de l'arborescence ou une contrainte précise du [brief](BRIEF-CLIENT.md).

## Limites, à lire en premier

**Vérification du 2026-11-12**, faite avec un vrai navigateur (Chrome piloté par Playwright).

- **Ce qui a été vu** : 14 des 20 références d'origine ont été ouvertes à leur adresse, et 13 capturées (Kinéis, n° 5, a été lue sans pouvoir être capturée). 5 autres, bloquées, ont été remplacées par une page équivalente ouverte et capturée (le site réel ou une page Dribbble : n° 3, 4, 13, 17 et 18). Une seule reste sans équivalent direct (n° 19, Behance), remplacée par 4 captures mobiles de 3 sites réels. Une référence a été ajoutée (n° 21). Les captures sont en 1440 × 900 px, au-dessus de la ligne de flottaison. Les fichiers en `NNb` sont une seconde capture ciblée sur un élément clé plus bas. Les couleurs et les polices citées ont été relevées dans la page (`getComputedStyle`) ou dans la fiche Awwwards et Dribbble, pas devinées. Les chiffres cités sont ceux affichés le 2026-11-12.
- **Bloqué, et pourquoi** :
  - Behance (n° 3 et 19) renvoie une erreur 400 au navigateur automatisé.
  - Lapa Ninja (n° 4) et Land-book (n° 13) bloquent par Cloudflare.
  - Pinterest (n° 17 et 18) affiche un mur de connexion. Aucune capture n'a été faite (c'est une page de connexion).
  - L'article Fast Company cité au n° 1 s'affiche vide pour le navigateur automatisé.
  - Kinéis (n° 5) a répondu par des erreurs 429 (trop de requêtes) sur toutes ses feuilles de style : le texte a été lu, la mise en page n'a pas été vue. Pas de capture.
- **Corrections importantes** (vérification du 2026-11-12, toujours valables) :
  - Kinéis (n° 5) : la phrase « pas de gros flux » n'est pas sur la page. Les chiffres sont confirmés, avec 20 stations sol (et non « environ 20 »).
  - EnduroSat (n° 16) : ce n'est pas un site « sans effets ». La fiche Awwwards porte les tags Parallax, Video, 3D et Transitions.
  - Cowboy Space (n° 4) : la palette n'est pas noire mais brun très sombre, avec un bouton orange. La phrase « Earth's energy grid can't run at the pace of AI » est dans le paragraphe sous le titre, pas dans le hero.
  - Turion (n° 1) : l'étude de cas ne parle pas de parallaxe. BUCK a signé l'identité et des rendus 3D, pas des photos.
  - Anduril (n° 15) : la fiche Fonts In Use date d'avril 2020 et montre un site sur fond blanc. Le site de 2026 est sur fond noir.
  - Roobinium (n° 20) : c'est une landing de jeu crypto et NFT, pas un site spatial.
  - Shakuro (n° 2) : le shot est signé Conceptzilla seul.
- **URL morte** : le site primé NASA Spacecrafts (n° 8) n'existe plus, le domaine redirige vers une page de parking. Toutes les autres URL d'origine répondent.
- **Passe du 2026-11-13** : aucun chiffre propre à l'entreprise fictive n'est conservé. Les chiffres du bench sont ceux observés sur les pages citées, avec leur URL. Les photos d'équipe ont été cherchées sur Unsplash puis Pexels, sans résultat (bloc 7). Les anciennes questions ouvertes sont devenues des [arbitrages](#arbitrages).
- **Bannières cookies** : refusées partout où un refus existait. **Données personnelles** : avatars floutés sur les pages Dribbble et Awwwards ; sur le n° 20, l'e-mail et le téléphone affichés ont été masqués.

**Refonte du 2026-11-12** (tri et réorganisation selon le brief) :

- **Tri** : chaque référence est classée « inspiration » (au moins un élément sert une exigence précise du brief, sans contredire la marque ni ses interdits) ou « à côté » (contre-exemple, hors marque, URL morte, non vérifié). Rien n'a été supprimé. Les captures mobiles sont triées une par une, comme des références.
- **Résultat** : 18 références et 2 captures mobiles en inspiration, dans [`captures/inspis/`](captures/inspis/). 5 références et 2 captures mobiles à côté, dans [`captures/a-cote/`](captures/a-cote/). Les numéros et les noms de fichiers n'ont pas changé.
- **Nouvelle organisation** : un tableau de couverture du brief, puis les inspirations rangées dans l'ordre de l'arborescence du brief (section 6), puis le mobile, les directions, les tokens et la liste « à côté ».
- **Nouvelles références** : 2 (n° 22 et 23), pour la feuille de route et le formulaire de contact, qui n'avaient aucune inspiration. Dribbble a demandé une vérification anti-robots à la deuxième recherche : la recherche a été arrêtée là, sans contourner.
- **Directions** : 3 pistes ramenées à 2, comme le demande le brief (« 2 pistes, puis 1 »). La piste C est retirée, la raison est donnée plus bas.
- **Tokens corrigés** (détail dans la section Palette) :
  - l'orange assombri `#C2410C` n'est plus annoncé « pour le texte » en mode clair : le brief interdit l'orange en texte courant sur fond clair ;
  - valeurs du mode clair ajoutées pour le texte secondaire, le focus et les couleurs sémantiques, qui échouaient sur `#F4F4F1` (de 1,9:1 à 3,0:1) ;
  - `type.display` passe d'IBM Plex Sans Condensed à IBM Plex Sans : le brief impose Plex Sans et Plex Mono seulement ;
  - ajout d'un bouton pause pour l'orbite animée (critère WCAG 2.2.2).

---

## Couverture du brief

| Exigence du brief | Inspirations | Manque |
|---|---|---|
| 1. Hero (visuel orbital léger, phrase de mission, 2 CTA) | 1, 2, 3, 4, 7, 13, 16, 21 | Aucune référence ne montre les deux CTA du brief côte à côte. Le hero de Cowboy Space (n° 4) est une vidéo, trop lourde pour le Lighthouse mobile visé. |
| 2. La technologie à 3 niveaux (En bref, Pour les ingénieurs, Publications) | 2, 5, 6, 7, 18 | Aucune liste de publications avec DOI vue, ni de bilan de précision. Le n° 5 n'a pas de capture (mise en page non vue). |
| 3. Applications (problème, donnée, décision) | 10, 11, 12 | Aucune référence ne présente 3 cas d'usage côte à côte avec la décision rendue possible. Rien sur l'assurance climatique ni l'indice paramétrique. |
| 4. Feuille de route (horizontale sur desktop, verticale sur mobile, statuts) | 9, 22 | Aucune timeline horizontale à défilement lent vue. L'axe vertical des années du n° 8 est utile mais à côté (URL morte), cité avec renvoi. |
| 5. Données (carte, curseur 30 jours, légende accessible, tableau) | 7, 10, 11, 12, 13 | Aucun tableau de valeurs en alternative à la carte, aucun curseur temporel jour par jour vu en fonctionnement. |
| 6. Partenaires et financeurs (logos monochromes, nature du soutien) | 21 | Le n° 21 montre l'emplacement et les logos monochromes, mais sans la nature du soutien. Aucune référence n'affiche « lauréat de… » ou « contrat d'étude… » à côté d'un logo. |
| 7. Qui sommes-nous et recrutement (bloc court sans photo, 3 offres, page carrière) | 14 | Aucune offre qui décrit le problème technique à résoudre (attente de P3). Pas de photo d'équipe : Unsplash et Pexels ont bloqué le navigateur le 2026-11-13, le bloc passe à un « Qui sommes-nous » sans photo. |
| 8. Presse et contact (3 retombées, kit presse, formulaire segmenté, plan) | 23 | Aucun formulaire segmenté par type de demandeur, aucun kit presse, aucune retombée presse, aucun plan vus. Le n° 23 ne couvre que les libellés visibles et le compteur d'étapes. |
| Mobile (timeline verticale, visuels allégés, données en tableaux, Lighthouse ≥ 90) | 3, 9, 12, 22, mobile Spaceflux, mobile constellr | Aucune carte de données vue sur mobile avec sa légende au bon endroit (le seul cas vu est à côté). |
| Marque (noir, blanc, orange signal ; IBM Plex Sans et Mono ; sombre par défaut, bascule vers le clair) | 3, 4, 6, 7, 10, 13 | Aucune référence n'utilise Plex Mono. Le noir et l'orange sont déjà pris par d'autres acteurs (n° 4, 7, et le n° 20 à côté). |
| Accessibilité (WCAG 2.2 AA, `prefers-reduced-motion`, carte doublée d'un tableau, contrastes) | 4, 10, 22, mobile constellr | Aucune bascule « réduire les animations » vue. Aucun tableau alternatif à une carte. |
| Preuve « chaque jour, à la parcelle » (carte, résolution, revisite) | 3, 10, 11, 16 | Aucune. Dans la démo, la carte s'appuie sur des données publiques Copernicus, citées sur la carte, et aucun chiffre de performance n'est inventé (voir [Arbitrages](#arbitrages)). |
| Preuve « une mesure, pas une estimation » (courbe contre sondes au sol, DOI) | 10 (en partie) | Le n° 10 montre une courbe 2015 à 2024, pas une comparaison avec des mesures au sol. Aucun lien DOI vu. |
| Preuve « déjà en orbite » (timeline, première image datée) | 9, 11, 22 | La première image datée n'a pas d'équivalent exact : le n° 11 date une image satellite, pas une première acquisition. |
| Preuve « soutenus par des acteurs publics » (logos avec la nature du soutien) | 21 (emplacement) | La nature du soutien n'apparaît nulle part (voir bloc 6). |
| Règle « chaque chiffre daté et sourcé, chaque vue d'artiste légendée » | 11, 14 | Aucune vue d'artiste légendée vue. Le n° 1 montre des rendus 3D sans qu'on sache s'ils sont légendés sur le site. |

---

## Inspirations, bloc par bloc

### 1. Hero

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 1 | [Turion Space, refonte par WILD](https://wild.as/work/turion-space) (étude de cas d'agence) | [capture](captures/inspis/01-turion-wild.jpg) | Petites mentions en capitales mono autour du visuel (« ORBIT WITH PURPOSE », « 001 »), sur fond noir. Site Framer, sur l'identité et les rendus 3D de BUCK. **À éviter** : le dégradé violet de l'horizon, hors palette. | Visuel orbital léger, entouré de repères courts en Plex Mono. |
| 2 | [Satellite Landing Page Animation (Conceptzilla)](https://dribbble.com/shots/16467758-Satellite-Landing-Page-Animation) (Dribbble) | [capture](captures/inspis/02-dribbble-satellite.jpg) | Un seul objet (un CubeSat) sur fond noir `#010101`, un titre qui répond à une question simple. **À éviter** : le logo NASA dans l'en-tête, que le brief interdit (pas d'emprunt à l'identité d'une agence spatiale). | Un seul visuel, une phrase de mission comprise en 30 s. |
| 3 | [Spaceflux](https://spaceflux.io/) (site réel, UK ; Behance d'origine non vérifié) | [capture](captures/inspis/03-spaceflux.jpg) | Titre « Space Intelligence » en IBM Plex Sans 80 px. Coordonnées GPS en petit corps en haut à gauche. Plus bas, 3 chiffres avec leur unité (« en 90 secondes », « jusqu'à 10 cm », 2,5 cm). **À éviter** : la palette violette (`#100919`, `#C09EFF`), et les coordonnées en 10 px (12 px minimum chez nous). | Preuves chiffrées avec unité, typographie Plex Sans. |
| 4 | [Cowboy Space](https://www.cowboyspace.com/) (site réel, US ; Lapa Ninja d'origine non vérifié) | [capture](captures/inspis/04-cowboy-space.jpg) | La structure « problème terrestre, puis réponse spatiale », dans le paragraphe sous le titre. Bouton orange `#F47D49` à texte sombre `#17191C` (6,6:1). **À éviter** : la vidéo plein écran et la police Panell Wide. | Sous-titre du brief (« piloter l'irrigation, anticiper la sécheresse… ») ; CTA primaire orange à texte sombre. |
| 7 | [Artificial Satellite (Hanwha Space Hub, FAVE®)](https://www.awwwards.com/sites/artificial-satellite) (Awwwards, mention honorable du 24 août 2023) | [élément](captures/inspis/07b-awwwards-earth-observation.jpg) | La Terre dans une orbite au trait, un réticule orange fin et des crochets de cadrage orange. Paire `#000000` et `#F77D16` (7,9:1). | Visuel orbital en SVG, en trait fin, qui n'alourdit pas la page. |
| 13 | [SkyFi](https://skyfi.com/) (site réel, US ; Land-book d'origine non vérifié) | [capture](captures/inspis/13-skyfi.jpg) | Coordonnées et libellés de boutons en DM Mono 13 à 14 px, crochets de cadrage au trait. Un seul accent, réservé au bouton d'action (`#FCC219`, texte noir, 12,9:1). | Un seul accent pour le CTA primaire ; le mono (Plex Mono chez nous) pour les coordonnées. |
| 16 | [EnduroSat](https://www.awwwards.com/sites/endurosat) (Awwwards, mention honorable du 20 août 2024) | [capture](captures/inspis/16-awwwards-endurosat.jpg) | Une grille de filets verticaux fins avec un chiffre en petites capitales par colonne (450+ années d'expérience cumulée, 230+ clients, 150+ personnes). **À éviter** : parallaxe, vidéo et 3D (tags de la fiche). | Ce que Claire (P1) doit voir en 30 s : la preuve en orbite et le marché, en faits datés et sourcés (chiffres de marché publics, aucun chiffre inventé). |
| 21 | [Starcloud, site orienté investisseurs (Flexy LLC)](https://dribbble.com/shots/27116861-Building-an-Investor-Focused-Website-for-Starcloud) (Dribbble) | [capture](captures/inspis/21-dribbble-starcloud.jpg) | Dès le premier écran, une ligne « Backed by » avec 4 logos blancs. Le shot vise « investisseurs, partenaires et ingénieurs », nos trois personas. **À éviter** : des logos sans la nature du soutien. | Une preuve de soutien visible dès le hero, pour P1. |

### 2. La technologie à 3 niveaux

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 2 | Conceptzilla (voir bloc 1) | [capture](captures/inspis/02-dribbble-satellite.jpg) | Une phrase de définition en mots simples (« moins de 10 kilogrammes »). | Onglet « En bref » compris sans jargon (plan de recherche, section 12). |
| 5 | [Kinéis, page Technologie](https://kineis.com/en/technology-kineis-iot/) (site réel, FR) | Pas de capture (erreurs 429), texte lu | Le fonctionnement en 4 étapes (objet, satellite, station sol, centre de service 24 h/24). Des chiffres avec unité : 25 nanosatellites, 650 km, 5 plans orbitaux, 20 stations sol, 80 passages par jour. Un renvoi vers une base de connaissances « pour les ingénieurs ». Aucune limite assumée sur la page : à écrire nous-mêmes. | « En bref » (3 phrases et un schéma) et passage vers « Pour les ingénieurs ». |
| 6 | [Pasqal](https://www.pasqal.com/) et sa [documentation](https://docs.pasqal.com/) (site réel, FR) | [capture](captures/inspis/06-pasqal.jpg) | La documentation technique séparée du site vitrine, reliée depuis le menu. **À éviter** : le titre en graisse 100 sur photo, et le bouton vert `#00C887` à texte blanc (2,2:1, échec AA). | Niveaux séparés, ici en onglets « Pour les ingénieurs » et « Publications ». |
| 7 | Hanwha Space Hub (voir bloc 1) | [capture](captures/inspis/07-awwwards-artificial-satellite.jpg) | Un module par sous-système (caméra EO/IR, antenne, liaison inter-satellites, SAR). | Le schéma de l'onglet « En bref » : un nanosatellite 6U, un module par fonction, sans détail de charge utile au-delà du publié. |
| 18 | [Orbita Spacecraft Mission UI (Notionhive)](https://dribbble.com/shots/27534165-Orbita-Spacecraft-Mission-UI) (Dribbble ; Pinterest d'origine non vérifié) | [capture](captures/inspis/18-dribbble-orbita-mission-ui.jpg) | Une fiche technique libellé gris, valeur blanche, alignée à droite, sous une mention en capitales « TECHNICAL SPECIFICATIONS ». Des orbites au trait fin. **À éviter** : les valeurs en 8 px environ, illisibles. | « Pour les ingénieurs » et la fiche technique attendue par Marc (P2) : résolution, revisite, formats, en Plex Mono. |

### 3. Applications

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 10 | [constellr, Dhun Climate Resilience Study](https://urban-resilience.constellr.com/) (microsite de données) | [capture](captures/inspis/10-constellr-dhun.jpg) | Une question, une réponse : le résultat chiffré est dans le titre (« 8°C Temperature Reduction »), puis 3 chiffres, une courbe, une carte et 4 cartes d'explication. **À adapter** : chez nous, la décision rendue possible est dans le titre, sans résultat chiffré (l'entreprise est fictive). | La structure de chaque cas d'usage : problème, donnée livrée, décision rendue possible. |
| 11 | [EarthEye, Agriculture Dashboard (Shakuro)](https://dribbble.com/shots/24596768-EarthEye-Agriculture-Dashboard-Design) (Dribbble) | [capture](captures/inspis/11-dribbble-eartheye.jpg), [tableau de bord](captures/inspis/11b-dribbble-eartheye-dashboard.jpg) | Un widget mobile (« Water, Dangerous Level, 98.4 % »), puis des parcelles détourées avec leurs mesures (sol 16,7 %, eau 92,2 %). **À éviter** : l'état codé seulement par vert, jaune et rouge. | Cas « agriculture » : la donnée à la parcelle, telle qu'un agriculteur la lit. |
| 12 | [Land Lines (Google Data Arts Team)](https://www.awwwards.com/sites/land-lines) (Awwwards, site du jour du 10 janvier 2017) | [capture](captures/inspis/12-awwwards-land-lines.jpg) | Une image satellite de pivots d'irrigation (cercles verts), lisible sans légende. | Visuel du cas « irrigation ». À légender (source, date), selon la règle du brief. |

### 4. Feuille de route

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 9 | [Roadmap timeline (Anastasia Dvorzhanska)](https://dribbble.com/shots/4258663-Roadmap-timeline) (Dribbble) | [capture](captures/inspis/09-dribbble-roadmap.jpg) | Timeline verticale : un nœud par jalon, la date en capitales (« JUN 2017 »), puis une ou deux lignes. **À éviter** : des nœuds tous identiques, qui ne distinguent pas le passé de l'avenir, et le dégradé vert. | Version mobile verticale ; carte jalon (date en `type.overline`, puis une ligne). |
| 22 | [Daily UI Component #4: Timeline Status (Tridip Thrizu)](https://dribbble.com/shots/5659998-Daily-UI-Component-4-Timeline-Status) (Dribbble, **ajouté le 2026-11-12**) | [capture](captures/inspis/22-dribbble-timeline-status.jpg) | Trois variantes de timeline verticale. Dans la première, chaque statut a une couleur **et** une icône : coche verte (fait), cercle bleu avec flèches (en cours), jaune, gris (à venir). La ligne est colorée jusqu'au jalon en cours. Palette de la fiche : `#020408`, `#0EAC4A`, `#1524AA`. **À éviter** : la deuxième variante, codée par la couleur seule ; et aucune variante n'a de libellé texte. | Statuts « réalisé / partiel / à venir » : couleur, icône et libellé texte ensemble (WCAG 1.4.1). |

Détail utile d'une référence à côté : l'axe vertical des années avec un point par lancement de NASA Spacecrafts (n° 8, [capture](captures/a-cote/08b-awwwards-nasa-timeline.jpg)) se lit bien sur mobile. Voir la section « À côté ».

### 5. Données

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 7 | Hanwha Space Hub (voir bloc 1) | [élément](captures/inspis/07b-awwwards-earth-observation.jpg) | Le réticule fin et les crochets de cadrage. | Le curseur de la carte (`color.brand.accent`), hors de l'échelle de couleurs. |
| 10 | constellr (voir bloc 3) | [carte](captures/inspis/10b-constellr-carte.jpg) | Deux cartes côte à côte, la légende divergente de −8 °C à +8 °C sous la carte, une carte d'explication par motif visible. Les chiffres techniques sont donnés : 30 m, ±2 K, 8 jours. **À noter** : l'orange y signifie « réchauffement » ; l'orange de marque n'entre donc pas dans notre échelle. | Légende accessible collée à la carte ; résolution et revisite affichées près de la carte. |
| 11 | EarthEye (voir bloc 3) | [tableau de bord](captures/inspis/11b-dribbble-eartheye-dashboard.jpg) | La source et la période écrites sur la carte (« Sentinel-hub 2024-11-04/2024-11-17 »), un panneau de calques repliable, un sélecteur de dates. | Règle « chaque chiffre daté et sourcé » appliquée à la carte ; curseur temporel. |
| 12 | Land Lines (voir bloc 3) | [capture](captures/inspis/12-awwwards-land-lines.jpg) | Les interactions « Draw » et « Drag » au doigt. | Le curseur temporel sur 30 jours, manipulable au doigt sur mobile. |
| 13 | SkyFi (voir bloc 1) | [capture](captures/inspis/13-skyfi.jpg) | Image satellite avec crochets de cadrage, coordonnées en mono. | Habillage de la carte : coordonnées et dates en Plex Mono. |

### 6. Partenaires et financeurs

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 21 | Starcloud (voir bloc 1) | [capture](captures/inspis/21-dribbble-starcloud.jpg) | Logos en blanc, monochromes et petits, alignés après une mention « Backed by ». **À éviter** : aucun logo ne dit la nature du soutien, ce que la règle du brief exige (« lauréat de l'appel X », « contrat d'étude ESA »). | Logos sobres en monochrome, ici des logotypes fictifs. La nature du soutien est écrite en texte, pas seulement au survol. |

### 7. Équipe et recrutement

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 14 | [Aura Aero, page Carrière](https://www.aura-aero.com/en/carriere) (site réel, FR) | [capture](captures/inspis/14-aura-aero-carriere.jpg), [chiffres](captures/inspis/14b-aura-aero-chiffres.jpg) | Un bloc de chiffres datés (250+ personnes, index d'égalité 94/100 en 2024) et les 4 implantations. Un processus de recrutement en 3 étapes. La photo d'équipe (prise par drone, autour de 3 avions) n'est pas reprise : pas de photo d'équipe chez nous. **À éviter** : les chiffres bleus `#0167FF` sur marine (3,6:1), valables seulement en grand corps. | Ce qu'Inès (P3) cherche : un processus clair et des faits sur l'entreprise. Chez nous, ces faits sont écrits sans chiffre (entreprise fictive). |

**Photos d'équipe, recherche du 2026-11-13** : Unsplash a renvoyé « Access Denied » dès la première recherche, et Pexels une vérification anti-robots de Cloudflare. Rien n'a été contourné. Décision : pas de photo d'équipe. Le bloc devient un « Qui sommes-nous » court (2 ou 3 phrases : l'origine en laboratoire, le métier, Toulouse), avec le logotype ou une illustration au trait. Aucune photo réelle n'est exigée.

### 8. Presse et contact

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 23 | [Contact Form (fyne digital creative)](https://www.awwwards.com/inspiration/contact-form) (élément Awwwards, **ajouté le 2026-11-12**) | [capture](captures/inspis/23-awwwards-fyne-contact-form.jpg) | Formulaire en français, libellés visibles en grand corps au-dessus d'un filet épais (« Prénom », « Nom »), le champ facultatif écrit en toutes lettres (« Société (optionnel) »), un compteur d'étapes « 01 / 02 » sur le côté. **À éviter** : le fond clair comme fond par défaut (le brief veut le sombre par défaut). | Formulaire à 5 champs maximum, libellés visibles, en deux étapes : « Vous êtes » d'abord, puis la suite adaptée. |

---

## Mobile

Le brief demande une timeline verticale sur mobile, des visuels allégés (pas de 3D), des données en tableaux simples, Lighthouse mobile ≥ 90 et LCP < 2,5 s. Observé à 390 × 844 px :

| Site | Capture | Ce qu'on a vu | Exigence du brief |
|---|---|---|---|
| Spaceflux (n° 3) | [mobile](captures/inspis/mobile-spaceflux.jpg) | Le visuel passe au-dessus du titre et rétrécit, sans disparaître. Titre en Plex Sans 54 px sur deux lignes. Aucun bouton visible dans le premier écran. Pas de défilement horizontal. | Visuel allégé mais présent. **À corriger chez nous** : le CTA primaire doit être dans le premier écran. |
| constellr (n° 10) | [hero](captures/inspis/mobile-constellr.jpg) | Hero propre : titre 36 px, bouton pleine largeur. | CTA primaire pleine largeur, comme prévu dans le composant bouton. |

Ce qu'on en retient :
- Le satellite SVG passe au-dessus du titre, plus petit, plutôt que supprimé (Spaceflux). Pas de scène 3D sur mobile.
- Le bouton principal est pleine largeur, dans le premier écran (constellr).
- La timeline est verticale, statut en couleur, icône et libellé (n° 9 et 22).
- Le curseur temporel se manipule au doigt (n° 12), et la carte est suivie de son tableau de valeurs.
- Les chiffres-clés passent en grille de 2 colonnes, entièrement visibles. Pas de carrousel (contre-exemple Pasqal, à côté).
- La légende est collée sous chaque carte (contre-exemple constellr carte, à côté). Aucun débordement horizontal à 390 px, carte comprise.

---

## Directions

Le brief prévoit 2 pistes de direction artistique, puis 1 (planning, S3-S4). Les deux pistes gardent la marque du brief : noir profond, blanc, orange signal, IBM Plex Sans et Mono, mode sombre par défaut avec une bascule vers le clair.

**Le noir et l'orange ne suffisent pas à distinguer Strate Orbital.** Cowboy Space (n° 4) a le même bouton orange à texte sombre, Hanwha (n° 7) la même paire, et la crypto aussi (n° 20, à côté). Spaceflux (n° 3) utilise déjà IBM Plex Sans en titre. La distinction doit venir de la grille, du mono et de la carte.

**Direction A : « Instrument »** (recommandée)
- Noir mat, grille stricte de filets fins, chiffres en Plex Mono avec leur unité et leur date, comme sur un tableau de bord de vol (n° 16, 13, 3).
- Un seul satellite en SVG, en trait fin, avec réticule et crochets de cadrage (n° 7), entouré de mentions courtes en mono (n° 1).
- L'orange est réservé au CTA, à l'état « en cours » et au curseur de la carte, toujours plat, sans halo.
- Une ligne de soutiens dès le hero, avec la nature de chaque soutien (n° 21, corrigé).

**Direction B : « Carte d'abord »**
- Le visuel orbital du hero est la trace au sol du satellite, en SVG, posée sur une tuile de la carte d'humidité qui s'anime lentement (n° 12 pour l'image agricole, n° 7 pour le trait).
- Plus proche de l'usage client (eau, agriculture), et le CTA secondaire « Explorer la carte d'exemple » prend tout son sens.
- Récit « une question, une réponse » pour les Applications et la section Données : la décision rendue possible dans le titre, sans résultat chiffré, légende sous la carte (n° 10), source et date sur la carte (n° 11).
- Exige la tuile de carte dès S2 : on la produit à partir du Surface Soil Moisture de Copernicus, cité sur la carte (voir [Arbitrages](#arbitrages)).

**Direction retirée : C « Archive de mission ».** Elle remplaçait le visuel orbital du hero par de grandes photos d'intégration et de lancement. Le brief demande un visuel orbital léger (bloc 1), ne prévoit aucune photo parmi les contenus à produire, et des photos d'intégration risquent de montrer une charge utile (contrainte de confidentialité et de double usage). Son point fort, la photo d'équipe (n° 14), ne tient plus : le bloc 7 passe à un « Qui sommes-nous » sans photo.

Le traitement en mode clair de constellr (n° 10) sert la bascule vers le mode clair, pas une section claire dans le mode sombre : le brief fixe le sombre par défaut.

---

## Palette recommandée (mode sombre par défaut)

Contrastes recalculés le 2026-11-12 (formule WCAG 2.x), puis vérifiés contre les contraintes du brief à la refonte.

| Rôle | Hex | Note |
|---|---|---|
| Fond | `#0A0B0D` | noir profond |
| Surface (cartes) | `#14171B` | |
| Filets et grilles | `#2A2F36` | décoratif uniquement (1,5:1 sur le fond) |
| Texte principal | `#F4F4F1` | blanc cassé, 17,9:1 sur le fond |
| Texte secondaire | `#9AA0A6` | 7,5:1 sur le fond, 6,8:1 sur la surface |
| Accent orange signal | `#FF5A1F` | 6,3:1 sur `#0A0B0D` ; **jamais en texte sur fond clair** (3,1:1 sur blanc, 2,8:1 sur `#F4F4F1`) |
| Mode clair : fond | `#F4F4F1` | texte `#0A0B0D` (17,9:1) |
| Mode clair : accent | `#C2410C` | **corrigé** : fond du CTA (texte `#F4F4F1`, 4,7:1) et éléments graphiques seulement. Le bench annonçait cette valeur « pour le texte », ce que le brief interdit (« l'orange n'est jamais utilisé pour du texte courant sur fond clair »). Les liens en mode clair sont en `#0A0B0D` soulignés. |
| Mode clair : texte secondaire | `#5C636A` | **ajouté** : `#9AA0A6` ne donnait que 2,4:1 sur `#F4F4F1` ; `#5C636A` donne 5,5:1 |
| Échelle d'humidité (séquentielle, de sec à humide) | `#6B5A3E` `#8C8A5A` `#4F8F86` `#3C7FB0` `#9CCBEB` | distincte de l'accent ; passée au simulateur de daltonisme en maquette (S3-S4), teinte ajustée si deux paliers se confondent |

Pour comparaison, relevé sur les sites vus : bouton orange de Cowboy Space `#F47D49` à texte `#17191C`, 6,6:1 ; orange `#F77D16` de Hanwha sur noir, 7,9:1 ; bouton vert de Pasqal à texte blanc, 2,2:1 (échec AA).

## Polices (Google Fonts)

- **IBM Plex Sans** : 400 et 500 pour le texte, 600 pour les titres, y compris le titre d'affichage du hero.
- **IBM Plex Mono** : 400 et 500 pour les chiffres, coordonnées, dates et légendes de la carte.
- **Corrigé** : l'option IBM Plex Sans Condensed pour les titres est retirée. C'est une famille à part, et le brief impose Plex Sans et Plex Mono. Elle n'est pas retenue (voir [Arbitrages](#arbitrages)).
- Observé : Spaceflux utilise déjà IBM Plex Sans en titre (80 px, graisse 400). Notre titre en graisse 600 et la grille aideront à ne pas lui ressembler.

## 3 « à ne pas faire »

1. Pas de nébuleuses, de néon ni de glassmorphism : c'est le cliché Dribbble et Pinterest (n° 17), hors palette du brief, et c'est aussi le code de la crypto (n° 20).
2. Pas de 3D WebGL plein écran ni de défilement détourné qui bloque l'accès aux chiffres : un investisseur doit pouvoir sauter le récit. Pas non plus de hero sans texte (Anduril 2026, n° 15).
3. Pas de vue d'artiste sans légende, ni de logo de partenaire sans la nature du soutien (Starcloud, n° 21).

---

## Design tokens

Le mode sombre est le mode par défaut. Les valeurs du mode clair sont entre parenthèses quand elles diffèrent.

### Couleurs

| Token | Hex | Usage |
|---|---|---|
| `color.brand.accent` | `#FF5A1F` (clair : `#C2410C`) | fond du CTA principal, état « en cours » de la timeline, curseur de la carte. Jamais pour du texte en mode clair. |
| `color.brand.accent-hover` | `#FF7440` (clair : `#9A3412`) | survol du CTA |
| `color.brand.on-accent` | `#0A0B0D` (clair : `#F4F4F1`) | texte sur fond orange (6,3:1 ; 7,3:1 au survol). En clair, 4,7:1 sur `#C2410C` et 6,6:1 sur `#9A3412` |
| `color.neutral.1000` | `#0A0B0D` | fond (clair : texte) |
| `color.neutral.900` | `#14171B` | surface des cartes |
| `color.neutral.700` | `#2A2F36` | filets, grilles |
| `color.neutral.400` | `#9AA0A6` (clair : `#5C636A`) | texte secondaire (7,5:1 sur le fond ; clair 5,5:1) |
| `color.neutral.50` | `#F4F4F1` | texte principal (clair : fond) |
| `color.semantic.success` | `#3FB950` (clair : `#1A7F37`) | jalon « réalisé », envoi réussi (7,8:1 ; clair 4,6:1) |
| `color.semantic.warning` | `#D4A72C` (clair : `#8A6100`) | jalon « partiel », donnée provisoire (8,8:1 ; clair 5,0:1) |
| `color.semantic.error` | `#F85149` (clair : `#B42318`) | erreur de formulaire, jalon « échec » (5,9:1 ; clair 6,0:1) |
| `color.focus` | `#7AB8FF` (clair : `#1F5FBF`) | anneau de focus, distinct de l'orange (9,5:1 ; clair 5,5:1) |
| `color.data.moisture.1` à `.5` | `#6B5A3E` `#8C8A5A` `#4F8F86` `#3C7FB0` `#9CCBEB` | échelle séquentielle, de sec à humide |

**Corrigé** : les valeurs claires des couleurs sémantiques, du texte secondaire et du focus manquaient. Les valeurs sombres reprises telles quelles échouaient sur `#F4F4F1` : succès 2,3:1, avertissement 2,0:1, erreur 3,0:1, focus 1,9:1, texte secondaire 2,4:1.

L'orange de marque et le rouge d'erreur sont proches. L'erreur porte donc toujours une icône et un libellé, et l'orange n'est jamais utilisé pour signaler un problème. Il n'entre pas non plus dans l'échelle de la carte : sur une carte satellite, l'orange se lit « chaud » ou « sec » (constellr, n° 10).

### Typographie

| Token | Police | Taille (desktop / mobile) | Graisse | Interlignage |
|---|---|---|---|---|
| `type.display` | IBM Plex Sans (**corrigé**, au lieu de Plex Sans Condensed) | 80 / 44 px | 600 | 1,0 |
| `type.h1` | IBM Plex Sans | 48 / 32 px | 600 | 1,1 |
| `type.h2` | IBM Plex Sans | 34 / 26 px | 600 | 1,15 |
| `type.h3` | IBM Plex Sans | 22 / 19 px | 500 | 1,3 |
| `type.body` | IBM Plex Sans | 18 / 16 px | 400 | 1,6 |
| `type.small` | IBM Plex Sans | 14 px | 400 | 1,5 |
| `type.data` | IBM Plex Mono | 15 px, chiffres tabulaires | 500 | 1,4 |
| `type.overline` | IBM Plex Mono | 12 px, majuscules, interlettrage 0,08 em | 500 | 1,2 |

Observé : les coordonnées de Spaceflux sont en 10 px et les valeurs de la fiche Orbita en 8 px environ. On garde 12 px au minimum pour `type.overline`.

### Espacement (base 4 px)

`space.1` 4 · `space.2` 8 · `space.3` 12 · `space.4` 16 · `space.6` 24 · `space.8` 32 · `space.12` 48 · `space.20` 80 · `space.32` 128 (respiration entre sections sur desktop ; 80 sur mobile).

### Rayons

`radius.none` 0 (sections, carte de données) · `radius.sm` 2 px (boutons, champs) · `radius.pill` 999 px (pastilles de statut de la timeline uniquement).

### Ombres

Pas d'ombre portée en mode sombre : la profondeur vient des surfaces (`neutral.900` sur `neutral.1000`) et des filets. `shadow.overlay` `0 8px 24px rgba(0,0,0,.5)` est réservé aux infobulles de la carte. Mode clair : `0 1px 2px rgba(10,11,13,.08)`.

### Motion

| Token | Valeur | Usage |
|---|---|---|
| `motion.duration.fast` | 120 ms | survol, focus |
| `motion.duration.base` | 240 ms | onglets « 3 niveaux », infobulles |
| `motion.duration.slow` | 600 ms | entrée d'un jalon de timeline |
| `motion.duration.ambient` | 60 à 90 s par boucle | orbite du satellite en SVG (lente, en boucle) |
| `motion.easing.standard` | `cubic-bezier(.2,0,0,1)` | |
| `motion.easing.orbit` | `linear` | |

`prefers-reduced-motion` : l'orbite est figée, les jalons sont affichés sans animation et le défilement de la timeline est natif.

**Ajouté** : l'orbite tourne plus de 5 secondes à côté d'autres contenus. Le critère WCAG 2.2.2 (niveau A) demande alors un moyen de la mettre en pause, même pour les visiteurs qui n'ont pas réglé `prefers-reduced-motion`. Un bouton « Mettre en pause l'animation » (icône et libellé accessible) est placé près du visuel. Même règle pour la timeline si elle défile seule.

### Composants clés

**Bouton primaire** (« Contacter l'équipe partenariats »)
- Fond `brand.accent`, texte `brand.on-accent`, IBM Plex Sans 500 en 16 px, hauteur 48 px, `radius.sm`. Pleine largeur sur mobile.
- États :
  - survol : `accent-hover` ;
  - focus : anneau `color.focus` de 2 px, décalé de 2 px ;
  - actif : luminosité −8 % ;
  - désactivé : `neutral.700` avec texte `neutral.400` et `aria-disabled` ;
  - chargement : libellé « Envoi… » et spinner.

**Bouton secondaire** (« Explorer la carte d'exemple »)
- Contour de 1 px `neutral.50`, texte `neutral.50`.
- États :
  - survol : fond `neutral.900` ;
  - focus : identique au primaire ;
  - désactivé : contour `neutral.700`.

**Carte jalon (timeline)**
- Date en `type.overline`, titre en `type.h3`, une ligne de description (n° 9). Dans la démo, le numéro d'étape (« ÉTAPE 01 ») remplace la date (voir [Arbitrages](#arbitrages)).
- Pastille de statut (`radius.pill`) : réalisé, partiel ou à venir, toujours avec une icône et un libellé texte (n° 22).
- Surface `neutral.900`, filet `neutral.700`.

**Formulaire de contact segmenté**
- Premier champ « Vous êtes » (investisseur, client, presse, candidat), qui adapte la suite (deux étapes, compteur visible, n° 23).
- 5 champs maximum, libellés visibles, champs facultatifs écrits « (facultatif) », erreurs sous le champ avec une icône et `aria-describedby`.

**Bouton pause de l'animation** (ajouté)
- Bouton icône de 44 × 44 px, contour `neutral.700`, libellé accessible « Mettre en pause l'animation » puis « Relancer l'animation ».

### À faire / À ne pas faire

| À faire | À ne pas faire |
|---|---|
| Orange réservé au CTA, à l'état « en cours » et au curseur de la carte | Orange pour les titres, les liens et les alertes en même temps, ou en texte sur fond clair |
| Chiffres en Plex Mono, avec leur unité et leur date | Chiffres arrondis sans date (« bientôt 100 satellites ») |
| Un seul visuel animé, léger (SVG), avec un bouton pause | Plusieurs scènes WebGL qui font chuter le Lighthouse mobile |
| Carte doublée d'un tableau de valeurs accessible, source et date écrites sur la carte | Carte seule, sans légende textuelle ni alternative |
| Vues d'artiste légendées « vue d'artiste » | Rendus 3D présentés comme des photos en orbite |
| Mode clair disponible et testé, avec ses propres valeurs de contraste | Mode sombre imposé avec du gris `#666` sur du noir |
| Chiffres-clés en grille de 2 colonnes sur mobile | Chiffres en carrousel horizontal coupé au bord |

---

## À côté

| # | Référence | Capture | Pourquoi à côté |
|---|---|---|---|
| 8 | [NASA Spacecrafts (Yanlin Ma)](https://www.awwwards.com/sites/nasa-spacecrafts) (Awwwards, site du jour du 11 juin 2018) | [capture](captures/a-cote/08-awwwards-nasa-spacecrafts.jpg), [timeline](captures/a-cote/08b-awwwards-nasa-timeline.jpg) | **URL morte** : nasaspacecraft.com redirige vers une page de parking. C'est aussi une expérience WebGL (Three.js, D3), contraire au visuel léger et au Lighthouse mobile ≥ 90 du brief. Un détail utile (l'axe vertical des années) est cité dans le bloc 4. |
| 15 | [Anduril, d'après Fonts In Use](https://fontsinuse.com/uses/32662/anduril-industries) (avril 2020) et [site 2026](https://www.anduril.com/) | [capture](captures/a-cote/15-fontsinuse-anduril.jpg), [site 2026](captures/a-cote/15b-anduril-2026.jpg) | Le hero de 2026 n'a aucun texte au-dessus de la ligne de flottaison : il échoue au critère de réussite du brief (comprendre la mission et le contact en 30 s). La fiche de 2020 montre un site blanc qui n'existe plus, en Helvetica Now, hors des polices du brief. Le seul détail utile (un seul accent, rare) est déjà porté par SkyFi (n° 13). |
| 17 | Space-themed Website Inspiration ([Pinterest](https://www.pinterest.com/ideas/space-themed-website-inspiration/943348102916/), non vérifié : mur de connexion ; vu à la place : [recherche Dribbble « space website »](https://dribbble.com/search/space-website)) | [capture](captures/a-cote/17-dribbble-recherche-space-website.jpg) | Contre-exemple : astronautes, planètes, nébuleuses violettes. Hors palette du brief (noir, blanc, orange signal) et hors du ton « ambitieux mais rigoureux ». |
| 19 | [SpaceX Redesign UI/UX](https://www.behance.net/gallery/94175367/SpaceX-Redesign-UI-UX) (Behance) | Pas de capture | **Non vérifié** : Behance renvoie une erreur 400 au navigateur automatisé. Remplacé par les captures mobiles de sites réels. |
| 20 | [Space Themed Landing Page (Roobinium)](https://dribbble.com/shots/21435075-Space-Themed-Landing-Page) (Dribbble) | [capture](captures/a-cote/20-dribbble-roobinium.jpg) | Contre-exemple : landing de jeu crypto et NFT (« Earn up to 167.75% APR »), trou noir à lueur orange, nébuleuses, glassmorphism. Contraire au ton et à la règle « chaque chiffre daté et sourcé ». Il montre que noir, orange et espace sont aussi le code de la crypto : l'orange de Strate Orbital reste plat, sans halo. |
| mobile | Pasqal sur mobile (n° 6) | [mobile](captures/a-cote/mobile-pasqal.jpg) | Contre-exemple mobile : titre de 44 px en graisse 100 sur photo (8 lignes, peu lisible), chiffres en carrousel coupé au bord, bandeau vert collé aux bords. Contraire aux contrastes vérifiés et à la lisibilité demandés par le brief (WCAG 2.2 AA). |
| mobile | constellr, carte sur mobile (n° 10) | [carte](captures/a-cote/mobile-constellr-carte.jpg) | Contre-exemple mobile : la légende de −8 à +8 °C arrive deux écrans sous les cartes, et la page déborde de 24 px (414 px pour 390). Contraire à la « légende accessible » du bloc Données. |

---

## Galeries : requêtes lancées

| Date | Galerie | Requête ou page | Résultat |
|---|---|---|---|
| 2026-11-12 | Behance | galeries des n° 3 et 19 | Erreur 400 au navigateur automatisé. Non réessayé. |
| 2026-11-12 | Lapa Ninja | fiche Cowboy Space (n° 4) | Bloqué par Cloudflare. Site réel vu à la place. |
| 2026-11-12 | Land-book | fiche SkyFi (n° 13) | Bloqué par Cloudflare. Site réel vu à la place. |
| 2026-11-12 | Pinterest | idées « space-themed website inspiration » et « space UI design » (n° 17 et 18) | Mur de connexion. Dribbble vu à la place. |
| 2026-11-12 | Dribbble | recherche « space website » | Capture n° 17 (contre-exemple). |
| 2026-11-12 (refonte) | Dribbble | recherche « roadmap timeline status » | Résultats affichés. Retenu : « Daily UI Component #4: Timeline Status » (n° 22). |
| 2026-11-12 (refonte) | Dribbble | recherche « contact form inquiry type » | Page « Let's confirm you are human » (HTTP 405). Arrêté, sans contourner. |
| 2026-11-12 (refonte) | Awwwards | recherche « contact form », puis catégorie d'éléments [Forms](https://www.awwwards.com/inspiration/forms) | Vus : « Built By Silo - Contact form » (deux étapes sur noir, mais libellés en placeholder seulement, écarté pour l'accessibilité) et « Contact Form » de fyne digital creative (retenu, n° 23). Aucun formulaire segmenté par type de demandeur trouvé. |
| 2026-11-12 (refonte) | Awwwards | page [Elements](https://www.awwwards.com/elements/), recherche d'un mur de logos avec la nature du soutien | Rien de pertinent dans les éléments listés. Bloc 6 laissé avec son manque. |
| 2026-11-13 | Unsplash | recherches « aerospace engineer » et « engineers laboratory » (photos d'équipe) | « Access Denied » dès la première page. Arrêté, sans contourner. |
| 2026-11-13 | Pexels | recherche « engineers laboratory » (photos d'équipe) | Vérification anti-robots de Cloudflare. Arrêté, sans contourner. Bloc 7 passé à « Qui sommes-nous » sans photo. |

---

## Arbitrages

- **Pause des animations** : on ajoute un bouton pause visible près de l'orbite, parce que `prefers-reduced-motion` ne suffit pas. Le critère WCAG 2.2.2 (niveau A) l'exige pour une animation de plus de 5 secondes affichée à côté d'autres contenus. Même règle pour la timeline si elle défile seule.
- **Distinction de la marque** : on garde le noir, le blanc, l'orange signal et IBM Plex Sans et Mono, et la différence passe par la grille, le mono et la carte, parce que la palette est déjà prise (n° 3, 4, 7 et 20). IBM Plex Sans Condensed n'est pas retenue : le brief s'en tient à Plex Sans et Plex Mono.
- **Carte de démonstration** : on construit la tuile sur le produit Surface Soil Moisture du Copernicus Land Monitoring Service (1 km de résolution en Europe, à partir de Sentinel-1 ; [CLMS, Soil Moisture](https://land.copernicus.eu/en/products/soil-moisture), vu le 2026-11-13), avec la source et la date écrites sur la carte. Une carte inventée passerait pour une mesure de Strate Orbital.
- **Courbe « une mesure, pas une estimation »** : on ne la trace que sur des données publiques, légendées comme telles. Sans paire de données publiques satellite et sondes, le bloc montre le format de la courbe, axes et légende, sans valeurs.
- **Publications** : l'onglet liste des publications réelles sur la GNSS-R, avec DOI, présentées comme lectures de référence du domaine et jamais comme travaux de l'entreprise. À produire en S2.
- **Jalons sans date** : les jalons de la timeline portent un numéro d'étape et un statut (réalisé, partiel, à venir), pas de date, parce qu'une date inventée se lirait comme un fait.
- **Soutiens** : des logotypes fictifs, avec la nature du soutien écrite en texte. Aucun logo d'institution réelle (Bpifrance, ESA, France 2030), parce que l'entreprise est fictive et n'a aucun soutien réel.
- **Photos d'équipe** : un bloc « Qui sommes-nous » court, sans photo, parce qu'Unsplash et Pexels ont bloqué le navigateur le 2026-11-13 (voir bloc 7).
