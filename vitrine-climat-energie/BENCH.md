# Benchmark visuel : Sobra (climat / énergie, B2B tertiaire)

## Limites, à lire en premier

Mise à jour du 2026-11-12, faite avec un vrai navigateur (Chrome piloté par Playwright). La première version avait été écrite sans accès réseau, « d'après la description » des résultats de recherche.

- **Ce qui a été vu** : 17 des 22 références d'origine ont une capture. 15 ont été ouvertes à leur propre URL. Pour 2 autres, l'URL d'origine est bloquée et la capture vient d'une page équivalente : le site réel de carbonplan (n° 15) et les shots Dribbble du même projet Manatee Energy (n° 19). Les captures sont en 1440 × 900 px, au-dessus de la ligne de flottaison (plus une capture ciblée quand un élément clé est plus bas), dans [`captures/`](captures/). Les couleurs et les polices citées ont été relevées dans la page (`getComputedStyle`), pas devinées. Les chiffres cités sont ceux affichés le 2026-11-12.
- **Bloqué, non vérifié** :
  - Land-book (n° 4) et Lapa Ninja (n° 14, 15, 20) : challenge Cloudflare, non contourné.
  - Behance (n° 19) : erreur HTTP 400 renvoyée au navigateur automatisé.
  - Pinterest (n° 7, 21, 22) : mur de connexion. Aucune épingle individuelle n'était listée dans le bench, donc rien n'a pu être capturé.
  - Le site réel d'Energy Park (n° 20) : certificat HTTPS invalide (`ERR_CERT_COMMON_NAME_INVALID`), avertissement non contourné. Seule la fiche Awwwards a été vue.
  - Ubigreen (n° 17) : le site renvoie des erreurs 429 sur ses feuilles de style. La page s'affiche sans mise en forme, malgré plusieurs essais espacés. Le texte est lisible et cité, mais la capture ne montre pas le vrai design.
- **URL mortes** : eTactica (n° 14) n'a plus de site, `etactica.com` redirige vers une page de nom de domaine à vendre.
- **Corrections importantes** :
  - BrainBox AI (n° 1) : le H1 est « AI Control », pas le chiffre. Les chiffres sont dans des cartes plus bas, avec « up to ».
  - Deepki (n° 5) : l'IPMVP n'est pas mentionné sur la page d'accueil.
  - Le tag Dribbble « impact » (n° 6) est rempli de logos, pas de sections « Our impact ». Le shot Cambium Impact, lui, est pertinent.
  - Fuselab (n° 11) n'est pas une carte comparative de sites : c'est une ville 3D de nuit et le monitoring d'une centrale solaire, en néon. Remplacé pour la carte par MapMortar (n° 25).
  - Breakthrough Energy (n° 2) est un site clair (fond `#FAFBF8`, accent vert-jaune `#DFFF5C`), pas un « tableau de bord de nuit ». La direction B est corrigée.
  - Citron (n° 16) : les titres « Automatisez… » ne sont pas sur l'accueil. Advizeo (n° 18) : la fourchette « 10 à 40 % » n'y est pas non plus.
  - Les calculateurs n° 8 et 9 sont des projets immobiliers, pas énergie. Deux calculateurs énergie ont été ajoutés (n° 23 et 24).
- **Ajouts** : 3 références Dribbble ouvertes et capturées (n° 23, 24, 25). One Page Love a été consulté : ses 20 résultats « energy » sont hors sujet (un guide de 2012 hors ligne, des gabarits solaires), aucun n'est retenu. Godly n'a pas été essayé (il redirige vers recent.design).
- **Mobile** : 3 sites réels capturés en 390 × 844 px (Deepki, ON Energy, Citron). Voir la section « Mobile, observé ».
- **Bannières cookies** : refusées partout où un refus existait (« Decline All », « Deny all cookies », « Reject All », « Continuer sans accepter »). Breakthrough Energy, ON Energy et carbonplan n'affichaient pas de bannière.
- **Données personnelles** : sur Dribbble, les avatars et les noms des designers ont été masqués avant capture. Les crédits d'Awwwards ont été laissés hors cadre.

**Répartition (après mise à jour)** : 25 références. Sites réels du secteur 5 · Dribbble 10 · Awwwards 3 · Pinterest 3 · Lapa Ninja 2 · Land-book 1 · Behance 1. Energy Park est cité sur Awwwards et sur Lapa Ninja.

---

## 1. Hero

| # | Titre | Source | URL | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 1 | BrainBox AI : AI Control | Site réel (Canada) | https://brainboxai.com/en/solutions/ai-control | [capture](captures/01-brainboxai-ai-control.jpg) · [chiffres](captures/01-brainboxai-chiffres.jpg) | Fond blanc, texte `#17171B`, Atlas Grotesk graisse 300, H1 56 px. **Correction** : le H1 est « AI Control », suivi d'une phrase de bénéfice. Le chiffre n'est que dans la balise `<title>` (« Reduce building energy consumption by up to 25% »). Sous le hero, deux grandes cartes blanches sur fond gris : « -40% » (émissions CO₂ liées au CVC) et « -25% » (coûts d'énergie CVC), chiffres très fins, flèche rouge vers le bas. Les légendes disent « by up to ». Onglet vertical rouge « Let's talk » collé à droite. **À reprendre** : le chiffre en très grand et fin, l'unité collée, une légende courte dessous. **À éviter** : le « jusqu'à » dans la légende. Pour Sobra, le chiffre passe en H1, avec une moyenne mesurée et sa note de méthode. |
| 2 | Breakthrough Energy | Awwwards SOTD (15/01/2026, 7,38, studio Resn) + site réel | https://www.awwwards.com/sites/breakthrough-energy · https://www.breakthroughenergy.org/ | [fiche](captures/02-breakthrough-energy-awwwards.jpg) · [site](captures/02-breakthrough-energy-site.jpg) · [plus bas](captures/02-breakthrough-energy-sections.jpg) | Palette relevée par Awwwards : vert-jaune `#DFFF5C` et blanc cassé `#FAFBF7`. Le site est clair. Hero : vidéo plein cadre d'ingénieurs en atelier, titre géant en blanc (police Saans) « Empowering innovators to build the future of energy ». Plus bas, un collage de photos qui flottent autour d'un logo vert-jaune, dont des éoliennes et des champs. L'accueil n'a presque pas de texte : un titre, une inscription à la newsletter, un menu. **Correction** : pas de « hiérarchie typographique éditoriale », et pas de registre sombre. **À reprendre** : le grand titre sur photo réelle de personnes au travail. **À éviter** : le collage d'images de nature et d'éoliennes. |
| 3 | ON Energy | Awwwards SOTD (09/03/2026, 7,44, Studio 28K) + site réel | https://www.awwwards.com/sites/on-energy · https://www.on.energy/ | [fiche](captures/03-on-energy-awwwards.jpg) · [site](captures/03-on-energy-site.jpg) | Fond noir `#000`, texte `#EEEEEE`, Univers Next Pro graisse 300, H1 64 px « Grid-Safe Power for AI Factories. » (la fiche Awwwards montre une version antérieure : « Perfect Power for AI Factories. »). Photo produit en niveaux de gris (une armoire électrique) et **un seul accent jaune `#FFF313`** : logo, bouton « Get in touch » à texte noir, carte « Explore AI UPS ». Navigation en pastilles grises translucides, rayon 6 px. **À reprendre** : la photo d'équipement réel désaturée et l'accent jaune unique. C'est le registre le plus proche de la direction A, en version sombre. **À éviter** : la 3D et le noir intégral pour un public de gestionnaires de bâtiments. |
| 4 | Galactic Energy | Land-book | https://land-book.com/websites/26111-galactic-energy | Non vérifié (Cloudflare) | **Non vérifié** : Land-book bloque par un challenge Cloudflare. Le nom correspond probablement au lanceur de fusées chinois Galactic Energy (https://www.galactic-energy.cn/, ouvert : « Build the next generation of commercial launch vehicles »), donc hors secteur. Le « grand titre sur image plein cadre » est mieux illustré par les n° 2 et 3, vus. |

## 2. Chiffres d'impact et compteurs

| # | Titre | Source | URL | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 5 | Deepki | Site réel (FR, version anglaise) | https://www.deepki.com/ | [capture](captures/05-deepki.jpg) · [chiffres](captures/05-deepki-chiffres.jpg) | Fond `#F8F8F8`, H1 en Century Gothic Bold 44 px `#111` avec « Most trusted » en sarcelle `#18A19A`, boutons sarcelle arrondis (rayon 25 px), texte en Roboto. Sous le titre : « Trusted by 900+ companies • $5T monitored ». Le hero est une vraie capture de la plateforme : une courbe de trajectoire carbone 2020-2050 avec une infobulle « 2033 » qui compare objectif, actions et scénario tendanciel. Plus bas, 3 cartes chiffres, **chacune signée d'un logo client** : « 6,500+ buildings monitored » (CBRE), « 40% time saved on reporting campaigns » (Icade), « 32% reduction in energy consumption » (Heppner). Un bandeau annonce le Deepki Index 2026. **Correction** : l'IPMVP n'apparaît pas sur l'accueil. **À reprendre** : le chiffre attribué à un client nommé, la courbe de trajectoire annotée. **À éviter** : le superlatif « Most trusted » et le « 32 % » sans période ni périmètre. |
| 6 | Tag « impact » et shot « Cambium : Impact » (Exo Ape) | Dribbble | https://dribbble.com/tags/impact · https://dribbble.com/shots/24767351-Cambium-Impact | [tag](captures/06-dribbble-tag-impact.jpg) · [Cambium](captures/06-dribbble-cambium-impact.jpg) | **Correction** : le tag « impact » montre surtout des logos (une marque « ImpactPilot » occupe la première page), pas des sections « Our impact ». Le shot Cambium Impact, lui, montre un seul chiffre géant en serif terracotta sur fond crème : « 3.5 Gigaton CO2e », « / Year » en petit, puis une phrase de comparaison et un bouton « More impact ». Un globe terrestre en 3D occupe la moitié gauche. **À reprendre** : un chiffre par écran, l'unité en petit, une phrase qui le rend concret. **À éviter** : le globe. |
| 7 | Green Energy Website Design Inspiration | Pinterest (page d'idées) | https://www.pinterest.com/ideas/green-energy-website-design-inspiration/953706463630/ | Non vérifié (connexion) | **Non vérifié** : mur de connexion « Log in to see more ». Derrière la fenêtre, on devine des gabarits à éoliennes, panneaux solaires et vert vif, mais aucune épingle n'est identifiable. L'épingle « hero photo + icônes + compteurs + formulaire de devis » n'a pas pu être retrouvée. Équivalent vu : le n° 23 (Sunora AI), qui a exactement cette structure. |

## 3. Simulateur

| # | Titre | Source | URL | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 8 | Savings calculator (Opendoor Design) | Dribbble | https://dribbble.com/shots/13944005-Savings-calculator | [capture](captures/08-dribbble-opendoor-savings-calculator.jpg) | **Projet immobilier**, pas énergie (« bundle and save » : vendre, acheter, financer). Deux pistes de landing. Le calculateur est une carte : un curseur de prix, des interrupteurs par service, puis « Total est. savings $5,000 » en bas de la carte. Texte à gauche, carte à droite. Le designer note qu'un calculateur est délicat juridiquement. **À reprendre** : le résultat en bas de la carte, sous les entrées, et la prudence juridique (afficher les hypothèses). |
| 9 | Savings Slider (Ryan Ostrander) | Dribbble | https://dribbble.com/shots/2635549-Savings-Slider | [capture](captures/09-dribbble-savings-slider.jpg) | **Projet immobilier** (thème WordPress pour un agent). Une seule image floue et zoomée : un curseur à pastille rouge (icône maison), « Sale price $420,000 », « Savings $11,1… ». Peu exploitable. L'idée du curseur doublé d'un champ numérique est mieux montrée par le n° 24. |
| 10 | Mobile Energy Savings Calculator | Dribbble (shot ancien, basse définition) | https://dribbble.com/shots/787436-Mobile-Energy-Savings-Calculator | [capture](captures/10-dribbble-mobile-energy-calculator.jpg) | Écran bleu ardoise : « Cooling Savings », « 38% Saved per year* » en très grand avec un anneau de progression, puis les économies à 5, 10 et 15 ans (« $432 », « $864 », « $1,232 »), une note « *Based on US national… » et un champ « 20 » avec « Update ». **Correction** : rien ne montre « une étape par écran » ni des boutons de type de bâtiment. **À reprendre** : l'astérisque relié à une note de méthode sous le résultat, et le gain sur plusieurs horizons. |
| 23 | Sunora AI : Energy Calculator Web (Trexa Lab) | Dribbble (ajout) | https://dribbble.com/shots/27487059-Sunora-AI-Solar-Energy-Website-Design-Energy-Calculator-Web | [capture](captures/23-dribbble-sunora-energy-calculator.jpg) | Hero sombre sur photo de champ solaire au couchant, 3 chiffres sous le titre (« 4.9/5 », « 70% Potential bill reduction », « 850+ Homes powered ») et **un mini-calculateur dans le hero** : facture mensuelle, bouton « Calculate Savings », résultat « $169 est. monthly savings ». Un second écran détaille le résultat en tableau : économie mensuelle, puissance conseillée (6.9 kW), retour sur investissement (9.5 ans). CTA vert vif. **À reprendre** : le résultat présenté en tableau de 3 lignes. **À éviter** : le champ solaire, le vert vif et le « 70 % » sans méthode. C'est la structure type du secteur que décrivait le n° 7. |
| 24 | Solar energy saver calculator | Dribbble (ajout) | https://dribbble.com/shots/24936784-Solar-energy-saver-calculator | [capture](captures/24-dribbble-solar-saver-calculator.jpg) | **Le modèle le plus direct pour le simulateur Sobra.** Entrées à gauche : un curseur de facture doublé d'un champ « €23 Euro », puis des boutons segmentés (pans de toit, orientation, chauffage). Résultat à droite, qui change en direct : « Estimated annual savings (EUR) €324 », bascule « 1 year / 25 years », puissance, retour (« ≈24.8 years »), réduction de CO₂ en kg par an. Une phrase dit que le calcul est indicatif, à côté du bouton « Get a Quote ». **À reprendre** : la mise en page, le champ numérique à côté du curseur, la phrase « indicatif ». **À éviter** : l'équivalence en arbres plantés, garder kWh et kg CO₂. |

## 4. Data-viz, courbes et carte des bâtiments

| # | Titre | Source | URL | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 11 | Energy Consumption Dashboard UI (Fuselab Creative) | Dribbble | https://dribbble.com/shots/25574779-Energy-Consumption-Dashboard-UI | [capture](captures/11-dribbble-fuselab-energy-dashboard.jpg) (image à 22 s de la vidéo) | Vidéo de 27 s : une ville en 3D de nuit, un zoom sur une centrale solaire, puis chaque panneau avec sa valeur en W, une alerte rouge, un panneau « Root cause analysis » et une courbe de production. Bleu marine et néons bleu et magenta. **Correction** : la description parle d'une carte qui compare des sites par code postal, mais la vidéo ne montre qu'un seul site. Ce n'est pas un modèle pour la carte des bâtiments, c'est le **dashboard décoratif à éviter**. Remplacé par le n° 25. |
| 12 | Dashboard for an innovative energy storage product (BatteryLoop) | Dribbble | https://dribbble.com/shots/21454833-Dashboard-for-an-innovative-energy-storage-product | [capture](captures/12-dribbble-batteryloop-dashboard.jpg) | Écrans sombres vert-noir. « Consumption Overview » en aires empilées vert, orange et jaune. « Savings from BLESS Storage » et « Savings from Peak Shave » chiffrés en SEK. Schéma de flux d'énergie. **Correction** : ce sont des aires empilées, pas des barres. **À reprendre** : le gain décomposé par levier, chacun avec son montant. Pour Sobra, l'équivalent « réglages CVC / détection de dérives / suivi » en version claire. |
| 13 | Smart Energy Dashboard Concept (Zajno) | Dribbble | https://dribbble.com/shots/25108413-Smart-Energy-Dashboard-Concept | [capture](captures/13-dribbble-zajno-smart-energy.jpg) | Fond noir et cartes vert sauge pâle, typo fine. La consommation est découpée **par usage** (éclairage, réfrigérateur, climatisation), en barres et en **fourchettes** : « 52–71 kWh per month ». Rapport hebdomadaire en kWh par jour, « 47% » d'énergie verte. Contexte domestique. **Correction** : pas de courbe annotée ni de repérage de pic dans l'écran vu. **À reprendre** : la fourchette avec l'unité en petit (le format du résultat du simulateur) et le découpage par usage, qui correspond au sous-comptage des capteurs Sobra. |
| 14 | eTactica | Lapa Ninja | https://www.lapa.ninja/post/etactica/ | Non vérifié (Cloudflare, site mort) | **Non vérifié** : Lapa Ninja bloque par Cloudflare, et `etactica.com` redirige vers une page de nom de domaine à vendre. Référence abandonnée. Les landings « outil de mesure » B2B sont couvertes par les n° 5, 17 et 18. |
| 25 | MapMortar : Decarbonisation Platform Design (Lumi studio) | Dribbble (ajout) | https://dribbble.com/shots/26536376-MapMortar-Decarbonisation-Platform-Design | [capture](captures/25-dribbble-mapmortar-decarbonisation.jpg) | Interface claire. Une carte de quartier en gris avec des repères colorés **par statut de trajectoire** : « On track » (noir), « Off track » (orange), « No plan » (gris). À gauche : deux cartes chiffres avec l'unité et la période (« 876,000 kg per year » de CO₂ scope 1, « 257,200 kWh per year »), un anneau par type de bâtiment, des « Next actions », une « Decarbonisation progress » à 16 %. **Modèle direct pour la carte des bâtiments équipés** : des points agrégés colorés selon la trajectoire 2030, avec la légende chiffrée sous la carte. |

## 5. Ton éditorial, sobriété, crédibilité

| # | Titre | Source | URL | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 15 | carbonplan | Lapa Ninja (bloqué) + site réel | https://www.lapa.ninja/post/carbonplan/ · https://carbonplan.org/ | [site](captures/15-carbonplan.jpg) | Lapa Ninja : non vérifié (Cloudflare). Site réel : fond sombre `#1B1E23` (un bouton permet de passer en clair), H1 « Data and science for climate action » en relative-medium-pro 64 px `#EBEBEC`. Le hero est une grille de 12 petites data-viz (barres, courbe, points, curseurs) à la place d'une photo. Liens de navigation en capitales soulignées, coordonnées en chiffres mono dans la marge, articles datés en capitales (« MAY 07 2026 »). **À reprendre** pour la page Méthode : les dates visibles, les petites data-viz comme illustration, le ton sec. **À éviter** : le fond sombre par défaut pour Sobra. |
| 16 | Citron | Site réel (FR) | https://citron.io/ | [capture](captures/16-citron.jpg) | Hero en dégradé vert (du sarcelle `#00AEA2` au vert-jaune), H1 blanc en Open Sans 800 48 px : « Accélérons la transition énergétique de vos bâtiments ! ». Bouton magenta `#E71B6D`, rayon 8 px. Illustration plate d'une femme avec une loupe devant une maquette de tableau de bord (jauge « 21,3 », anneau). L'allégation précise est confirmée : « Citron® répond à 3 des 7 obligations liées au décret BACS ». **Correction** : les titres « Automatisez… » ne sont pas sur l'accueil (« Améliorez… » n'est qu'un lien de menu), et le H1 est une exhortation avec point d'exclamation. **À reprendre** : l'allégation réglementaire chiffrée et sa source. **À éviter** : le dégradé vert, le personnage à loupe, le point d'exclamation. |
| 17 | Ubigreen | Site réel (FR, version anglaise) | https://www.ubigreen.com/en/ | [capture](captures/17-ubigreen.jpg) (sans mise en forme) · [témoignage](captures/17-ubigreen-cas.jpg) | Page affichée sans ses feuilles de style (erreurs 429), design non vu. Relevé dans le code : H1 en Open Sans 800, bleu marine `#091C4F`, texte gris `#666`. H1 : « Energy management platform for multi-site property portfolios ». Résultat client **confirmé**, en citation : de 2018 à 2021, gaz corrigé -5,3 % et électricité -13 %, attribué au responsable énergie du Conseil départemental de la Haute-Garonne, avec les leviers cités. **À reprendre** : le petit chiffre daté, corrigé, attribué à un client nommé, avec ses leviers. C'est le modèle des fiches cas Sobra. |
| 18 | Advizeo (by Hager) | Site réel (FR) | https://www.advizeo.io/ | [capture](captures/18-advizeo.jpg) · [chiffres](captures/18-advizeo-chiffres.jpg) | Hero vidéo teintée violet et rose, H1 « Maximiser les économies d'énergie sur votre patrimoine » en Kanit 59 px blanc, 3 cartes translucides « Connecter / Analyser / Piloter ». Bouton corail `#FC6A55`, rayon 40 px. Bandeau bleu nuit `#0D123C` avec chiffres corail : « 410 millions de m² optimisés », « + de 300 clients », « 1 TWh d'économies d'énergie réalisées en 2025 ». **Correction** : la fourchette « 10 à 40 % » n'est pas sur l'accueil, et le bandeau de logos par segment n'a pas été vérifié. **Contre-exemple** trouvé à la place : la même page dit « + de 300 clients » puis « plus de 250 acteurs », et « leader de l'Energy Management » sans source. **À reprendre** : le titre de replay « Covéa Immobilier : -33 % de consommation sur 1000 bâtiments, la méthode » (chiffre, périmètre et méthode dans la même ligne). |

## 6. Pages produit énergie et mobile

| # | Titre | Source | URL | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 19 | Manatee Energy Website (tubik) | Behance (oct. 2025, bloqué) + Dribbble | https://www.behance.net/gallery/236008203/Manatee-Energy-Website · https://dribbble.com/shots/26339570-Website-Design-Landing-page-for-Manatee-Energy | [Dribbble](captures/19-dribbble-manatee-energy-landing.jpg) | Behance : non vérifié (erreur 400). Le même projet est publié sur Dribbble par le studio tubik, en une douzaine de shots dont un dashboard client (titres vus dans la recherche). Landing vue : « Heat pump and water installations for the people », illustration isométrique de terrasses et de pompes à chaleur, bouton bleu « Get a quote », témoignages de particuliers. Plateforme grand public. **À reprendre** : publier la landing et les écrans produit ensemble. **À éviter** : l'illustration et le bleu vif, proscrits par le brief. |
| 20 | Energy Park | Awwwards SOTD (07/12/2023, 7,58, Outpost) + Lapa Ninja (bloqué) | https://www.awwwards.com/sites/energy-park · https://www.lapa.ninja/post/energy-park/ | [fiche](captures/20-energy-park-awwwards.jpg) | Palette relevée par Awwwards : jaune `#FFF555` et blanc. Hero : « Get set for an electric future. » en blanc sur une vidéo aérienne de route en forêt, bouton blanc en pilule avec une pastille jaune. **Non vérifié** : le site réel (energy-park.co.uk) affiche une erreur de certificat, la segmentation par lieu et le comportement mobile n'ont pas pu être vus. **À éviter** : la forêt comme décor. |

## Mobile, observé (390 × 844 px)

| Site | Capture | Ce qu'on voit au premier écran |
|---|---|---|
| Deepki | [mobile](captures/mobile-deepki.jpg) | H1 35 px sur 4 lignes, la preuve « Trusted by 900+ companies », puis le bouton « Get a demo » (51 px de haut). La capture de la plateforme rétrécit au point d'être illisible. Plus bas, les 3 cartes chiffres s'empilent, une carte d'environ 350 px de haut chacune. Pas de bouton collant. |
| ON Energy | [mobile](captures/mobile-on-energy.jpg) | Logo et menu dans une pastille jaune en haut à droite, H1 37 px graisse 300 sur la photo produit, carte jaune « Explore AI UPS » en bas. Le bouton « Get in touch » n'est pas dans le premier écran, seulement dans le menu et en pied de page. |
| Citron | [mobile](captures/mobile-citron.jpg) | H1 24 px, bouton « Contacter un expert » visible mais haut de 38 px seulement (sous les 44 px conseillés), bandeau de logos clients dès le premier écran. Le bouton flottant de gestion des cookies recouvre le bas à gauche. |

**Ce qu'on en tire pour Sobra** :
- Le CTA principal doit être dans le premier écran, à 48 px de haut (le token actuel). Citron (38 px) est trop petit, ON Energy le cache dans le menu.
- Ne pas réduire une capture de plateforme entière en mobile : la recadrer sur une seule courbe lisible.
- Les cartes chiffres empilées prennent vite de la place (Deepki : plus de 1 000 px pour 3 cartes). Garder 2 ou 3 cartes compactes.
- **Non observé** : aucun des 3 sites ne met d'outil juste après le hero (Deepki renvoie vers un « Benchmark your building in 60 seconds » plus bas). Le simulateur en premier écran après le hero reste un choix propre à Sobra, à valider en test utilisateur.

## 7. Moodboards Pinterest (repoussoir et codes du secteur)

| # | Titre | Source | URL | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 21 | Renewable Energy / Clean Tech Web Design (7 épingles) | Pinterest (tableau) | https://www.pinterest.com/jackkoppa/renewable-energyclean-tech-web-design/ | Non vérifié (connexion) | **Non vérifié** en détail : mur de connexion. La description du tableau est lisible sans compte et confirme l'intention (designs plutôt plats, bonnes images, navigation simple). Le tableau a 12 ans : derrière la fenêtre, on devine une infographie avec éolienne, solaire et hydraulique. Garder seulement l'idée de navigation simple. |
| 22 | Utilities / Energy websites (20 épingles) | Pinterest (tableau) | https://www.pinterest.com/backinvenice/utilities-energy-websites/ | Non vérifié (connexion) | **Non vérifié** : mur de connexion. Le tableau a 7 ans. Derrière la fenêtre, on devine des sites de fournisseurs d'énergie en bleu, violet et rose. Les clichés à éviter sont mieux documentés par ce qui a été vu : éoliennes et nature (n° 2, 20), champ solaire et vert vif (n° 23), globe (n° 6). |

---

## Synthèse du moodboard : 3 directions possibles

> Mise à jour du 2026-11-12 : la recommandation (direction A) ne change pas, les observations la confortent. Trois ajustements, expliqués ci-dessous : la référence de la direction B (Breakthrough Energy est un site clair), la mention de carbonplan en direction C (son site est sombre, seul le ton compte), et les modèles du simulateur et de la carte, désormais vus (n° 24 et 25).

**A. « Relevé de compteur » (recommandée)**
Fond sable, grands chiffres en Archivo étendu vert profond, une seule courbe avant/après en trait fin, et le jaune réservé au delta (« -27 % »).
Photos réelles de capteurs et de locaux techniques, en noir et blanc légèrement teinté vert.
Sensation : précision d'ingénieur, rapport technique bien mis en page.
Ce que les références vues confirment :
- la photo d'équipement désaturée avec un seul accent jaune fonctionne (ON Energy, n° 3) ;
- un chiffre par écran, unité en petit, une phrase dessous (Cambium, n° 6 ; BrainBox, n° 1) ;
- le chiffre signé par un client nommé et daté (Deepki, n° 5 ; Ubigreen, n° 17) ;
- le simulateur entrées à gauche, résultat à droite, avec une phrase « indicatif » (n° 24) ;
- la carte à points colorés selon la trajectoire (n° 25).

**B. « Tableau de bord de nuit »**
Fond vert profond quasi noir, chiffres en sable, jaune pour les alertes et les gains. Le simulateur ressemble à un instrument.
Plus spectaculaire (le registre d'ON Energy : noir, photo produit en niveaux de gris, jaune `#FFF313`), mais le risque « SaaS générique » est plus fort : les dashboards sombres vus (n° 11, 12, 13) se ressemblent tous.
À garder pour la section Impact cumulé seulement.
Correction : Breakthrough Energy, cité ici dans la première version, est un site clair (fond `#FAFBF8`).

**C. « Rapport annuel éditorial »**
Mise en page magazine : Space Grotesk, grandes marges, chiffres en exergue, notes de bas de page pour les sources.
Très crédible auprès des foncières et des investisseurs, et proche du ton de carbonplan (dates visibles, données expliquées), pas de sa mise en page, qui est sombre.
Moins direct pour la conversion : il faut un CTA collant.

**Observation sur l'accent jaune** : les 3 sites primés vus utilisent un seul accent jaune ou vert-jaune fluo (ON Energy `#FFF313`, Energy Park `#FFF555`, Breakthrough Energy `#DFFF5C`). Le jaune soleil de Sobra (`#F2C230`) est plus chaud et plus doré, ce qui le distingue de cette tendance. La palette ne change pas.

## Palette recommandée (direction A)

| Rôle | Hex | Usage |
|---|---|---|
| Vert profond | `#0E3B2E` | Titres, chiffres, fond des sections sombres |
| Vert encre | `#0A2A21` | Texte courant sur sable (contraste élevé) |
| Sable | `#EFE6D2` | Fond principal |
| Sable clair | `#F8F4EA` | Cartes, fond du simulateur |
| Jaune soleil | `#F2C230` | Accent unique : delta d'économie, focus, CTA sur fond vert |
| Gris vert data | `#7C8F86` | Courbe « avant » sur sable clair (pas de texte, voir les contrastes) |
| Rouge alerte (rare) | `#B8452F` | Dérive de consommation dans les courbes |

Contrastes calculés (WCAG 2.1) : le jaune `#F2C230` sur sable `#EFE6D2` donne 1,35:1, il **échoue**. Le jaune ne s'utilise que sur vert profond (7,44:1 avec `#0E3B2E`), ou en fond derrière un texte vert profond.
Le gris vert data `#7C8F86` donne 2,76:1 sur sable et 3,12:1 sur sable clair : **trop faible pour du texte** (légendes, valeurs d'axe), et sous 3:1 pour un trait de courbe sur sable. Les légendes passent en `neutral.700` `#3F4A44` (7,44:1 sur sable) ; `#7C8F86` reste pour la courbe « avant », sur sable clair uniquement.

## Polices (Google Fonts)

- **Archivo** (police variable, axe de largeur jusqu'à 125, plus la graisse) : gros chiffres et titres en largeur étendue, graisses 700 à 800.
- **Space Grotesk** : alternative pour les titres en direction C.
- **Inter** : texte courant et interface du simulateur.
- **JetBrains Mono** ou **IBM Plex Mono** : unités, valeurs dans les graphiques, notes de méthode.

## 3 « à ne pas faire »

1. **Pas de feuille, de planète, d'éolienne ni de prise électrique verte**, et pas de vert pomme. Rien qui crie « écolo » à la place de « mesuré ».
2. **Pas de dashboard décoratif** : pas de widgets inventés, pas de néon sur fond noir. Montrer une vraie courbe (anonymisée) avec une annotation lisible.
3. **Pas de chiffre sans méthode** : pas de « jusqu'à -40 % », pas de compteur qui tourne sans date de mise à jour ni lien vers le calcul.

---

## Design tokens (direction A, « Relevé de compteur »)

### Couleurs

| Token | Hex | Usage |
|---|---|---|
| `color.brand.primary` | `#0E3B2E` | Vert profond : titres, chiffres, fonds sombres, bouton primaire |
| `color.brand.primary-hover` | `#155240` | Survol du bouton primaire |
| `color.brand.ink` | `#0A2A21` | Texte courant |
| `color.brand.sand` | `#EFE6D2` | Fond principal |
| `color.brand.sand-light` | `#F8F4EA` | Cartes, simulateur |
| `color.brand.accent` | `#F2C230` | Jaune soleil : delta d'économie, focus, CTA sur fond vert uniquement |
| `color.semantic.success` | `#2F7D4F` | Économie confirmée, envoi réussi |
| `color.semantic.error` | `#B3261E` | Erreur de champ, échec d'envoi |
| `color.semantic.warning` | `#B86E00` | Dérive de consommation, hors périmètre (texte sur clair) |
| `color.semantic.info` | `#2D5C7A` | Notes de méthode, infobulles |
| `color.neutral.900` | `#1A1F1C` | Texte maximal |
| `color.neutral.700` | `#3F4A44` | Texte secondaire, légendes et valeurs des graphiques |
| `color.neutral.500` | `#7C8F86` | Courbe « avant » et traits d'axe, sur sable clair (pas de texte) |
| `color.neutral.300` | `#C9CFC6` | Bordures |
| `color.neutral.100` | `#EEF0EB` | Fonds neutres |
| `color.neutral.0` | `#FFFFFF` | Champs de formulaire |

Contrastes calculés (WCAG 2.1) : le texte `#0A2A21` sur `#EFE6D2` donne 12,39:1 (AAA). `#0E3B2E` sur `#EFE6D2` : 10,05:1. `sand-light` sur `brand.primary` (bouton primaire) : 11,36:1. Le jaune `#F2C230` est interdit en texte sur fond clair (1,35:1 sur sable). `neutral.500` `#7C8F86` ne sert pas au texte (2,76:1 sur sable).

### Typographie

| Token | Police | Taille (desktop / mobile) | Graisse | Interligne |
|---|---|---|---|---|
| `type.display` (chiffre du hero) | Archivo, largeur 125 | 120 / 64 px | 800 | 0.95 |
| `type.h1` | Archivo, largeur 115 | 56 / 36 px | 700 | 1.05 |
| `type.h2` | Archivo, largeur 110 | 40 / 28 px | 700 | 1.1 |
| `type.h3` | Archivo | 24 / 20 px | 600 | 1.25 |
| `type.stat` (cartes chiffres) | Archivo, largeur 125 | 64 / 48 px | 800 | 1.0 |
| `type.body-lg` | Inter | 20 / 18 px | 400 | 1.55 |
| `type.body` | Inter | 17 / 16 px | 400 | 1.6 |
| `type.small` | Inter | 14 px | 500 | 1.45 |
| `type.mono` (unités, méthode) | JetBrains Mono | 14 / 13 px | 500 | 1.4 |

### Espacement (base 4 px)
`space.1` 4 · `space.2` 8 · `space.3` 12 · `space.4` 16 · `space.5` 24 · `space.6` 32 · `space.7` 48 · `space.8` 64 · `space.9` 96 · `space.10` 128 px.
Section : 128 px desktop, 64 px mobile. Gouttière : 24 px, et 16 px de marge latérale sur mobile.

### Rayons
`radius.sm` 4 px (champs, tags) · `radius.md` 8 px (boutons) · `radius.lg` 16 px (cartes, simulateur) · `radius.full` 999 px (pastilles).
Les angles restent assez vifs pour garder un registre technique.

### Ombres
- `shadow.none` : par défaut, on préfère les bordures `neutral.300`.
- `shadow.sm` : `0 1px 2px rgba(10,42,33,.08)` (cartes au repos).
- `shadow.md` : `0 4px 16px rgba(10,42,33,.10)` (simulateur, carte survolée).
- `shadow.focus` : `0 0 0 3px #F2C230` (anneau de focus).

### Motion
- Durées : `motion.fast` 120 ms (survol, focus) · `motion.base` 200 ms (ouverture, transitions d'état) · `motion.slow` 400 ms (mise à jour du résultat du simulateur) · `motion.count` 1 200 ms (compteur, une seule fois à l'apparition).
- Easings : `ease.standard` `cubic-bezier(.2,0,0,1)` · `ease.enter` `cubic-bezier(0,0,0,1)` · `ease.exit` `cubic-bezier(.3,0,1,1)`.
- `prefers-reduced-motion` : compteur et courbes affichés directement à leur valeur finale.

## Composants clés

- **Bouton primaire** : fond `brand.primary`, texte `sand-light`, `radius.md`, hauteur 48 px (zone tactile d'au moins 44 px).
  - Survol : `primary-hover`. Focus : `shadow.focus`. Actif : enfoncé de 1 px.
  - Désactivé : fond `neutral.300` et texte `neutral.700`. Ajouter `aria-disabled` et dire pourquoi il est désactivé.
  - Chargement : spinner et libellé « Envoi… », sans changement de largeur.
- **Bouton secondaire** : contour de 1,5 px `brand.primary`, fond transparent.
  - Survol : fond `neutral.100`. Focus, désactivé et chargement comme le primaire.
  - **Sur fond vert** : fond `accent` et texte `brand.primary`.
- **Carte chiffre** : fond `sand-light`, chiffre `type.stat`, unité `type.mono`, une ligne de contexte, et le lien « source » en `type.small`.
- **Carte cas client** : mini-courbe avant/après, type, surface, ville, gain sur 12 mois, et le lien « Voir la courbe ».
- **Formulaire / simulateur** :
  - libellé toujours visible au-dessus du champ ;
  - aide en `type.small` ;
  - erreur en `semantic.error`, avec icône et texte (jamais la couleur seule) ;
  - curseur de surface doublé d'un champ numérique ;
  - résultat annoncé par `aria-live="polite"` ;
  - résultat en fourchette avec l'unité en petit (format vu au n° 13), suivi d'une phrase « estimation indicative » et du lien vers les hypothèses (comme au n° 24).

| À faire | À ne pas faire |
|---|---|
| Un seul bouton primaire par écran (audit ou simulation) | Deux CTA jaunes côte à côte |
| Afficher la source et la date sous chaque chiffre | Un compteur animé sans date ni méthode |
| Libellés de champ visibles et unités explicites (m², kWh) | Placeholder qui sert de libellé |
| Erreur décrite (ce qui s'est passé, pourquoi, comment corriger) | « Champ invalide » en rouge seul |
| Courbes avec une alternative en tableau de données | Graphique sans texte alternatif ni légende |
| Jaune réservé à l'accent et au focus | Jaune en texte sur fond sable |
