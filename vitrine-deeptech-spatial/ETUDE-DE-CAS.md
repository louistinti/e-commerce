# Étude de cas : site vitrine deeptech / spatial

> Document de travail de l'agence. **Strate Orbital est une entreprise fictive.** Les entreprises analysées sont réelles. La première version a été écrite sans pouvoir ouvrir leurs sites (réseau de la session bloqué). Les pages ont ensuite été ouvertes et capturées le 2026-11-12 pour le [bench](BENCH.md) : les affirmations que cette vérification contredit sont corrigées ici. Les chiffres de marché ont été rouverts le 2026-11-13 : ceux dont la source ne répond plus sont retirés. Voir les notes de méthode en fin de document.

## Executive summary

Le spatial européen lève gros en 2026 : 1,6 Md€ en fonds propres et 1,3 Md€ de dette au premier semestre, avec la France en tête (Tech.eu, vu le 2026-11-13). Les jeunes deeptechs doivent donc se distinguer face à des concurrents très bien dotés. Les 6 sites étudiés partagent les mêmes codes : mode sombre, chiffres orbitaux, fil d'actualités comme preuve. En revanche, très peu montrent ce que la technologie *produit* (la donnée) ou parlent au niveau technique sans quitter la home. Pour Strate Orbital, l'opportunité est un site « carte d'abord » : la donnée d'humidité comme héroïne, une explication à 3 niveaux, une timeline honnête et un ton rigoureux mais civil, à rebours de la dérive défense du secteur.

## 1. Le marché en 5 lignes

- **Les montants montent en 2026** : au S1 2026, 30 entreprises spatiales européennes ont levé 1,6 Md€ en fonds propres (+543,7 % sur un an), plus 1,3 Md€ de dette, et la France est en tête. Sur toute l'année 2025 : 859 M€ en fonds propres et 197 M€ de dette, sur 54 tours ([Tech.eu Funding Explorer, S1 2026](https://funding.tech.eu/sectors/space/2026/h1), [2025](https://funding.tech.eu/sectors/space/2025), données au 12 novembre 2026, vu le 2026-11-13).
- **Des tickets géants** : au S1 2026, Iceye a levé 450 M€ en série D+ (juin) et Isar Aerospace 270 M€ (juin), d'après le tableau des plus gros tours de la même page Tech.eu (vu le 2026-11-13).
- **La souveraineté tire l'observation de la Terre** : constellr (Allemagne, imagerie thermique) a levé 37 M€ en série A le 10 février 2026, pour du « defence grade thermal intelligence » ([constellr](https://www.constellr.com/article/constellr-secures-eu37-million-series-a-funding-to-deliver-defence-grade-thermal-intelligence), vu le 2026-11-13).
- **Les nanosatellites sont opérationnels** : Kinéis (essaimage du CNES) affiche 25 nanosatellites sur sa [page Technologie](https://kineis.com/en/technology-kineis-iot/) (lue le 2026-11-12 pour le bench, n° 5).
- **Des investisseurs de toute l'Europe** : au S1 2026, la France, la Finlande, l'Espagne et l'Allemagne mènent par montant levé (Tech.eu, même page). Le site doit donc convaincre en anglais autant qu'en français.

Les chiffres Tech.eu sont mis à jour en continu : chaque chiffre est cité avec la date de ses données.

## 2. Critique de 6 sites réels

Grille utilisée : première impression (2 s), usabilité, hiérarchie visuelle, accessibilité, ce qui marche, recommandations. « Non observé » signifie que l'information exige une visite visuelle qui n'a pas pu être faite. Les observations du bench (2026-11-12) sont signalées par leur numéro.

### 2.1 Kinéis (France), IoT par nanosatellites
- **URL** : https://kineis.com/en/technology-kineis-iot/
- **Positionnement** : opérateur européen d'IoT satellitaire. Le produit vendu est la connectivité, pas le satellite.
- **Première impression** : non observée. Le site a répondu par des erreurs 429 sur ses feuilles de style : le texte a été lu, la mise en page n'a pas été vue (bench, n° 5). D'après les titres de pages, le visiteur comprend vite l'objectif (« universal connectivity », « locate your assets 24/7 »).
- **Usabilité** : navigation par usage (`/solutions/iot-to-track/`), par secteur, et une FAQ dédiée. Le parcours d'achat B2B est lisible. Le CTA n'a pas été observé.
- **Hiérarchie** : la page Technologie est structurée autour de chiffres-clés : 25 nanosatellites, 650 km, 5 plans orbitaux, 20 stations sol, 80 passages par jour (bench, n° 5).
- **Accessibilité** : non observée.
- **Ce qui marche** :
  - Le fonctionnement expliqué en 4 étapes : objet, satellite, station sol, centre de service (bench, n° 5).
  - Une FAQ qui traite les objections.
- **Recommandations** :
  1. Rendre visibles le récit de mission et le recrutement, absents des résultats indexés.
  2. Rassembler les chiffres-clés dans un bloc unique sur la home.
  3. Écrire les limites du service : la page Technologie n'en assume aucune (bench, n° 5).

### 2.2 constellr (Allemagne), « thermal intelligence »
- **URL** : https://www.constellr.com/solutions ; microsite : https://urban-resilience.constellr.com/
- **Positionnement** : donnée thermique spatiale, de l'agriculture vers la défense. C'est l'analogue le plus proche de Strate Orbital.
- **Première impression** : la page Solutions s'ouvre sur « We close blind spots in intelligence ». Le titre de la page reste « Thermal Intelligence » : la catégorie est martelée (vu le 2026-11-13).
- **Usabilité** : la page Solutions présente des « missions » : le problème, ce que le thermique a révélé, l'enseignement stratégique. La sécurité nationale vient en premier (vu le 2026-11-13). L'étude de cas reste un microsite séparé : le contenu est éclaté entre plusieurs domaines.
- **Hiérarchie** : sur le microsite, le résultat chiffré est dans le titre, et la résolution, la précision et la revisite sont données près de la carte : 30 m, ±2 K, 8 jours (bench, n° 10).
- **Accessibilité** : légende de la carte collée à la carte sur desktop, mais deux écrans plus bas sur mobile, et un débordement horizontal à 390 px (bench, n° 10 et capture mobile).
- **Ce qui marche** :
  - Posséder une catégorie.
  - Le récit « problème, ce que la donnée révèle, décision ».
  - Montrer la donnée dans un microsite narratif.
- **Recommandations** :
  1. Réintégrer l'étude de cas sur le domaine principal.
  2. Séparer clairement les parcours civil et défense : la page Solutions met la défense en tête.

### 2.3 The Exploration Company (France et Allemagne), capsule Nyx
- **URL** : https://exploration.space (domaine des pages indexées, par exemple le [blog](https://exploration.space/blog/the-exploration-companys-nyx-earth-capsule-receives-phase-1-iss-safety-approval))
- **Positionnement** : capsule cargo réutilisable européenne.
- **Première impression** : non observée.
- **Usabilité** : une page programme (exploration.space/nyx selon Wikipédia) et un blog d'étapes datées. La navigation n'a pas été observée.
- **Hiérarchie** : les fiches mettent en avant la charge utile. La capsule Nyx doit apporter 2 600 kg de cargo vers l'ISS ([Wikipédia, The Exploration Company](https://fr.wikipedia.org/wiki/The_Exploration_Company), vu le 2026-11-13).
- **Accessibilité** : non observée.
- **Ce qui marche** : chaque jalon technique devient un billet daté, ce qui forme une timeline de preuves.
- **Recommandations** :
  1. Assumer les résultats partiels. Le démonstrateur Mission Possible, lancé le 24 juin 2025, a été déclaré « succès partiel » par l'entreprise (même page Wikipédia, qui cite European Spaceflight). Un site qui ne montre que les succès perd en crédibilité.
  2. Agréger les jalons dans une timeline visuelle sur la home.

### 2.4 EnduroSat (Bulgarie), plateformes nanosatellites
- **URL** : https://www.awwwards.com/sites/endurosat (mention honorable du 20 août 2024)
- **Positionnement** : des satellites configurables, en « space as a service ».
- **Première impression** : fond sombre, une grille de filets verticaux fins avec un chiffre par colonne (bench, n° 16). Ce n'est pas un site sans effets : la fiche Awwwards porte les tags Parallax, Video, 3D et Transitions.
- **Usabilité** : un configurateur client qui transforme le catalogue en interaction, d'après les descriptions indexées (non vu). La fiche Awwwards crédite Kreativa Studio.
- **Hiérarchie** : des chiffres en petites capitales, un par colonne : 450+ années d'expérience cumulée, 230+ clients, 150+ personnes (bench, n° 16).
- **Accessibilité** : non observée. Le mode sombre est à mesurer (gris sur noir).
- **Ce qui marche** : une interaction qui *fait comprendre* le produit, saluée par un prix.
- **Recommandations** :
  1. Pour une boîte en amorçage, remplacer le configurateur par une carte de données : même effet, coût bien moindre.
  2. Prévoir une alternative non interactive pour le configurateur (accessibilité).

### 2.5 Anduril (États-Unis), défense : référence internationale
- **URL** : https://www.anduril.com/, et la fiche [Fonts In Use](https://fontsinuse.com/uses/32662/anduril-industries) (avril 2020) ; voir aussi [UI UX Showcase](https://uiuxshowcase.com/industrial-design/anduril-defence-technology/)
- **Positionnement** : une entreprise de défense « logicielle » (Lattice), avec des produits air, mer et terre.
- **Première impression** : le site de 2026 est sur fond noir, et son hero n'a aucun texte au-dessus de la ligne de flottaison (bench, n° 15). L'œil va aux images produit.
- **Usabilité** : navigation par domaine (air, mer, terre, logiciel). Non observée en détail.
- **Hiérarchie** : la fiche Fonts In Use montre un site blanc en Helvetica Now, qui n'existe plus. La couleur vient des images.
- **Accessibilité** : non mesurée. Un hero sans texte échoue au critère « comprendre la mission en 30 s » du brief.
- **Ce qui marche** : la retenue, une voix unique et une image de très haut niveau.
- **Recommandations pour notre usage** :
  1. Reprendre la discipline (un accent, peu d'effets) sans le registre martial.
  2. Ne pas reprendre le hero sans texte.
  3. Ne pas copier sans les moyens visuels équivalents.

### 2.6 Turion Space (États-Unis), refonte par WILD : référence internationale
- **URL** : https://wild.as/work/turion-space ; [Fast Company](https://www.fastcompany.com/91614321/turion-space-rebrand)
- **Positionnement** : surveillance de l'espace et vaisseaux orbitaux.
- **Première impression** : sur l'étude de cas de WILD, fond noir et petites mentions en capitales mono autour du visuel (bench, n° 1). BUCK signe l'identité et les rendus 3D, pas des photos.
- **Usabilité** : site Framer sur mesure. L'étude de cas ne parle pas de parallaxe (bench, n° 1).
- **Hiérarchie** : les rendus 3D et le système de marque d'abord, puis le texte.
- **Accessibilité** : le récit au défilement doit respecter `prefers-reduced-motion`. Non vérifié.
- **Ce qui marche** : la cohérence de la marque et la maintenabilité (Framer).
- **Recommandations** :
  1. Prévoir un raccourci « l'essentiel en 30 s » pour les visiteurs pressés.
  2. Proposer une ancre directe vers les chiffres.

Consultés en surface, sans critique : Unseenlabs (https://unseenlabs.space/technology), Pasqal (https://www.pasqal.com/ et https://docs.pasqal.com/), Aura Aero (https://www.aura-aero.com/en), Planet ([annonce de refonte de marque](https://www.planet.com/pulse/?p=2185)).

## 3. Thèmes clés

### T1 : Le chiffre technique comme preuve principale
- **Prévalence** : 5 sites sur 6 (sauf Anduril, qui mise sur l'image).
- **Observations** :
  - Kinéis : 25 nanosatellites, 650 km, 20 stations sol.
  - constellr : 30 m, ±2 K, 8 jours (microsite).
  - TEC : 2 600 kg de cargo vers l'ISS.
  - EnduroSat : une grille de chiffres (450+, 230+, 150+).
  - Turion : présence de jalons techniques, d'après la presse.
- **Interprétation** : le public (investisseurs techniques, ingénieurs) juge sur des chiffres vérifiables. Les chiffres sans date ni source sont un signal négatif.

### T2 : Le fil d'actualités sert de timeline
- **Prévalence** : 3 sur 6 (Kinéis, constellr, TEC), plus Unseenlabs parmi les sites consultés en surface.
- **Observations** : lancements, partenariats et levées publiés comme articles datés. Aucun des sites consultés ne les agrège dans une frise sur la home (d'après les pages indexées).
- **Interprétation** : la preuve existe mais elle est dispersée. Une timeline visuelle est un manque à combler.

### T3 : La donnée produite est rarement montrée
- **Prévalence** : 1 sur 6 la montre vraiment (constellr, et seulement dans un microsite).
- **Observations** : les autres sites montrent le véhicule (satellite, capsule) plutôt que ce qu'il produit.
- **Interprétation** : pour un acheteur public, « voir la carte » vaut plus que « voir le satellite ». C'est l'opportunité principale de Strate Orbital.

### T4 : Le glissement vers la défense
- **Prévalence** : 3 sur 6 (constellr, Anduril, Turion), plus Unseenlabs et Helsing dans le paysage.
- **Observations** : la levée de constellr est explicitement « defence grade », et sa page Solutions ouvre sur la sécurité nationale (vu le 2026-11-13). Le ton noir, sobre et martial est devenu la norme.
- **Interprétation** : une mission civile (eau, agriculture) peut se démarquer en gardant la rigueur sans la posture militaire.

### T5 : L'ambition visuelle repose sur des moyens lourds
- **Prévalence** : 3 sur 6 (EnduroSat avec un configurateur, de la vidéo et de la 3D ; Turion avec les rendus 3D de BUCK ; Anduril avec un studio interne).
- **Interprétation** : ces codes ne se copient pas avec un budget d'amorçage. Il faut un seul élément « signature » bon marché (une carte, un SVG).

## 4. Insights → Opportunités

| Insight | Opportunité | Impact | Effort |
|---|---|---|---|
| La donnée produite est presque jamais montrée sur la home | Section « Données » avec une carte d'exemple et un curseur temporel, sans 3D | H | M |
| Les jalons sont dispersés dans le blog | Timeline en home avec des statuts réalisé / partiel / à venir, éditable dans le CMS | H | B |
| Les décideurs et les ingénieurs n'ont pas les mêmes besoins (site d'un côté, documentation de l'autre, comme chez Pasqal) | Explication à 3 niveaux en onglets, avec les publications en DOI | H | B |
| Le ton défense domine | Positionnement civil assumé, rigueur graphique sans registre martial | M | B |
| Les codes visuels premium exigent de gros moyens | Un seul visuel SVG animé, léger, et une typo Plex en signature | M | B |
| Les échecs partiels sont relayés par la presse | Une timeline qui assume un statut « partiel » avec sa cause | M | B |
| Le recrutement est souvent externalisé ou invisible | 3 offres visibles sur la home, avec le problème technique à résoudre | M | B |
| Les investisseurs viennent de toute l'Europe | FR et EN complets dès le lancement, avec hreflang | H | M |

## 5. Erreurs à éviter

- La 3D WebGL lourde qui fait ramer le mobile et masque le message.
- Les vues d'artiste présentées comme des photos (il faut toujours légender).
- Des chiffres sans date ni source.
- Des logos de financeurs sans la nature du soutien, ou des logos d'institutions réelles sur un site de démonstration.
- Des spécifications de charge utile qui pourraient relever du contrôle export des biens à double usage.
- Le cliché Dribbble (nébuleuses, néon, glassmorphism).
- L'orange signal pour du texte courant sur fond clair (3,1:1 sur blanc, calculé dans le bench, quand WCAG demande 4,5:1).

## 6. Conclusion pour Strate Orbital (fictif)

- **Angle** : « la donnée d'humidité des sols, vue de l'espace, pour décider sur le terrain ». Le héros est la carte.
- **Le README est pertinent.** Ajustements retenus :
  - Section 5 : une carte interactive légère, construite sur des données publiques Copernicus citées sur la carte.
  - Section 4 : des statuts explicites.
  - Section 2 : des onglets avec DOI.
  - Section 6 : la nature exacte de chaque soutien, sur des logotypes fictifs.
  - Section 7 : un bloc « Qui sommes-nous » court, sans photo.
- **Ton** : la rigueur d'Anduril et Turion, mais un usage civil. Le noir et l'orange signal sont dosés.
- **Bilingue FR/EN dès le lancement.**
- **Budget** : Webflow, Framer ou Astro, sans configurateur ni WebGL. L'investissement signature est la carte.

## 7. Questions à tester en recherche utilisateur

1. Un investisseur comprend-il en 5 secondes ce que fait Strate Orbital à partir du hero seul ?
2. Quelle preuve pèse le plus pour un acheteur public : une publication, une image en orbite, une référence client ou un financeur public ?
3. Le niveau « En bref » est-il compris sans jargon par un agronome ou un gestionnaire de l'eau ?
4. La carte d'exemple est-elle lue correctement (légende, échelle, date) sur mobile ?
5. Afficher un jalon « partiel » renforce-t-il ou affaiblit-il la confiance ?
6. Le mode sombre gêne-t-il la lecture longue (onglet technique, publications) ?
7. Un ingénieur postule-t-il depuis la home, ou cherche-t-il d'abord une page carrière complète ?

## 8. Notes de méthode

- **Sources** :
  - Environ 45 recherches web (partagées entre les deux catégories) (novembre 2026).
  - Pages officielles indexées (kineis.com, constellr.com, exploration.space, pasqal.com, aura-aero.com, helsing.ai).
  - Fiches Awwwards, Fonts In Use et UI UX Showcase.
  - Presse (Fast Company), Wikipédia et l'agrégateur de levées Tech.eu Funding Explorer.
- **Vérifications** :
  - 2026-11-12 : sites ouverts et capturés dans un vrai navigateur pour le [bench](BENCH.md). Les rubriques de ce document que le bench contredisait sont corrigées (Kinéis, constellr, EnduroSat, Anduril, Turion).
  - 2026-11-13 : chiffres de marché rouverts. Tech.eu a mis à jour ses montants (le total du S1 2026 se lit désormais 1,6 Md€ en fonds propres plus 1,3 Md€ de dette) ; la levée de constellr est confirmée ; la charge utile de Nyx et le « succès partiel » de Mission Possible viennent de Wikipédia.
- **Retirés faute de source qui répond le 2026-11-13** : la levée de 450 M$ de The Exploration Company (l'article de Techniques de l'Ingénieur redirige vers la liste des brèves), les 300 M€ d'Open Cosmos (page 24matins introuvable), le « depuis juin 2025 » et les « 20 000 objets actifs » de Kinéis (erreur 429), la domination des investisseurs américains (pulse.bot injoignable), le 1,4 Md€ « d'une autre source » (aucune source citée), les dimensions de Nyx, le « 10 m affiné » et la « première image de Tokyo » de constellr (absents de la page Solutions actuelle), le « 60fps » d'EnduroSat (absent de la fiche Awwwards).
- **Limites** :
  - Les rubriques « non observé » restent des déductions : Kinéis n'a pas pu être vu en page, ni les sites de TEC et EnduroSat en direct.
  - Les chiffres d'entreprise sont auto-déclarés (pages officielles, communiqués).
  - Strate Orbital est un nom de démonstration, non déposé.
