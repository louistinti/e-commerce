# Benchmark visuel : Strate Orbital (entreprise fictive)

## Limites, à lire en premier

Mise à jour du 2026-11-12, faite avec un vrai navigateur (Chrome piloté par Playwright).

- **Ce qui a été vu** : 14 des 20 références d'origine ont été ouvertes à leur adresse, et 13 capturées (Kinéis, n° 5, a été lue sans pouvoir être capturée). 5 autres, bloquées, ont été remplacées par une page équivalente ouverte et capturée (le site réel ou une page Dribbble : n° 3, 4, 13, 17 et 18). Une seule reste sans équivalent direct (n° 19, Behance), remplacée par 4 captures mobiles de 3 sites réels. Une référence a été ajoutée et capturée (n° 21). Les captures sont en 1440 × 900 px, au-dessus de la ligne de flottaison, dans [`captures/`](captures/). Les fichiers en `NNb` sont une seconde capture ciblée sur un élément clé plus bas. Les couleurs et les polices citées ont été relevées dans la page (`getComputedStyle`) ou dans la fiche Awwwards et Dribbble, pas devinées. Les chiffres cités sont ceux affichés le 2026-11-12.
- **Bloqué, et pourquoi** :
  - Behance (n° 3 et 19) renvoie une erreur 400 au navigateur automatisé.
  - Lapa Ninja (n° 4) et Land-book (n° 13) bloquent par Cloudflare.
  - Pinterest (n° 17 et 18) affiche un mur de connexion. Les vignettes sont à moitié visibles derrière, mais aucune capture n'a été faite (c'est une page de connexion).
  - L'article Fast Company cité au n° 1 s'affiche vide pour le navigateur automatisé.
  - Kinéis (n° 5) a répondu par des erreurs 429 (trop de requêtes) sur toutes ses feuilles de style pendant toute la session : le texte a été lu, mais la mise en page n'a pas pu être vue. Pas de capture.
- **Corrections importantes** :
  - Kinéis (n° 5) : la phrase « pas de gros flux » n'est pas sur la page. Les chiffres sont confirmés, avec 20 stations sol (et non « environ 20 »).
  - EnduroSat (n° 16) : ce n'est pas un site « sans effets ». La fiche Awwwards porte les tags Parallax, Video, 3D et Transitions. Les tags cités venaient d'Awwwards, pas de Dribbble.
  - Cowboy Space (n° 4) : la palette n'est pas noire mais brun très sombre, avec un bouton orange. La phrase « Earth's energy grid can't run at the pace of AI » est dans le paragraphe sous le titre, pas dans le hero.
  - Turion (n° 1) : l'étude de cas ne parle pas de parallaxe. BUCK a fourni l'identité et des rendus 3D, pas des photos.
  - Anduril (n° 15) : la fiche Fonts In Use date d'avril 2020 et montre un site sur fond blanc. Le site de 2026 est sur fond noir.
  - Roobinium (n° 20) : c'est une landing de jeu crypto et NFT, pas un site spatial. Le contre-exemple tient, et il est plus fort qu'annoncé.
  - Shakuro (n° 2) : le shot est signé Conceptzilla seul.
- **URL mortes ou redirigées** : le site primé NASA Spacecrafts (n° 8) n'existe plus, le domaine redirige vers une page de parking. Toutes les autres URL d'origine répondent.
- **Bannières cookies** : refusées partout où un refus existait (« I decline », « Reject All », « Refuser », « No, thanks », « Reject »).
- **Données personnelles** : avatars floutés sur les pages Dribbble et Awwwards. Sur le n° 20, l'e-mail et le téléphone affichés ont été masqués avant la capture.

---

**Méthode d'origine.** Les URL viennent de résultats de recherche web (novembre 2026), sans ouverture des pages. Toutes les mentions « d'après la description » ont été remplacées par ce qui a été vu, ou marquées « non vérifié ».

Répartition après vérification : sites réels 8 (dont 3 qui remplacent une galerie bloquée) · Awwwards 4 · Dribbble 7 (dont 2 qui remplacent Pinterest) · Fonts In Use 1 · non vérifiées sans remplacement direct 1 (Behance). **Total : 21 références**, plus 4 captures mobiles.

---

## Hero

| # | Référence | URL | Source | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 1 | Turion Space, refonte par WILD | https://wild.as/work/turion-space | Site réel (étude de cas d'agence) | [capture](captures/01-turion-wild.jpg) | L'étude de cas montre le hero de Turion dans un ordinateur : fond noir, horizon violet, satellite en rendu 3D, titre « Unleashing humanity's galactic potential », petites mentions en capitales mono (« ORBIT WITH PURPOSE », « 001 »). Le texte confirme un site Framer, construit sur l'identité et les rendus 3D de BUCK (crédit « Branding & Photography »). **Correction** : la page ne parle pas de parallaxe, et les visuels sont des rendus, pas des photos. L'article Fast Company cité n'a pas pu être lu (page vide, non vérifié). **À reprendre** : les mentions courtes en mono autour du visuel. **À éviter** : le dégradé violet de l'horizon, qui rejoint le cliché du n° 17. |
| 2 | Satellite Landing Page Animation (Conceptzilla) | https://dribbble.com/shots/16467758-Satellite-Landing-Page-Animation | Dribbble | [capture](captures/02-dribbble-satellite.jpg) | Fond noir `#010101`, un CubeSat en 3D à droite, titre « What are CubeSats » en grotesque blanche, une phrase de définition (« moins de 10 kilogrammes »), un bouton pastille bleu `#1B4AD0`. Le concept affiche le logo NASA dans l'en-tête. **Correction** : le shot est signé Conceptzilla seul, pas Shakuro. **À reprendre** : un seul objet sur fond noir, et un titre qui répond à une question simple. **À éviter** : emprunter le logo d'une agence spatiale, ce que le brief interdit. |
| 3 | Spaceflux | Behance d'origine non vérifié (erreur 400) : https://www.behance.net/gallery/183406451/Spaceflux-Website-and-UIUX-for-Space-Company. Vu à la place : https://spaceflux.io/ | Site réel (UK) | [capture](captures/03-spaceflux.jpg) | Le motif d'œil est bien là : des traînées d'orbites violettes forment un œil autour de la Terre. Fond `#100919`, titre « Space Intelligence » en **IBM Plex Sans** 80 px, graisse 400, couleur `#F5EEFF`. Sous-titre en capitales (NB Architekt) `#C09EFF`, et des coordonnées GPS en 10 px en haut à gauche. Plus bas, 3 cartes avec des chiffres précis : données livrées « en 90 secondes », objets suivis « jusqu'à 10 cm » en orbite géostationnaire, 2,5 cm en orbite basse. **Non vérifié** : la réaction de l'œil au défilement (c'est une image, sans canvas ni vidéo). **À reprendre** : les coordonnées en petit corps, les chiffres avec leur unité. **À noter** : un acteur spatial utilise déjà IBM Plex Sans en titre. |
| 4 | Cowboy Space | Lapa Ninja d'origine non vérifié (Cloudflare) : https://www.lapa.ninja/post/cowboyspace/. Vu à la place : https://www.cowboyspace.com/ | Site réel (US) | [capture](captures/04-cowboy-space.jpg) | Hero vidéo plein écran (satellite au-dessus d'un désert), logo en Panell Wide Bold, carte « BIG IRON EXPRESS » avec un champ e-mail et un bouton orange `#F47D49` à texte sombre `#17191C` (6,6:1). Le titre est « POWERING HUMANITY FROM THE HIGH FRONTIER » en Panell Wide Bold, texte `#EBE6E0` sur brun très sombre `#1F1509`. **Correction** : la phrase « Earth's energy grid can't run at the pace of AI. We can. » conclut le paragraphe sous ce titre. Elle n'est pas la promesse du hero. **À reprendre** : la structure « problème terrestre, puis réponse spatiale », à placer cette fois dans le sous-titre. **À noter** : le bouton orange à texte sombre est exactement notre token `brand.accent`, ce qui confirme qu'il fonctionne, mais aussi qu'il n'est pas distinctif seul. |

## Explication technologique

| # | Référence | URL | Source | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 5 | Kinéis, page Technologie | https://kineis.com/en/technology-kineis-iot/ | Site réel (FR) | Pas de capture : erreurs 429 sur toutes les feuilles de style | Texte lu, mise en page non vue. Chiffres confirmés : 25 nanosatellites, 650 km, 5 plans orbitaux de 5 satellites, **20 stations sol** (et non « environ 20 »). D'autres chiffres sont là : 1,40 × 1,60 m, 28 kg, 7,8 km/s, 80 passages par jour au-dessus de chaque point, et une accroche « seulement 15 % de la planète est couverte par les réseaux terrestres ». Le fonctionnement est raconté en 4 étapes (objet, satellite, station sol, centre de service 24 h/24). La page renvoie vers une base de connaissances « pour les ingénieurs ». **Correction** : la phrase « pas de gros flux » n'est pas sur la page, aucune limite n'y est assumée. **À reprendre** : les chiffres avec unité, et le récit en 4 étapes pour l'onglet « En bref ». Les limites restent à écrire nous-mêmes. |
| 6 | Pasqal, site et documentation séparés | https://www.pasqal.com/ (documentation : https://docs.pasqal.com/) | Site réel (FR) | [capture](captures/06-pasqal.jpg) | Hero photo sombre (salle de machines), titre en Grotesk 55 px **graisse 100**, blanc. Bouton vert `#00C887` à texte blanc : 2,2:1, sous le seuil AA. En-tête blanc, texte et bouton « Contact » en `#0F1E23`. Sous le hero, sur une bande sombre, 4 chiffres : 85 brevets, 70 docteurs, 1 000+ atomes, 25 clients. La séparation est confirmée : le menu mène à « Pasqal Documentation » (docs.pasqal.com), qui reprend le vert et propose un sélecteur de thème sombre, clair ou automatique. **À reprendre** : la documentation séparée, en onglets chez nous, et la bascule de thème. **À éviter** : un titre en graisse 100 sur photo, et du blanc sur un vert clair. |
| 7 | Artificial Satellite / Earth Observation Service (FAVE®) | https://www.awwwards.com/sites/artificial-satellite (élément : https://www.awwwards.com/inspiration/earth-observation-service-artificial-satellite) | Awwwards, mention honorable du 24 août 2023 | [capture](captures/07-awwwards-artificial-satellite.jpg), [élément](captures/07b-awwwards-earth-observation.jpg) | Site satellite de Hanwha Space Hub (le bouton « Visit Site » y mène, le site répond toujours, fond noir). Palette déclarée : `#000000` et `#F77D16` (7,9:1 sur noir). L'élément « Earth Observation Service » montre la Terre dans une orbite au trait, un **réticule orange fin** et des crochets de cadrage orange. Les éléments listés confirment des modules distincts : caméra EO/IR, antenne à balayage électronique, liaison inter-satellites, petit satellite SAR. **À reprendre** : le réticule et les crochets en trait fin pour la carte, et un module par sous-système pour le schéma éclaté. |

## Timeline

| # | Référence | URL | Source | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 8 | NASA Spacecrafts (Yanlin Ma) | https://www.awwwards.com/sites/nasa-spacecrafts | Awwwards, site du jour du 11 juin 2018 | [capture](captures/08-awwwards-nasa-spacecrafts.jpg), [timeline](captures/08b-awwwards-nasa-timeline.jpg) | Expérience WebGL (Three.js, D3) : des engins de 1960 à 2025 sur une grille, avec deux modes, « Date Sorting » et « Image Sorting ». L'élément « Chronologic Satellite Timeline » montre un **axe vertical des années** (1970 à 2025) avec un point par lancement, et l'engin choisi au centre. Palette `#000`, `#49C5B6`, `#FFFFFF`. **URL morte** : le site lui-même (nasaspacecraft.com) redirige vers une page de parking. **À reprendre** : l'axe vertical des années avec un point par jalon, très lisible sur mobile. **À éviter** : le WebGL. |
| 9 | Roadmap timeline (Anastasia Dvorzhanska) | https://dribbble.com/shots/4258663-Roadmap-timeline | Dribbble | [capture](captures/09-dribbble-roadmap.jpg) | Timeline verticale confirmée : une ligne blanche sinueuse, un nœud par jalon, la date en capitales vertes (« JUN 2017 », « JAN 2018 »), puis une ou deux lignes de texte. Cartes ardoise `#264441` sur un dégradé vert, accent `#2C9953`. Tous les nœuds sont identiques : rien ne distingue un jalon passé d'un jalon à venir. **À reprendre** : date en capitales, puis une ligne. **À ajouter** : nos pastilles de statut (réalisé, partiel, à venir) avec libellé. |

## Données

| # | Référence | URL | Source | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 10 | constellr, Dhun Climate Resilience Study | https://urban-resilience.constellr.com/ | Site réel (microsite de données) | [capture](captures/10-constellr-dhun.jpg), [carte](captures/10b-constellr-carte.jpg) | **Microsite en mode clair** : fond `#F8FAFC`, titre 72 px graisse 500 (SF Pro Display, puis Inter) avec le résultat dans le titre, « 8°C Temperature Reduction », en dégradé bleu. Bouton `#1476B8` à texte blanc (4,9:1). Le récit suit bien « une question, une réponse » : 3 chiffres (−8 °C à Dhun, −2,5 °C autour, +0,2 °C à Jaipur), une courbe 2015 à 2024, deux cartes thermiques côte à côte avec la zone hachurée, une légende divergente de −8 °C à +8 °C (bleu vers orange-rouge), puis 4 cartes d'explication. La section technique donne 30 m, ±2 K, 8 jours. **À reprendre** : le résultat chiffré dans le titre, la légende sous la carte, une carte d'explication par motif visible. **À noter** : l'orange y signifie « réchauffement ». Sur notre carte d'humidité, l'orange de marque ne doit jamais entrer dans l'échelle. |
| 11 | EarthEye, Agriculture Dashboard (Shakuro) | https://dribbble.com/shots/24596768-EarthEye-Agriculture-Dashboard-Design | Dribbble | [capture](captures/11-dribbble-eartheye.jpg), [tableau de bord](captures/11b-dribbble-eartheye-dashboard.jpg) | Le premier visuel est un widget mobile (« Water, Dangerous Level, 98.4 % »). Le tableau de bord est plus bas : colonne gauche avec les parcelles et leurs mesures (sol 16,7 %, eau 92,2 %…), puis des barres d'état par zone en vert, jaune et rouge ; carte satellite au centre avec les parcelles détourées ; à droite, un panneau « Map Layers & Data » (NDVI, EVI, NDRE…) et un sélecteur de dates. **Détail utile** : la source et la période sont écrites sur la carte (« Sentinel-hub 2024-11-04/2024-11-17 »). **À reprendre** : la source et la date sur la carte, le panneau de calques repliable. **À éviter** : l'état codé seulement par vert, jaune et rouge. |
| 12 | Land Lines (Google Data Arts Team, avec Zach Lieberman) | https://www.awwwards.com/sites/land-lines | Awwwards, site du jour du 10 janvier 2017 | [capture](captures/12-awwwards-land-lines.jpg) | Image satellite plein cadre de pivots d'irrigation (cercles verts), titre « LAND LINES » et deux boutons au trait, « Draw » et « Drag ». Palette `#000`, `#2779A7`, `#987654`. Le site répond toujours (lines.chromeexperiments.com). **À reprendre** : le glisser au doigt pour le curseur temporel sur mobile, et les pivots d'irrigation comme image d'ambiance, très parlants pour l'agriculture. |
| 13 | SkyFi, imagerie satellite commerciale | Land-book d'origine non vérifié (Cloudflare) : https://land-book.com/websites/38292-commercial-high-resolution-satellite-imagery-and-video-skyfi. Vu à la place : https://skyfi.com/ | Site réel (US) | [capture](captures/13-skyfi.jpg) | Fond noir, titre « Earth Intelligence Platform » en Hanken Grotesk 85 px graisse 300, posé sur une image satellite ronde avec des cadres de détection jaunes. Coordonnées et boutons en **DM Mono** 13 à 14 px, crochets de cadrage au trait. Un seul accent, le jaune `#FCC219`, sur « ORDER NOW » (texte noir, 12,9:1). Plus bas : « Trusted by 10,000+ companies », « STARTING AT $5 », et l'accès « sans barrières commerciales ni contractuelles ». **À reprendre** : le mono pour les coordonnées et les libellés de boutons, un seul accent réservé à l'action principale. C'est la direction A déjà en ligne. |

## Recrutement

| # | Référence | URL | Source | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 14 | Aura Aero, page Carrière | https://www.aura-aero.com/en/carriere | Site réel (FR) | [capture](captures/14-aura-aero-carriere.jpg), [chiffres](captures/14b-aura-aero-chiffres.jpg) | Hero : toute l'équipe photographiée par drone sur la piste, autour de 3 avions, titre « Your next mission starts here. ». Bloc « in figures » sur marine : 250+ personnes, 36 ans d'âge moyen, index d'égalité 94/100 (2024), et les **4 implantations confirmées** (Toulouse, Bernay, Daytona Beach, Abu Dhabi). Chiffres en bleu `#0167FF` (3,6:1 sur la marine, valable en grand corps seulement). Le processus de recrutement est en 3 étapes (candidature, appel RH, entretien avec le manager). **À reprendre** : une vraie photo d'équipe, les implantations, le processus en 3 étapes. |

## Palette et typo

| # | Référence | URL | Source | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 15 | Anduril, d'après Fonts In Use | https://fontsinuse.com/uses/32662/anduril-industries (site actuel : https://www.anduril.com/) | Fonts In Use (avril 2020) et site réel | [capture](captures/15-fontsinuse-anduril.jpg), [site 2026](captures/15b-anduril-2026.jpg) | La fiche confirme Helvetica Now et une palette noir et blanc où la couleur ne vient que des produits. **Correction** : la fiche date d'avril 2020 et montre un site sur fond blanc. Le site de 2026 est un cadre noir `#000` avec une vidéo produit pleine largeur, menu en Helvetica Now Display blanc, aucun texte au-dessus de la ligne de flottaison. La discipline tient toujours : aucune couleur d'accent. **À reprendre** : un seul accent, rare. **À éviter** : un hero sans aucun texte, qui ne passerait pas le test des 30 secondes du brief. |
| 16 | EnduroSat (Kreativa Studio et RISE2 Studio) | https://www.awwwards.com/sites/endurosat | Awwwards, mention honorable du 20 août 2024 | [capture](captures/16-awwwards-endurosat.jpg) | Titre « MAKING SPACE UNIVERSALLY ACCESSIBLE » en capitales (Magnetik 108 px, graisse 600 sur le site en ligne), photo produit d'un satellite, et surtout une **grille de filets verticaux fins** avec un chiffre en petites capitales dans chaque colonne : 450+ années d'expérience cumulée, 230+ clients, 150+ personnes. Palette `#000000` et `#00A1FF` ; sur le site, le bouton bleu porte un texte noir (7,5:1). **Correction** : ce n'est pas un site « sans effets ». La fiche porte les tags Parallax, Video, 3D et Transitions, et le texte parle d'un site « immersif ». **À reprendre** : la grille de filets avec un chiffre par colonne, c'est la direction A. |
| 17 | Space-themed Website Inspiration | Pinterest d'origine non vérifié (mur de connexion) : https://www.pinterest.com/ideas/space-themed-website-inspiration/943348102916/. Vu à la place : https://dribbble.com/search/space-website | Dribbble (recherche « space website ») | [capture](captures/17-dribbble-recherche-space-website.jpg) | Derrière le mur Pinterest, on devine des vignettes violettes, des planètes et des nébuleuses, sans pouvoir les capturer. La recherche Dribbble donne le même tableau : astronautes, fusée sur Mars, planètes, Terre bleue, et du bruit (bureaux, coworking, un mème). Les noms des auteurs sont masqués sur la capture. **À éviter** : tout ce répertoire. Il sert de liste de ce qu'il ne faut pas faire. |
| 18 | Space UI Design | Pinterest d'origine non vérifié (mur de connexion) : https://www.pinterest.com/ideas/space-ui-design/904954707495/. Vu à la place : https://dribbble.com/shots/27534165-Orbita-Spacecraft-Mission-UI | Dribbble (Notionhive) | [capture](captures/18-dribbble-orbita-mission-ui.jpg) | Derrière le mur Pinterest : des panneaux HUD cyan et des planètes. Le shot Orbita montre les micro-éléments utiles : une fiche technique alignée à droite, libellé gris puis valeur blanche (équipage 12, longueur 42 m, orbite basse, 120 kW), des orbites au trait fin, une petite mention en capitales « TECHNICAL SPECIFICATIONS ». **À reprendre** : la fiche libellé-valeur en Plex Mono, les orbites au trait. **À éviter** : les valeurs en 8 px environ, illisibles, et le titre géant découpé par l'objet. |

## Mobile

| # | Référence | URL | Source | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 19 | SpaceX Redesign UI/UX | https://www.behance.net/gallery/94175367/SpaceX-Redesign-UI-UX | Behance | Non vérifié (erreur 400) | Non vérifié : Behance renvoie une erreur 400. La recommandation mobile s'appuie désormais sur les 4 captures de sites réels de la section « Observé sur mobile » ci-dessous. |

### Observé sur mobile (390 × 844 px)

| Site | Capture | Ce qu'on a vu |
|---|---|---|
| Spaceflux | [mobile](captures/mobile-spaceflux.jpg) | Le visuel passe au-dessus du titre et rétrécit, sans disparaître. Titre en Plex Sans 54 px sur deux lignes, sous-titre mono, puis deux paragraphes. Aucun bouton visible dans le premier écran. Pas de défilement horizontal. |
| Pasqal | [mobile](captures/mobile-pasqal.jpg) | Titre de 44 px en graisse 100 sur la photo : 8 lignes, peu lisible. Les 4 chiffres deviennent un carrousel horizontal coupé au bord (« 70 », puis « 1… »). Le bandeau vert colle aux bords de l'écran, sans marge. |
| constellr | [hero](captures/mobile-constellr.jpg), [carte](captures/mobile-constellr-carte.jpg) | Hero propre : titre 36 px, bouton pleine largeur. Les deux cartes thermiques s'empilent, mais la légende de −8 à +8 °C se retrouve deux écrans plus bas. La page déborde de 24 px en largeur (414 px pour 390). |

**Ce qu'on en retient pour Strate Orbital**
- **À reprendre** : le satellite SVG au-dessus du titre et plus petit, plutôt que supprimé (Spaceflux). Le bouton principal pleine largeur dans le premier écran (constellr).
- **À reprendre** : la légende collée sous chaque carte, pas en fin de section.
- **À éviter** : les chiffres en carrousel horizontal. Sur mobile, les chiffres-clés passent en grille de 2 colonnes, entièrement visibles.
- **À éviter** : une graisse fine sur photo. Le titre mobile reste en graisse 600, comme prévu dans les tokens.
- **À vérifier** : aucun débordement horizontal à 390 px, carte comprise.

## Contre-exemple

| # | Référence | URL | Source | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 20 | Space Themed Landing Page (Roobinium) | https://dribbble.com/shots/21435075-Space-Themed-Landing-Page | Dribbble | [capture](captures/20-dribbble-roobinium.jpg) | Fond noir, trou noir à disque d'accrétion orange, nébuleuse, planète rouge, boutons rouge-orangé. Le texte du shot parle de glassmorphism, de nébuleuses et de parallaxe. **Correction** : c'est une landing de jeu crypto et NFT (« BlackQuantum », « Earn up to 167.75% APR », tableau de collections NFT), pas un site spatial. Le contre-exemple est donc plus fort : noir, orange et espace sont aussi le code visuel de la crypto. **À éviter** : la lueur orange, les nébuleuses et tout ce qui ressemble à un rendement promis. L'orange de Strate Orbital reste plat, sans halo. |

## Référence ajoutée

| # | Référence | URL | Source | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 21 | Starcloud, site orienté investisseurs (Flexy LLC) | https://dribbble.com/shots/27116861-Building-an-Investor-Focused-Website-for-Starcloud | Dribbble | [capture](captures/21-dribbble-starcloud.jpg) | Startup de centres de données en orbite. Le texte du shot vise explicitement « investisseurs, partenaires et ingénieurs », nos trois personas. Hero sombre (`#06090F`) avec des filets verticaux, un bouton vidéo en pastille et, dès le premier écran, une ligne « Backed by » avec 4 logos (NFX, NVIDIA, Y Combinator, In-Q-Tel). Site fait sous Webflow. **À reprendre** : une preuve de soutien visible dès le hero, pour Claire (P1). **À éviter** : des logos sans la nature du soutien, ce que notre règle n° 3 interdit. |

---

## Synthèse du moodboard

**Ce que les observations changent.** La direction A est confirmée et précisée par quatre sites réels vus : Spaceflux (coordonnées en petit corps, IBM Plex Sans), SkyFi (DM Mono, crochets, un seul accent), EnduroSat (grille de filets avec un chiffre par colonne) et Hanwha Space Hub (réticule orange fin sur noir). Deux nuances s'ajoutent. D'abord, le noir et l'orange sont déjà pris : Cowboy Space utilise le même bouton orange à texte sombre, Hanwha la même paire, et la crypto aussi (n° 20). L'orange ne suffit donc pas à distinguer Strate Orbital : la grille, le mono et la carte doivent le faire. Ensuite, la seule étude de cas « par la donnée » vue (constellr) est en mode clair, ce qui renforce la direction B pour la section Données. La palette et les tokens ne changent pas : aucune observation ne justifie de toucher aux couleurs, et les contrastes annoncés ont été recalculés (voir plus bas).

**Direction A : « Instrument »** (recommandée)
- Noir mat, grille stricte de filets fins, chiffres en Plex Mono avec leur unité, comme sur un tableau de bord de vol (EnduroSat, SkyFi).
- Un seul satellite en SVG, en trait fin, avec réticule et crochets de cadrage (Hanwha).
- L'orange est réservé aux CTA et à l'état « en cours », toujours plat, sans halo.

**Direction B : « Carte d'abord »**
- Le hero est la carte d'humidité elle-même (tuile animée lentement), et le satellite passe au second plan.
- Plus proche de l'usage client (eau, agriculture), moins « spatial ».
- Exige de vraies données d'exemple dès le départ.
- Observé : constellr raconte sa donnée en mode clair, résultat chiffré dans le titre. Si la direction A est retenue, la section Données peut emprunter ce traitement (fond clair, légende sous la carte).

**Direction C : « Archive de mission »**
- Ton éditorial, grandes photos d'intégration et de lancement, timeline en colonne vertébrale.
- Fort pour le recrutement et la presse (la photo d'équipe d'Aura Aero le montre).
- Dépend d'une vraie production photo.

## Palette recommandée (mode sombre par défaut)

Inchangée. Contrastes recalculés le 2026-11-12 (WCAG 2.1) : les valeurs annoncées sont justes.

| Rôle | Hex | Note |
|---|---|---|
| Fond | `#0A0B0D` | noir profond |
| Surface (cartes) | `#14171B` | |
| Filets et grilles | `#2A2F36` | décoratif uniquement (1,5:1 sur le fond) |
| Texte principal | `#F4F4F1` | blanc cassé, 17,9:1 sur le fond |
| Texte secondaire | `#9AA0A6` | 7,5:1 sur le fond, 6,8:1 sur la surface |
| Accent orange signal | `#FF5A1F` | 6,3:1 sur `#0A0B0D` ; **jamais en texte courant sur fond blanc** (3,1:1) ni sur `#F4F4F1` (2,8:1) |
| Mode clair : fond | `#F4F4F1` | accent assombri en `#C2410C` pour le texte (4,7:1) |
| Échelle d'humidité (séquentielle, de sec à humide) | `#6B5A3E` `#8C8A5A` `#4F8F86` `#3C7FB0` `#9CCBEB` | distincte de l'accent ; à valider avec un simulateur de daltonisme |

Pour comparaison, relevé sur les sites vus : bouton orange de Cowboy Space `#F47D49` à texte `#17191C`, 6,6:1 ; orange `#F77D16` de Hanwha sur noir, 7,9:1 ; bouton vert de Pasqal à texte blanc, 2,2:1 (échec AA).

## Polices (Google Fonts)

- **IBM Plex Sans** : 400 et 500 pour le texte, 600 pour les titres.
- **IBM Plex Mono** : 400 et 500 pour les chiffres, coordonnées, dates et légendes de la carte.
- Option pour les titres d'affichage : **IBM Plex Sans Condensed** 600, afin de rester dans la même famille.
- Observé : Spaceflux, acteur spatial britannique, utilise déjà IBM Plex Sans en titre (80 px, graisse 400). Le choix reste valable, mais la Condensed 600 et la grille aideront à ne pas lui ressembler.

## 3 « à ne pas faire »

1. Pas de nébuleuses, de néon ni de glassmorphism : c'est le cliché Dribbble et Pinterest (n° 17), qui fait amateur auprès des ingénieurs, et c'est aussi le code de la crypto (n° 20).
2. Pas de 3D WebGL plein écran ni de défilement détourné qui bloque l'accès aux chiffres : un investisseur doit pouvoir sauter le récit. Pas non plus de hero sans texte (Anduril 2026).
3. Pas de vue d'artiste sans légende, ni de logo de partenaire sans la nature du soutien (Starcloud, n° 21).

---

## Design tokens

Le mode sombre est le mode par défaut. Les valeurs du mode clair sont entre parenthèses quand elles diffèrent.

### Couleurs

| Token | Hex | Usage |
|---|---|---|
| `color.brand.accent` | `#FF5A1F` (clair : `#C2410C`) | fond du CTA principal, état « en cours » de la timeline, curseur de la carte |
| `color.brand.accent-hover` | `#FF7440` (clair : `#9A3412`) | survol du CTA |
| `color.brand.on-accent` | `#0A0B0D` | texte sur fond orange (6,3:1 ; 7,3:1 au survol). En clair, texte `#F4F4F1` sur `#C2410C` (4,7:1) |
| `color.neutral.1000` | `#0A0B0D` | fond (clair : texte) |
| `color.neutral.900` | `#14171B` | surface des cartes |
| `color.neutral.700` | `#2A2F36` | filets, grilles |
| `color.neutral.400` | `#9AA0A6` | texte secondaire (7,5:1 sur le fond) |
| `color.neutral.50` | `#F4F4F1` | texte principal (clair : fond) |
| `color.semantic.success` | `#3FB950` | jalon « réalisé », envoi réussi |
| `color.semantic.warning` | `#D4A72C` | jalon « partiel », donnée provisoire |
| `color.semantic.error` | `#F85149` | erreur de formulaire, jalon « échec » |
| `color.focus` | `#7AB8FF` | anneau de focus (distinct de l'orange, 9,5:1 sur le fond) |
| `color.data.moisture.1` à `.5` | `#6B5A3E` `#8C8A5A` `#4F8F86` `#3C7FB0` `#9CCBEB` | échelle séquentielle, de sec à humide |

L'orange de marque et le rouge d'erreur sont proches. L'erreur porte donc toujours une icône et un libellé, et l'orange n'est jamais utilisé pour signaler un problème. Il n'entre pas non plus dans l'échelle de la carte : sur une carte satellite, l'orange se lit « chaud » ou « sec » (constellr, n° 10).

### Typographie

| Token | Police | Taille (desktop / mobile) | Graisse | Interlignage |
|---|---|---|---|---|
| `type.display` | IBM Plex Sans Condensed | 80 / 44 px | 600 | 1,0 |
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

### Composants clés

**Bouton primaire** (« Contacter l'équipe partenariats »)
- Fond `brand.accent`, texte `brand.on-accent`, IBM Plex Sans 500 en 16 px, hauteur 48 px, `radius.sm`. Pleine largeur sur mobile.
- États :
  - survol : `accent-hover` ;
  - focus : anneau `color.focus` de 2 px, décalé de 2 px ;
  - actif : luminosité −8 % ;
  - désactivé : `neutral.700` avec texte `neutral.400` et `aria-disabled` ;
  - chargement : libellé « Envoi… » et spinner.

**Bouton secondaire** (« Explorer la carte »)
- Contour de 1 px `neutral.50`, texte `neutral.50`.
- États :
  - survol : fond `neutral.900` ;
  - focus : identique au primaire ;
  - désactivé : contour `neutral.700`.

**Carte jalon (timeline)**
- Date en `type.overline`, titre en `type.h3`, une ligne de description.
- Pastille de statut (`radius.pill`) : réalisé, partiel ou à venir, toujours avec un libellé texte.
- Surface `neutral.900`, filet `neutral.700`.

**Formulaire de contact segmenté**
- Premier champ « Vous êtes » (investisseur, client, presse, candidat), qui adapte la suite.
- 5 champs maximum, libellés visibles, erreurs sous le champ avec une icône et `aria-describedby`.

### À faire / À ne pas faire

| À faire | À ne pas faire |
|---|---|
| Orange réservé au CTA et à l'état « en cours » | Orange pour les titres, les liens et les alertes en même temps |
| Chiffres en Plex Mono, avec leur unité et leur date | Chiffres arrondis sans date (« bientôt 100 satellites ») |
| Un seul visuel animé, léger (SVG) | Plusieurs scènes WebGL qui font chuter le Lighthouse mobile |
| Carte doublée d'un tableau de valeurs accessible, source et date écrites sur la carte | Carte seule, sans légende textuelle ni alternative |
| Vues d'artiste légendées « vue d'artiste » | Rendus 3D présentés comme des photos en orbite |
| Mode clair disponible et testé | Mode sombre imposé avec du gris `#666` sur du noir |
| Chiffres-clés en grille de 2 colonnes sur mobile | Chiffres en carrousel horizontal coupé au bord |
