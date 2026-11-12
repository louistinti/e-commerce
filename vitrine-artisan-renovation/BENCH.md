# Benchmark visuel : Arotz Rénovation (artisan RGE, Pays basque)

## Limites, à lire en premier

- **Références ouvertes et capturées le 2026-11-12**, dans un navigateur Chrome piloté (viewport 1440×900, au-dessus de la ligne de flottaison, et 390×844 pour le mobile). Les captures sont dans [`captures/`](captures/). Les couleurs et les polices citées ont été relevées dans la page (styles calculés), pas devinées. Pour les shots Dribbble, qui sont des images, seules les couleurs visibles sont décrites. Les contrastes sont calculés selon la formule WCAG 2.1.
- **14 références sur 20 vues et capturées.** Les 2 liens Pinterest (n° 15 et 16) s'ouvrent, mais une fenêtre de connexion recouvre la page : seul le texte a été lu, aucune capture (le dépôt est public, pas de page de connexion). Les 3 liens Behance (n° 4, 19 et 20) renvoient une **erreur HTTP 400** au navigateur automatisé. Lapa Ninja (n° 18) affiche **« Sorry, you have been blocked »** (Cloudflare). Aucune protection n'a été contournée. Ces références gardent leur texte, marqué **non vérifié**.
- **Remplacées par des pages ouvertes** : n° 18 par le vrai site de Quilt, n° 19 par l'accueil d'Effy. Le n° 20 (Manatee) n'a pas de remplaçant : la seule trace trouvée est une adresse de préproduction, pas un site public.
- **6 références ajoutées** (n° 21 à 26) : un shot de PAC en français, la fiche d'un artisan du 64 sur l'annuaire Effy, 2 pages officielles France Rénov', un vrai site d'entreprise de rénovation avec curseur avant/après, et un shot avant/après en même cadrage.
- **Corrections importantes** :
  - **Le bandeau France Rénov' est obligatoire depuis le 1er octobre 2026** sur tout support de promotion de travaux de rénovation énergétique (loi Cazenave, amende jusqu'à 75 000 € pour une société, n° 23). Le brief le classe encore « à confirmer par un juriste » : c'est désormais un composant à prévoir.
  - Final Touch Carpentry (n° 2) n'a pas de CTA dominants : 2 boutons fantômes de même poids. Son site renvoie aujourd'hui vers une autre activité (FTCC Group, réparation pour assureurs).
  - Le shot n° 3 n'a pas d'icônes de services ni de curseur : des cartes photo de banque d'images et une seule photo coupée en deux.
  - Le shot n° 6 est un écran de résultat (400×300 px), sans boutons de choix ni progression.
  - Le shot n° 8 n'a rien d'un avant/après de chantier : c'est l'histoire d'un bâtiment (« Wiley Club »). Remplacé pour le curseur par les n° 25 et 26.
  - Le lien du vrai site du shot n° 9 est mort (le domaine ne répond plus).
  - PRB Architects (n° 14) montre des rendus de bâtiments contemporains, pas du bâti ancien.
  - One Page Love compte 2 exemples de menuisiers (pas une sélection), dont le français est hors ligne depuis des années, et 9 exemples construction (pas 8, Keystone n'y figure pas).
  - Le tag « heat-pumps » (n° 17) n'est pas dominé par des fonds bleus : plutôt du rouge, du vert, des promos et des rendus produit.
- Aucun formulaire n'a été rempli ni envoyé. Le parcours Effy (n° 5) n'a pas été avancé au-delà du premier écran, car chaque réponse part vers leur serveur. Sur les captures, les photos de clients (n° 10) et les signatures et avatars de designers (Dribbble, Awwwards) ont été masqués.

**Répartition** : 26 références. Sites réels du secteur 9 (dont 2 officiels et les 2 remplaçants) · Dribbble 9 · One Page Love 2 · Awwwards 2 · Behance 2 (inaccessibles) · Pinterest 2 (mur de connexion). Les n° 18 (Lapa Ninja, bloqué) et 19 (Behance, inaccessible) sont comptés avec le site réel qui les remplace. Land-book et Godly n'ont pas été retestés : sur ce projet, Land-book bloque par Cloudflare et Godly redirige vers recent.design.

---

## 1. Hero

| # | Titre | Source | URL | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 1 | Aira : Heat pump installation | Site réel (UK) | https://www.airahome.com/en-gb/heat-pump-installation-2 | [hero](captures/01-aira-installation.jpg), [questions](captures/01-aira-installation-questions.jpg) | Texte alternatif confirmé : deux installateurs bras croisés devant la camionnette jaune Aira, une pastille ronde « Which? Trusted Trader » posée sur la photo. Fond blanc, H1 « Seamless heat pump installation » en airaText (police maison) 400, 54 px, `#222226`. À droite, 4 puces, dont la prime de 7 500 £ « grant eligibility applies ». CTA « Get a quote » `#222226` sur orange `#FFAF51` (8,7:1). Le téléphone est en texte dans l'en-tête. Plus bas : « Answer 4 quick questions » avec 5 cartes à pictogramme (type de maison), et un mur de logos (Which?, HIES, CTSI, MCS, Gas Safe) sans aucun numéro. Le carrousel Trustpilot précise « Showing our 4 & 5 star reviews ». **À reprendre** : l'équipe réelle et le label dans la même image, version Arotz avec la pastille RGE **et son numéro**. **À éviter** : les logos sans numéro et les avis filtrés (le brief exclut toute sélection trompeuse). |
| 2 | Final Touch Carpentry | Awwwards (nominé, 21/07/2021) | https://www.awwwards.com/sites/final-touch-carpentry | [fiche](captures/02-awwwards-final-touch-carpentry.jpg), [site actuel](captures/02-ftcc-site-reel.jpg) | La fiche dit bien « Function and conversion over design » (agence sitecentre), notes de la communauté entre 5,4 et 8,8. **Correction** : la capture montre un hero bleu nuit, une accroche manuscrite dorée, « SYDNEY TIMBER DECKING MADE EASY. » en capitales et **2 boutons fantômes de même poids** (« Request a quote » bordé d'or, « Call us now » bordé de blanc). Le téléphone est encadré en haut à droite. Le lien « Visit Site » (ftcc.com.au) mène aujourd'hui à **FTCC Group**, réparation de sinistres pour assureurs : hero `#17222A`, H1 Barlow Condensed 700, 78 px, or `#B8965F`, et une carte de 4 chiffres définis (« 10+ » ans, « 3000+ » sinistres, « <24 Hrs » d'intervention, « <5% » de reprises). **À reprendre** : des chiffres avec leur définition à côté. **À éviter** : 2 CTA fantômes de même poids. |
| 3 | Home Renovation Service : Website Landing Page | Dribbble | https://dribbble.com/shots/21920571-Home-Renovation-Service-Website-Landing-Page | [capture](captures/03-dribbble-home-renovation-service.jpg) | Une seule image de 4800×3600 px. Fond blanc et crème, accent orange (bouton « GET STARTED », « GET A QUOTE »), titres en sans géométrique noire, pastille « 12+ years ». **Correction** : pas d'icônes de services, mais 3 cartes photo (« Interior Renovation », « Home Maintenance », « Painting Services »), toutes de banque d'images (bricoleur à la scie, plombier souriant). L'avant/après se réduit à une photo coupée en deux dans la carte « Interior Renovation ». La description ne parle pas d'avant/après. **À reprendre** : la chaleur du crème et un seul accent. **À éviter** : la banque d'images. |
| 4 | Squarespace Construction Home Renovation Website | Behance (07/2026) | https://www.behance.net/gallery/252421797/SQUARESPACE-CONSTRAUCTION-HOME-RENOVATION-WEBSITE | inaccessible | **Inaccessible (erreur HTTP 400 de Behance)**, non vérifié. D'après la description : un site de rénovation centré sur les chantiers terminés, réalisé sur un constructeur de sites. |

## 2. Estimateur d'aides

| # | Titre | Source | URL | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 5 | Effy : Estimez votre prime énergie | Site réel | https://www.effy.fr/parcours/1/accueil | [desktop](captures/05-effy-parcours.jpg), [mobile](captures/mobile-effy-parcours.jpg) | L'URL redirige vers `/parcours/1/travaux-aides/logement-type`. Fond `#F0F6FF`, barre de progression bleue `#4754FF` tout en haut, pastille « En 2 minutes ! », H2 « Découvrez vos primes et estimez le coût de vos travaux » en buenos-aires 700, 32 px, bleu nuit `#161637` avec la fin en bleu (4,9:1 sur le fond). Une question, 2 grandes cartes à pictogramme et bouton radio (maison, appartement). À gauche, « Depuis 17 ans », Trustpilot 4,4 sur 9 005 avis et la mascotte (une femme à ailes de fée, « Élue marque de l'année 2026 »). Sur mobile : « 1/4 Votre logement », cartes de 312×64 px, bouton téléphone jaune de 54×48 px en haut à droite. **À reprendre** : une question par écran, « 1/4 » nommé et la barre de progression. **Non vérifié** : le moment où Effy demande les coordonnées, car le parcours n'a pas été avancé. Chez Arotz, le résultat s'affiche avant toute demande de contact. |
| 6 | Mobile Energy Savings Calculator (Patrick Bartenstein) | Dribbble | https://dribbble.com/shots/787436-Mobile-Energy-Savings-Calculator | [capture](captures/06-dribbble-mobile-energy-calculator.jpg) | **Correction** : l'image fait 400×300 px et montre un seul écran de résultat dans un iPhone ancien. « Cooling Savings », un interrupteur « COOL », un anneau et « 38 % Saved per year* », puis 3 montants sur 5, 10 et 15 ans, une note « *based on US national… » et un champ avec « UPDATE ». Pas de gros boutons de choix ni de progression. **À reprendre** : le résultat en très grand, avec l'astérisque et sa source collés dessous. Version Arotz : la fourchette d'aides en grand, « indicatif, barème du JJ/MM/AAAA » juste dessous. |

## 3. Réalisations avant/après

| # | Titre | Source | URL | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 7 | Remodelmate Before/After (Marko Ilic) | Dribbble | https://dribbble.com/shots/13476909-Remodelmate-Before-After | [capture](captures/07-dribbble-remodelmate-before-after.jpg) | Confirmé (vidéo). Un carrousel de cartes, une poignée ronde sombre au milieu de la photo, une bulle de témoignage posée sur l'image, et sous la photo « Budget $5000 », « Time 3 weeks » et le nom de l'artisan. Flèches et points de pagination. La description le dit : montrer les photos, mais aussi le coût, la durée et la personne derrière. Le sous-titre est encore en faux texte. **Référence principale** pour le contenu de la carte. Version Arotz : curseur, classe DPE avant → après, commune, travaux, durée, extrait d'avis. |
| 8 | Before and After Website Transition (Christian Reindl) | Dribbble | https://dribbble.com/shots/7180177-Before-and-After-Website-Transition | [capture](captures/08-dribbble-before-after-transition.jpg) | **Correction** : ce n'est pas un avant/après de chantier. Le GIF montre « Zeitreise durchs Wiley », un site d'histoire d'un bâtiment (« Wiley Club »), avec une photo noir et blanc et des motifs géométriques rouges. Rien à reprendre pour le curseur : voir les n° 25 et 26. |
| 9 | Renovations website (One-Shot Marketing) | Dribbble | https://dribbble.com/shots/20485061-Renovations-website | [capture](captures/09-dribbble-renovations-website.jpg) | Un carrousel de cuisine blanche, le logo au centre, des services en photos rondes (dont une main qui tient une maison miniature) et une grille « Recent projects ». **Lien mort** : le site annoncé dans la description (khokharrenovation.com) ne répond plus (domaine introuvable). **À éviter** : la maison miniature, un cliché de banque d'images. |
| 10 | Aira : Roger & Sue's installation | Site réel (UK) | https://www.airahome.com/en-gb/case-studies/roger-sue-aira-heat-pump-installation | [capture](captures/10-aira-roger-sue.jpg) (photo des clients floutée) | H1 de 94 px en airaText 400, la photo du couple devant la maison, un fil d'Ariane qui donne la ville. Puis « Property details » (maison individuelle, 2 niveaux, 3 chambres, construction récente), « The installation at a glance » (lieu, matériel posé dont « 11 new radiators », aide obtenue), puis défi, solution et verdict. Le technicien est nommé par son prénom. Le seul chiffre de résultat est dans la citation du client (« around 50% » d'économies en janvier et février). Une FAQ répond au bruit. **À reprendre** : le bloc « le chantier en bref » (logement, travaux, aide), le prénom du compagnon. Format « Maite et Jean-Pierre, Anglet ». |
| 11 | Hellio : Rénovation globale, 76 % d'économies à Orléans | Site réel | https://www.hellio.com/actualites/communiques/renovation-energetique-orleans-globale | [capture](captures/11-hellio-orleans.jpg) | Title de la page : « Évolution de la lettre F à B au DPE : 76 % d'économies d'énergie ». H1 en Lexend 700, 32 px, `#3A3A3A`. Une photo réelle de la maison après travaux (pas de photo avant), 156 m², chantier d'un mois, travaux listés, artisans locaux nommés. Le gain est au futur (« réalisera 76 % ») : c'est une estimation. Mis à jour le 20 nov. 2025, mais le texte parle encore des règles de 2024. CTA « Contacter un expert » blanc sur `#0070BB` (5,2:1). **À reprendre** : le titre « travaux, gain, ville » et la classe DPE avant → après. Écrire « gain estimé par l'audit », comme le brief le demande. |
| 25 | NSH Renovierung (Vechta, Allemagne) | Dribbble + site réel | https://dribbble.com/shots/27865951-NSH-Renovierung-Renovation-Company-Website-Vechta et https://nsh-renovierung.de/ | [shot](captures/25-dribbble-nsh-renovierung.jpg), [hero](captures/25-nsh-renovierung-site-reel.jpg), [références](captures/25-nsh-renovierung-references.jpg), [mobile](captures/mobile-nsh-renovierung.jpg) | **Ajoutée.** Le meilleur exemple vu d'artisan local en production. H1 en Inter 800, 77 px, puis une seconde ligne en serif italique (« Neues Lebensgefühl. »), pastille « Bauunternehmen & Generalunternehmer in Vechta », un seul bouton bleu « Kostenlose Beratung » (blanc sur `#0B4EEE`, 6,3:1). Les références sont filtrables (Alle, Wohnung, Haus, Bad, Boden, Büro) et chaque carte a un curseur avec les étiquettes « Vorher » et « Nachher », de vraies photos de chantier et un titre « travaux + commune ». Le curseur a `role="slider"`, un `aria-label` et se pilote au clavier (5 % par appui sur une flèche). Les sous-traitances sont signalées par un astérisque. **À reprendre** : le curseur, les étiquettes toujours visibles, les filtres par travaux, l'astérisque honnête. **À éviter** : des chiffres qui se contredisent (« 80+ » projets et « +23 » clients dans le hero, « über 150 » clients plus bas), des logos de fournisseurs (Bosch, Knauf…) sous « Vertraut von Kunden », et un bouton d'en-tête coupé à 1440 px. |
| 26 | Before & After renovation | Dribbble | https://dribbble.com/shots/14540322-Before-After-renovation | [capture](captures/26-dribbble-before-after-renovation.jpg) | **Ajoutée.** Une seule photo où l'avant (briques à nu, plafond abîmé) se fond en diagonale dans l'après (mur jaune, cabine de douche), **avec exactement le même cadrage**. **À reprendre** : photographier l'avant et l'après du même point de vue, sinon le curseur ne prouve rien. À noter dans le brief du shooting. |

## 4. Artisanat, matières, photo

| # | Titre | Source | URL | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 12 | Carpenter Website Examples (dont L'Atelier de la Menuisière) | One Page Love | https://onepagelove.com/tag/carpenter | [capture](captures/12-onepagelove-carpenter.jpg) | **Correction** : 2 exemples seulement (« 2 Real Examples »). L'Atelier de la Menuisière est hors ligne : présenté en décembre 2011, il ne reste qu'une capture (outils roses sur fond blanc, coordonnées en pied de page). Rien d'exploitable pour un one-page artisanal actuel. |
| 13 | Construction Website Examples | One Page Love | https://onepagelove.com/tag/construction | [capture](captures/13-onepagelove-construction.jpg) | **Correction** : 9 exemples, pas 8, et pas de Keystone. On y trouve Rockmaster, Tegra, PIQ-Mecobat, Strömma Projekt, Kvadrat, Farbenhaus, Pandolfo Costruzioni et Tvoříme domovy. Pandolfo (2012), Tvoříme domovy (2011) et Farbenhaus (2015) sont hors ligne. D'après le texte de sa fiche, Farbenhaus expliquait son procédé en 8 étapes avec une infographie en poteaux de bois. **À retenir** : la galerie est vieillie, elle sert surtout d'idée pour le déroulé en 5 étapes. |
| 14 | PRB Architects | Awwwards SOTD (20/03/2021) | https://www.awwwards.com/sites/prb-architects | [capture](captures/14-awwwards-prb-architects.jpg) | Note de 7,43/10, palette relevée par Awwwards : `#000`, `#DF6C4F`, `#fff`. La description parle bien de construction durable et de patrimoine, mais **la capture montre des rendus 3D de bâtiments contemporains**, une grande flèche noire et des numéros de projet verticaux (« PRB 21-319 »). Le lien « Visit Site » pointe vers une archive (prb-archive.netlify.app). **Correction** : pas de registre « bâti ancien ». **À reprendre** : le numéro de chantier en légende, utile pour la direction C. |
| 15 | Renovation Inspiration (Architectural Digest) | Pinterest (tableau) | https://www.pinterest.com/archdigest/renovation-inspiration/ | aucune (mur de connexion) | **Non vérifié visuellement** : une fenêtre de connexion couvre le tableau. Lu sans compte : 687 épingles, créé il y a 6 ans. Les vignettes visibles autour de la fenêtre sont surtout des articles de décoration (rideaux, papier peint, erreurs d'entrepreneur), pas des photos de chantier. La direction photo (lumière naturelle, matières, cadrages serrés) reste à prendre ailleurs : n° 18 et 25. |
| 16 | Artisan Renovations (artisandns) | Pinterest (profil) | https://www.pinterest.com/artisandns/ | aucune (mur de connexion) | **Partiellement vérifié** (texte lu, mur de connexion). Entreprise de gestion de travaux de la région de Toronto, tableaux par pièce (chambre 28, salle de bains 44, cuisine 54, séjour 55 épingles), tous vieux de 7 ans. L'idée des réalisations filtrables par travaux est confirmée en production chez NSH (n° 25). |

## 5. Pompe à chaleur et identité du secteur

| # | Titre | Source | URL | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 17 | Tag « heat-pumps » (dont Immergas, Orange Energia) | Dribbble | https://dribbble.com/tags/heat-pumps | [capture](captures/17-dribbble-tag-heat-pumps.jpg) | **Correction** : peu de fonds bleus. Les 8 premiers shots sont un gabarit vert et blanc, Alpha Innotec (gris et rouge, rendu produit), Calorex (noir et rouge), Wambreck (vert, n° 21), Solares Energies (bleu nuit et vert), Orange Energia (noir et orange, maison illustrée). Immergas est rouge et blanc, avec une prime de « 2000 zł » en gros. Sert de **repoussoir** : rendus produit, primes en gros caractères, maisons illustrées. Chez Arotz, la PAC se montre posée, en photo réelle, avec l'installateur. Le rouge est courant chez les marques de PAC : le rouge basque reste réservé aux CTA. |
| 18 | Quilt | Lapa Ninja (2024), remplacé par le site réel | https://www.lapa.ninja/post/quilt/ → https://www.quilt.com/ | [site réel](captures/18-quilt-site-reel.jpg) | Lapa Ninja : **inaccessible (Cloudflare, « Sorry, you have been blocked »)**. Sur quilt.com : l'unité intérieure à façade bois photographiée dans un vrai salon, une main qui pose un vase devant. Titres en serif (« Quilt Serif », 60 px, blanc), texte en « Quilt Sans », boutons-pilules « Find an installer » et « Become a partner », bandeau pétrole `#186767` avec une citation de Wirecutter. Les avis sont titrés par type de maison (« Crisp and cozy bungalow »). **À reprendre** : la PAC posée dans un intérieur réel, et un titre d'avis qui dit le logement. La serif chaleureuse pour une PAC conforte Fraunces. |
| 19 | EFFY : Branding | Behance, remplacé par effy.fr | https://www.behance.net/gallery/99403091/EFFY-Branding → https://www.effy.fr/ | [accueil Effy](captures/19-effy-accueil.jpg) | Behance : **inaccessible (erreur HTTP 400)**. Sur l'accueil : H1 « Votre maison, en mieux. » en buenos-aires 700, 80 px, blanc sur un salon mis en scène, avec l'affiche de la mascotte au mur. CTA « J'estime mon projet » `#161637` sur jaune `#FFF164` (15:1), second bouton blanc « Je demande ma prime Effy », Trustpilot « Excellent ». Plus bas, « Votre pompe à chaleur dès 49€/mois ». C'est le code « plateforme nationale » **dont Arotz doit se distinguer** : mascotte, jaune vif, prime et mensualité en avant, aucun visage d'artisan. |
| 20 | Manatee Energy Website | Behance (10/2025) | https://www.behance.net/gallery/236008203/Manatee-Energy-Website | inaccessible | **Inaccessible (erreur HTTP 400)**, non vérifié. D'après la description : une plateforme d'installation de PAC qui promet facilité, transparence et prix abordable. Pas de remplaçant : la promesse de transparence (étapes, aide, matériel posé) est visible chez Aira (n° 1 et 10). |
| 21 | Landing Page heat pumps, Wambreck | Dribbble (projet fictif) | https://dribbble.com/shots/24770469-Landing-Page-heat-pumps | [capture](captures/21-dribbble-wambreck-pac.jpg) | **Ajoutée.** En français. La description annonce un « lead magnet » : calculer ses aides. Au-dessus du logo, un bandeau jaune défilant « -10% sur toute la gamme · Offre promo spéciale été ». À droite, « Appelez-nous ! Du lundi au vendredi, 8h à 19h ». H1 vert et noir « Réduisez vos factures d'énergie avec nos pompes à chaleur écologiques. », puis « En 20 ans, plus de 15 000 systèmes ». 2 boutons : « J'obtiens mon devis gratuit » vert plein, « Je calcule mes aides » en contour. **À reprendre** : les horaires collés au téléphone, et « Estimer mes aides » en second bouton du hero. **À éviter** : le bandeau promo (code du démarchage) et « écologiques », exclu par le brief. |

## 6. Preuves, labels et obligations

| # | Titre | Source | URL | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 22 | Fiche « Renovation 64 & Co » | Annuaire Effy (site réel) | https://www.effy.fr/artisans/pro/2807-renovation-64-co | [capture](captures/22-effy-fiche-artisan-64.jpg) | **Ajoutée.** Ce que voit un particulier du 64 qui cherche un artisan : un sigle « R6 » à la place d'un logo, « Partenaire Effy », 5,0 sur 1 avis, adresse et SIRET, 4 étiquettes de travaux, et un formulaire de devis Effy en jaune. Pas de photo, pas d'équipe, et aucun numéro RGE dans la partie lue. La demande part chez Effy, pas chez l'artisan. **À retenir** : c'est exactement ce que le brief décrit (« les plateformes captent les demandes locales »). Le site Arotz doit montrer ce que la fiche n'a pas : visages, numéro RGE, chantiers voisins. |
| 23 | Publicité pour la rénovation énergétique : obligation de faire référence à France Rénov' | Site officiel | https://france-renov.gouv.fr/actualites/publicite-pour-la-renovation-energetique-obligation-desormais-de-faire-reference-au | [capture](captures/23-france-renov-bandeau-publicite.jpg) | **Ajoutée, change le bench.** La loi Cazenave impose depuis le **1er octobre 2026** que tout support de promotion ou de publicité proposant des travaux de rénovation énergétique fasse référence à France Rénov' avec un bandeau donné : Marianne, logo France Rénov' et « Avant de vous engager, le service public vous informe gratuitement… ». Amende jusqu'à 15 000 € (personne physique) et 75 000 € (personne morale). Un kit est annoncé dans l'espace professionnels du site (non ouvert). **À faire** : le bandeau officiel sur le site, au minimum en pied de page et près de l'estimateur, à faire valider par un juriste pour l'emplacement. |
| 24 | Annuaire des professionnels RGE | Site officiel | https://france-renov.gouv.fr/annuaires-professionnels/artisan-rge-architecte | [capture](captures/24-france-renov-annuaire-rge.jpg) | **Ajoutée.** Deux onglets, « Rechercher par type de prestation » et « Rechercher un professionnel », et le rappel « pour bénéficier de MaPrimeRénov', il est obligatoire de confier ses travaux à un professionnel RGE ». Aucune recherche n'a été lancée, donc l'existence d'un lien direct par entreprise n'est pas vérifiée. **À reprendre** : le lien « Vérifier » de la carte label pointe vers cet annuaire, avec la consigne « tapez Arotz Rénovation » si aucun lien direct n'existe. |

---

## Mobile (390×844)

| Site | Capture | Ce qu'on observe |
|---|---|---|
| Aira, installation (n° 1) | [capture](captures/mobile-aira-installation.jpg) | Le téléphone n'est qu'une icône de 31×31 px dans l'en-tête, sous les 48 px visés par le brief. L'en-tête se masque quand on fait défiler. Pas de barre fixe en bas. Le CTA orange « Get a quote » ne fait pas toute la largeur. |
| Effy, parcours (n° 5) | [capture](captures/mobile-effy-parcours.jpg) | L'estimateur occupe tout l'écran : « 1/4 Votre logement », barre de progression, 2 cartes de 312×64 px. Le bouton téléphone jaune fait 54×48 px, en haut à droite, sans `aria-label` ni texte relevé. |
| NSH Renovierung (n° 25) | [capture](captures/mobile-nsh-renovierung.jpg) | Un en-tête flottant avec le logo et un menu burger. Les 2 CTA font toute la largeur. Le numéro de téléphone n'apparaît qu'en bas de page, à environ 12 500 px du haut. Pas de barre fixe. |

**À retenir** : aucun des 3 n'a de barre fixe avec « Appeler » et « Visite gratuite ». Le téléphone est soit trop petit (Aira), soit introuvable sans défiler (NSH). La barre fixe du brief reste un vrai différenciant pour les seniors. Effy confirme le format de l'estimateur plein écran. Recommandations, maintenant appuyées sur ces observations :
- une barre fixe en bas, 2 boutons égaux d'au moins 48 px : « Appeler l'atelier » (vert sapin plein) et « Visite gratuite » (rouge basque) ;
- l'estimateur en plein écran, « 1/4 » nommé (« 1/4 Votre logement ») et barre de progression, comme Effy ;
- des cartes de choix pleine largeur d'au moins 64 px de haut ;
- l'en-tête ne disparaît pas au défilement si la barre fixe n'est pas encore visible.

---

## Synthèse du moodboard : 3 directions possibles

Les 3 directions sont maintenues. Trois ajustements, justifiés par ce qui a été vu : le bandeau France Rénov' devient obligatoire (n° 23), la carte réalisation suit le modèle NSH en production (n° 25), et le repoussoir PAC est corrigé (n° 17). Les références citées sont celles qui ont été capturées.

**A. « Atelier » (recommandée)**
Fond blanc chaux, titres Fraunces en vert sapin, rouge basque réservé aux CTA, photos réelles chaudes (bois, laine, mains).
Les avant/après sont la colonne vertébrale de la page, et les labels numérotés apparaissent comme des tampons.
Références : l'équipe et le label dans la photo (Aira, n° 1), la PAC posée dans un vrai intérieur et la serif chaleureuse (Quilt, n° 18), la carte avant/après en production (NSH, n° 25).
Sensation : un artisan fier de son travail, local et vérifiable.

**B. « Etxe » (maison basque)**
Grands aplats rouge profond et vert sapin, comme les colombages, avec un motif discret inspiré des linteaux sculptés.
Très identitaire et mémorable, mais il y a un risque de folklore et de contraste fort à maîtriser. Le rouge en aplat rappellerait aussi les marques de PAC (Immergas, Calorex, n° 17).
À garder pour le pied de page et les séparateurs.

**C. « Carnet de chantier »**
Mise en page de journal de bord : dates, étapes numérotées, photos en planche contact, notes manuscrites légères.
Excellent pour le déroulé en 5 étapes et la transparence (le bloc « le chantier en bref » d'Aira, n° 10, les numéros de projet de PRB, n° 14).
Moins direct pour la conversion : il faut la barre mobile fixe.

## Palette recommandée (direction A)

Inchangée : rien dans les observations ne justifie de la modifier. Les contrastes, qui étaient « à vérifier », sont maintenant calculés.

| Rôle | Hex | Usage |
|---|---|---|
| Blanc chaux | `#F6F1E7` | Fond principal |
| Chaux claire | `#FBF8F2` | Cartes, estimateur |
| Rouge basque profond | `#9E1B22` | CTA, accents, numéros d'étapes. Blanc sur rouge : 8,0:1. Rouge sur chaux : 7,1:1 |
| Vert sapin | `#1F4A37` | Titres, barre mobile, fonds sombres. Sur chaux : 8,9:1 |
| Bois | `#B98A5A` | Filets, icônes, pastilles (jamais en texte sur chaux : 2,7:1) |
| Bois foncé | `#7A5534` | Texte décoratif sur fond clair si besoin (5,9:1) |
| Encre | `#1E1A17` | Texte courant (15,4:1) |

Les couleurs DPE (étiquette A à G) servent **uniquement** aux badges de classe énergie, jamais à la décoration.

## Polices (Google Fonts)

- **Fraunces** (variable, axes optique et « soft ») : titres, graisses 600 à 700, réglage « soft » modéré pour un rendu chaleureux.
- **Source Sans 3** : texte courant, très lisible pour les seniors. Alternative : **Public Sans**.
- **Fraunces italique** : citations d'avis clients, et éventuellement la seconde ligne du H1, comme le fait NSH (n° 25) avec une sans et une serif italique.
- Relevé chez les autres : airaText, police maison (Aira), buenos-aires (Effy), Lexend (Hellio), Barlow Condensed (FTCC), Inter et une serif système en italique (NSH), « Quilt Serif » et « Quilt Sans » (Quilt). Rien ne justifie de changer : Quilt et NSH montrent qu'une serif chaleureuse fonctionne dans le secteur.

## 3 « à ne pas faire »

1. **Pas de codes de démarchage** : pas de compte à rebours, de « PAC à 1 € », de pop-up « on vous rappelle », de bandeau défilant « -10 % » (vu chez Wambreck, n° 21) ni de prime en très gros caractères (Immergas, n° 17).
2. **Pas de banque d'images ni d'allégation verte** : pas de famille souriante sur canapé, de maison miniature dans une main (n° 9), de salon mis en scène (n° 19), de PAC en rendu 3D. Pas de « écologique » (n° 21).
3. **Pas de logos sans preuve** : ni RGE ou Qualibat sans numéro et sans lien de vérification (mur de logos d'Aira, n° 1), ni logos de fournisseurs présentés comme une caution (NSH, n° 25), ni avis filtrés « 4 et 5 étoiles » (Aira, n° 1).

---

## Design tokens (direction A, « Atelier »)

### Couleurs

| Token | Hex | Usage |
|---|---|---|
| `color.brand.primary` | `#9E1B22` | Rouge basque : bouton primaire, numéros d'étapes |
| `color.brand.primary-hover` | `#821519` | Survol du primaire |
| `color.brand.secondary` | `#1F4A37` | Vert sapin : titres, barre mobile, bouton secondaire |
| `color.brand.secondary-hover` | `#173A2B` | Survol |
| `color.brand.wood` | `#B98A5A` | Filets, icônes, pastilles décoratives |
| `color.brand.lime` | `#F6F1E7` | Blanc chaux, fond principal |
| `color.brand.lime-light` | `#FBF8F2` | Cartes, estimateur |
| `color.semantic.success` | `#2E6B3F` | Demande envoyée, éligible |
| `color.semantic.error` | `#B3261E` | Erreur de champ : toujours avec une icône, pour ne pas se confondre avec le rouge de marque |
| `color.semantic.warning` | `#A15C00` | Hors zone, barème à confirmer |
| `color.semantic.info` | `#2D5C7A` | Mentions sur les aides, infobulles |
| `color.neutral.900` | `#1E1A17` | Texte courant |
| `color.neutral.700` | `#4A433D` | Texte secondaire |
| `color.neutral.500` | `#857A70` | Légendes |
| `color.neutral.300` | `#D8CFC3` | Bordures |
| `color.neutral.100` | `#EFE8DC` | Fonds alternés |
| `color.neutral.0` | `#FFFFFF` | Champs |
| `color.dpe.a` … `color.dpe.g` | reprendre l'étiquette officielle | Badges DPE uniquement |

Contrastes calculés (WCAG 2.1), sur `#F6F1E7` sauf mention :
- blanc sur `#9E1B22` : 8,0:1 ; blanc sur `#821519` : 10,1:1 ;
- `#1E1A17` : 15,4:1 ; `#1F4A37` : 8,9:1 ; `#4A433D` : 8,6:1 ;
- `#2E6B3F` : 5,7:1 ; `#2D5C7A` : 6,4:1 ; `#A15C00` : 4,6:1 (juste au-dessus du seuil) ; `#B3261E` sur blanc : 6,5:1 ;
- **`#857A70` : 3,7:1**, insuffisant pour un texte de moins de 24 px. Les légendes en `type.small` (15 px) passent en `neutral.700` ; `neutral.500` reste pour les gros textes et les éléments non textuels ;
- `#B98A5A` : 2,7:1, jamais en texte.

### Typographie (base 17 px pour le public senior)

| Token | Police | Taille (desktop / mobile) | Graisse | Interligne |
|---|---|---|---|---|
| `type.display` | Fraunces | 72 / 40 px | 700 | 1.05 |
| `type.h1` | Fraunces | 52 / 34 px | 650 | 1.1 |
| `type.h2` | Fraunces | 38 / 28 px | 600 | 1.15 |
| `type.h3` | Fraunces | 24 / 21 px | 600 | 1.25 |
| `type.quote` (avis) | Fraunces italique | 22 / 19 px | 400 | 1.45 |
| `type.body-lg` | Source Sans 3 | 20 / 19 px | 400 | 1.6 |
| `type.body` | Source Sans 3 | 18 / 17 px | 400 | 1.65 |
| `type.small` | Source Sans 3 | 15 px | 500 | 1.5 |
| `type.label` (champs, badges) | Source Sans 3 | 16 px | 600 | 1.3 |

### Espacement (base 4 px)
`space.1` 4 · `space.2` 8 · `space.3` 12 · `space.4` 16 · `space.5` 24 · `space.6` 32 · `space.7` 48 · `space.8` 64 · `space.9` 96 · `space.10` 120 px.
Section : 120 px desktop, 64 px mobile. Marge latérale mobile : 16 px. Barre mobile fixe : 72 px de haut, avec une réserve `padding-bottom` équivalente.

### Rayons
`radius.sm` 4 px (champs) · `radius.md` 10 px (boutons) · `radius.lg` 18 px (cartes, photos) · `radius.full` 999 px (badges DPE, pastilles labels).
Des angles doux pour un registre artisanal.

### Ombres
- `shadow.none` : par défaut.
- `shadow.sm` : `0 1px 3px rgba(30,26,23,.10)` (cartes).
- `shadow.md` : `0 6px 20px rgba(30,26,23,.12)` (estimateur, barre mobile).
- `shadow.focus` : `0 0 0 3px #1F4A37, 0 0 0 5px #F6F1E7` (focus, double anneau).

### Motion
- Durées : `motion.fast` 120 ms (survol) · `motion.base` 220 ms (étapes de l'estimateur, accordéons) · `motion.slow` 350 ms (apparition du résultat) · curseur avant/après sans inertie (suit le doigt).
- Easings : `ease.standard` `cubic-bezier(.2,0,0,1)` · `ease.enter` `cubic-bezier(0,0,0,1)` · `ease.exit` `cubic-bezier(.3,0,1,1)`.
- `prefers-reduced-motion` : pas d'animation d'apparition, curseur avant/après remplacé par deux images côte à côte si l'utilisateur le souhaite.

## Composants clés

- **Bouton primaire** (« Demander une visite gratuite ») : fond `brand.primary`, texte `#FFFFFF`, `radius.md`, hauteur 52 px.
  - Survol : `primary-hover`. Focus : `shadow.focus`. Actif : enfoncé de 1 px.
  - Désactivé : fond `neutral.300` et texte `neutral.700`, avec l'explication sous le bouton.
  - Chargement : « Envoi… » et spinner, largeur fixe.
- **Bouton secondaire** (« Appeler l'atelier ») : contour de 2 px `brand.secondary`, texte vert sapin, icône téléphone.
  - Survol : fond `neutral.100`. Mêmes états que le primaire.
  - **Dans la barre mobile** : fond `brand.secondary` plein, texte chaux, au moins 48 px de haut (l'icône de 31 px d'Aira est trop petite).
  - Les horaires d'appel sont écrits à côté du numéro sur desktop (idée vue chez Wambreck, n° 21).
- **Carte réalisation** (modèle NSH, n° 25) : curseur avant/après avec `role="slider"`, `aria-label` (« Comparer avant et après, maison de 1975 à Anglet »), flèches clavier par pas de 5 %, poignée de 44 px.
  - Étiquettes « Avant » et « Après » toujours visibles dans les coins.
  - Photos avant et après du même point de vue (n° 26).
  - Puis badges DPE avant → après, commune, travaux, durée, extrait d'avis en `type.quote`, et le bloc « le chantier en bref » d'Aira (n° 10).
  - Filtres par travaux au-dessus de la grille (isolation, PAC, menuiseries, rénovation globale).
- **Carte label** : logo, nom de la qualification, numéro, domaine, date de validité, lien « Vérifier » vers l'annuaire France Rénov' (n° 24).
- **Bandeau France Rénov'** (obligatoire depuis le 1er octobre 2026, n° 23) : le bandeau officiel tel que fourni dans le kit, sans le redessiner, en pied de page et près du résultat de l'estimateur. Emplacement à valider par un juriste.
- **Formulaire / estimateur** :
  - une question par écran sur mobile, avec une barre de progression et l'étape nommée (« 1/4 Votre logement », comme Effy, n° 5) ;
  - libellés visibles et aide en `type.small` ;
  - tranches de revenus en boutons radio (jamais un champ libre) ;
  - résultat annoncé par `aria-live`, en très grand, la mention collée dessous (n° 6) ;
  - mention « indicatif, barème du JJ/MM/AAAA » collée au montant.

| À faire | À ne pas faire |
|---|---|
| Afficher le résultat de l'estimateur avant de demander un contact | Bloquer le résultat derrière le numéro de téléphone |
| Une fourchette datée, avec « sous réserve d'éligibilité » | « Jusqu'à 11 000 € d'aides pour vous ! » |
| Labels avec numéro et lien de vérification | Mur de logos sans preuve, logos de fournisseurs |
| Les mêmes chiffres partout (chantiers, avis), tirés d'une seule source | « 80+ projets » en haut et « 150 clients » plus bas (n° 25) |
| Tous les avis, avec un lien vers la fiche Google | Un carrousel « nos avis 4 et 5 étoiles » (n° 1) |
| Le bandeau France Rénov' officiel | L'oublier : amende jusqu'à 75 000 € (n° 23) |
| Erreur en texte et icône (ce qui s'est passé, pourquoi, comment corriger), en `semantic.error` distinct du rouge de marque | Erreur signalée uniquement par une bordure rouge |
| Boutons d'au moins 48 px et texte de 17 px ou plus | Petits liens gris « rappel gratuit », icône téléphone de 31 px |
| Rouge réservé à l'action principale | Rouge partout (titres, fonds, icônes) |
| Photos réelles de chantiers et d'équipe, avant et après du même point de vue | Banque d'images, rendus 3D de PAC |
