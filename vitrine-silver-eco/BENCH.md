# Benchmark visuel : Les Jours Tranquilles (silver économie / aide à domicile)

> **Les Jours Tranquilles est fictive.** Les références sont réelles. Les URL d'origine viennent de résultats de recherche (novembre 2026), les références ajoutées ont été ouvertes le 2026-11-12.

## Limites, à lire en premier

- **Sites ouverts et capturés le 2026-11-12**, dans un navigateur Chrome piloté (viewport 1440×900, au-dessus de la ligne de flottaison, et 390×844 pour le mobile). Les captures sont dans [`captures/`](captures/). Les couleurs et les polices citées ont été relevées dans la page (styles calculés), pas devinées. Les contrastes sont recalculés selon la formule WCAG 2.1.
- **12 références sur 16 vues et capturées**, dont 2 épingles Pinterest seulement en partie (n° 11 et 15 : le mur de connexion assombrit la page, seule une zone reste lisible). **4 inaccessibles**, aucune protection n'a été contournée :
  - n° 6 et 10 (Behance) : erreur HTTP 400 renvoyée au navigateur automatisé. Elles sont **remplacées** par deux shots Dribbble ouverts (n° 6 bis et 10 bis). Le n° 10 bis porte exactement le titre du projet Behance cité.
  - n° 14 (Pinterest) : **épingle supprimée**. L'URL redirige vers la page « ideas » et l'identifiant seul mène à l'accueil.
  - n° 16 : Land-book affiche un challenge Cloudflare, Lapa Ninja « Sorry, you have been blocked ».
- **Corrections importantes** (détail dans chaque ligne) :
  - **Petits-fils (n° 4)** : la page citée ne parle ni des 3 ans d'expérience, ni d'auxiliaire attitrée, ni de prix. Les critères de recrutement sont sur une autre page, les tarifs dans une grille par agence. Et Petits-fils travaille en **mode mandataire** (la famille est l'employeur), l'inverse de notre modèle.
  - **Cera (n° 5)** : l'URL redirige vers Home Healthcare Connected. Le régulateur (CQC) n'est pas cité. L'application famille est décrite en texte, sans aucun visuel.
  - **O2 (n° 8)** : la visite et le devis gratuits sont confirmés. Le « contrat résiliable sans frais » et la « remplaçante en cas d'absence » n'apparaissent pas sur la page.
  - **O2 (n° 13)** : l'URL redirige. Sur mobile, aucun numéro en haut : une barre fixe en bas à 3 icônes, dont le combiné ouvre une demande de rappel et non un appel.
  - **Home Instead (n° 7)** : le process compte 7 étapes non numérotées, pas 4.
  - **Dribbble (n° 9)** : 245 shots, pas environ 170. Le téléphone de Birdie affiche une alerte de chute, pas un compte-rendu de visite.
  - **« À ne pas faire » n° 3** : le texte blanc sur `#C8775A` est à 3,4:1 (3,1:1 est le contraste de `#C8775A` sur le crème). La règle ne change pas.
- **7 références ajoutées** (5 Dribbble, 1 Awwwards, 1 site réel), numérotées 6 bis, 10 bis et 17 à 21. One Page Love ne contient aucun site d'aide aux seniors, Godly redirige vers recent.design et ThemeForest (pour retrouver le thème du n° 11) bloque par Cloudflare. Le détail est en fin de section « Références ajoutées ».
- Aucun formulaire n'a été rempli ni envoyé. Sur Dribbble, les avatars et les noms de designers ont été masqués avant la capture. Les personnes visibles sont celles des photos publiées par les entreprises.

**Répartition** : 16 entrées d'origine (17 URL) et 7 ajoutées. Sites réels 8, Dribbble 7 (dont 1 page de tag), Pinterest 3, Behance 2 (inaccessibles), One Page Love 1, Awwwards 1, Land-book et Lapa Ninja 1 (inaccessibles, regroupés dans l'entrée 16).

---

## Hero

| # | Titre | Source | URL | Capture | À retenir |
|---|---|---|---|---|---|
| 1 | Honor, « Quality of life has no expiration date » | Site réel (US) | https://www.honorcare.com/home-care/ | [capture](captures/01-honor-home-care.jpg) | Fond pêche `#FFF6F0`, accroche en Plus Jakarta Sans 400, 38 px, orange `#E76124` (3,2:1 : acceptable en grand texte seulement). Pas de H1 : le titre est une simple div. Un seul bouton « Find home care », blanc sur brun `#662A12` (11,0:1), et à droite une photo de deux hommes âgés qui rient, dans un cadre arrondi. Texte courant brun `#662A12`. Aucun numéro de téléphone sur la page. Honor est aussi la maison mère de Home Instead (n° 7). **À reprendre** : le ton digne, et le duo fond clair chaud + CTA brun foncé, très proche de notre crème + terracotta foncée. **À éviter** : un titre orange clair à 3,2:1, et une page sans numéro. |
| 2 | Agedly, a Home Care Service for Seniors Landing Page (Animated), 10am Studio | Dribbble | https://dribbble.com/shots/16641466-Agedly-a-Home-Care-Service-for-Seniors-Landing-Page-Animated | [capture](captures/02-dribbble-agedly.jpg) | Vidéo de 30 s (image de départ capturée). Hero blanc, H1 en grotesque grasse « We Provide Home Care Services for Seniors », « Seniors » en rouge, un champ code postal et un bouton rouge « Get Started ». La photo montre une soignante en blouse qui enlace une dame en fauteuil roulant. Plus bas, une bande bleu nuit et un gros plan de mains sur une canne. **À reprendre** : un seul champ ou un seul bouton dans le hero. **À éviter** : fauteuil roulant, mains sur la canne, blouse médicale : exactement les codes de dépendance que le brief exclut. L'animation reste à proscrire. |
| 3 | Ouihelp, landing « aide à domicile de confiance » | Site réel (FR) | https://lp.ouihelp.fr/l/aide-domicile-confiance | [capture](captures/03-ouihelp-landing.jpg) | Pas de menu : le logo et le numéro « 01 89 72 41 76, numéro gratuit ». Hero photo sur fond bleu, H1 blanc « Aide à domicile de confiance » en Source Sans Pro 700, 38 px, sous-titre en 14 px blanc (« disponible en 48h »). Bouton-pilule vert `#3ED096` avec le numéro, texte bleu nuit `#002C5A` (7,1:1). Deux pastilles : « Plus de 35 000 familles accompagnées depuis 2016 » et « Plus de 100 agences partout en France ». À droite, une carte « Je souhaite échanger avec un conseiller » : 4 champs (nom, téléphone, code postal, e-mail) et 2 cases de consentement, **la première déjà cochée**. Sous le hero : Certifié SAD, chèques CESU, avance immédiate, Google 4,5/5 et plus de 2400 avis. **À reprendre** : le numéro en gros bouton dans le hero, et la ligne de 4 preuves juste dessous. **À éviter** : la case de consentement pré-cochée (non conforme au RGPD), 4 champs au lieu de 2, du texte en 14 px blanc sur photo. |

## Réassurance et preuves

| # | Titre | Source | URL | Capture | À retenir |
|---|---|---|---|---|---|
| 4 | Petits-fils, nos services d'aide à domicile | Site réel (FR) | https://www.petits-fils.com/nos-services-aide-a-domicile/ | [services](captures/04-petits-fils-services.jpg), [tarifs](captures/04-petits-fils-tarifs.jpg) | H1 « Aide à domicile : nos services » en Montserrat 700, 38 px, cyan `#27CDE8` sur blanc (1,9:1). Encart bleu `#0067DA` « Rappel immédiat, dans les 2 heures ouvrables » avec un bouton orange `#EF7D00` (texte blanc 2,8:1). Note « 4.5/5 (12942 avis) » en haut de page, services en 4 blocs à pastille de couleur, illustration d'une dame dans un fauteuil. **Correction** : cette page ne mentionne ni les 3 ans d'expérience, ni l'auxiliaire attitrée, ni de prix (seulement un bouton « Demander les tarifs »). Les critères sont sur la page https://www.petits-fils.com/auxiliaires-de-vie/ : formation qualifiante ou certification Croix-Rouge, 3 ans d'expérience minimum, 3 références vérifiées. Les tarifs sont publiés par agence (https://www.petits-fils.com/tarifs-petits-fils/, puis choix d'une agence) : à Bordeaux Chartrons, 35,50 € TTC de l'heure jusqu'à 25 h par semaine, et une colonne « Coût indicatif réel après crédit d'impôt » à 17,75 € (seconde capture). Petits-fils travaille en **mode mandataire**. Incohérences : « 275 agences » en pied de page contre « 330+ agences » sur la page agence, et « Accessibilité : Non conforme » en pied de page. **À reprendre** : la colonne « coût réel après crédit d'impôt » dans le tableau des tarifs, et des critères de recrutement chiffrés. **À éviter** : le cyan et l'orange pour du texte, l'en-tête de tableau blanc sur jaune `#F9AE00` (1,9:1). |
| 5 | Cera, Care at Home | Site réel (UK) | https://ceracare.co.uk/home-care | [capture](captures/05-cera-home-care.jpg) | **Redirigée** vers https://homehealthcareconnected.co.uk/home-care (Home Healthcare Connected). Bannière rose à cœurs dessinés, H1 « Home Care » en Kinder Boy (police manuscrite), violet `#76299B` (8,2:1), une auxiliaire en blouse violette avec un monsieur âgé. Texte en Lato. **Correction** : le CQC n'est pas cité sur la page. La « Family App » tient en une phrase et une puce (planning, notes de visite, état de santé), sans capture d'écran. Le lien téléphone est cassé (`tel:"0330 123 9180"`, guillemets compris). **À reprendre** : l'idée « chaque visite est enregistrée et visible par la famille ». **À éviter** : un titre en police manuscrite, les cœurs dessinés, une promesse « famille » sans montrer à quoi elle ressemble. |
| 6 | Senior care branding (dont « Seniare – Brand Identity & UI/UX Design for Homecare ») | Behance (page de recherche) | https://www.behance.net/search/projects/senior%20care%20branding | inaccessible | **Inaccessible (erreur HTTP 400)**, non vérifié. D'après la session précédente : identités de marque pour l'aide à domicile, Seniare étant le projet le plus vu. Aucun shot « Seniare » sur Dribbble. Remplacée par le n° 6 bis. |
| 6 bis | AgeFree, Elder Care Branding and Identity Design (Techwitpro) | Dribbble | https://dribbble.com/shots/27547230-AgeFree-Elder-Care-Branding-and-Identity-Design | [capture](captures/06-dribbble-agefree.jpg) | Planche d'identité : vert sapin, crème, orange et jaune doux. Logo serif « AgeFree » avec un pictogramme de deux personnes, slogan « Respect. Support. Smile. ». Une carte « Dignity in every moment », des pastilles de services à icône au trait (Free Consultation, Daily Support, Home Visits…), une affiche « Helping elders live with dignity and joy » avec la fin en italique orange. **À reprendre** : l'accord vert profond + crème + orange, cousin de notre olive + crème + terracotta, et les pastilles de service à icône au trait. **À éviter** : les silhouettes à canne au coucher de soleil, et le mot « elders » (l'équivalent de « nos aînés », interdit par le brief). |

## Parcours (comment ça se passe)

| # | Titre | Source | URL | Capture | À retenir |
|---|---|---|---|---|---|
| 7 | Home Instead, « Our process to provide quality senior care » | Site réel (US) | https://www.homeinstead.com/location/782/home-care-services/our-process-to-provide-quality-senior-care/ | [hero](captures/07-home-instead-process.jpg), [étapes](captures/07-home-instead-etapes.jpg) | **Redirigée** vers la page de l'agence de St Charles (Missouri). Hero en deux moitiés : photo d'une auxiliaire en polo vert qui montre un vase à une dame, et aplat bleu clair `#D3ECFF` avec le H1 « Creating the Right Care Plan » en PP Editorial New (serif), 48 px, vert foncé `#2C4F26` (7,6:1). Fond de page crème `#FAFFEE`, texte `#2C4F26` (9,1:1) en Plus Jakarta Sans. Dans l'en-tête, le numéro en pilule blanche et « Get Started » sur vert anis `#DEED6A` (7,3:1). **Correction** : le process compte 7 étapes (besoins, actes du quotidien, pistes d'aide, sécurité du logement, isolement, plan de coordination, recommandations), en liste à icônes, non numérotées. La page finit sur « Honor Family App » : 6 puces (« Get a comprehensive update after every visit »…), sans visuel. Deux numéros différents : (636) 477-6025 en en-tête, (636) 206-4199 en pied de page. **À reprendre** : le serif éditorial vert foncé sur fond crème, la pilule téléphone dans l'en-tête. **À éviter** : 7 étapes sans numéro (on garde 4 étapes numérotées), deux numéros sur la même page. |
| 8 | O2, la méthode O2 | Site réel (FR) | https://www.o2.fr/aide-aux-personnes-agees/selon-o2/la-methode-o2 | [hero](captures/08-o2-methode.jpg), [avis](captures/08-o2-methode-avis.jpg) | Hero bleu `#005CB9`, H1 blanc « La Méthode O2 Faire Ensemble » en MontBold, 59 px (6,5:1), photo d'une dame âgée et d'une jeune femme qui regardent un album. Bandeau « Choisir O2 c'est » : 5 engagements à icône au trait (continuité de service, auxiliaires salariés et formés, accompagnement sur mesure, démarches administratives, coordination médicale). Puis « 4,7/5 sur 589 avis Google récoltés entre le 01/03/2026 et le 31/03/2026 ». La méthode écrit en toutes lettres « Ne pas infantiliser la personne ». **Correction** : « visite gratuite et sans engagement » et « devis personnalisé, gratuit et sans engagement » sont bien écrits. Le contrat résiliable sans frais et la remplaçante en cas d'absence n'y sont pas. **À reprendre** : la note avec le nombre d'avis et la période de collecte (bon modèle pour l'information sur les avis), et les micro-réassurances sous le CTA. **À éviter** : le H2 vert `#00BFA2` sur blanc (2,3:1). |

## Lien famille, services et cartes

| # | Titre | Source | URL | Capture | À retenir |
|---|---|---|---|---|---|
| 9 | Elderly care tag (dont « Birdie Family Landing Page », Koncepted) | Dribbble | https://dribbble.com/tags/elderly-care | [tag](captures/09-dribbble-elderly-care.jpg), [Birdie](captures/09-dribbble-birdie-famille.jpg) | **Correction** : 245 shots, pas environ 170. La première page mélange des sites (Agewise, CareHaven, Agedly), une illustration de robot qui aide une dame à traverser et un logo sans rapport. Les 3 shots Birdie sont plus bas ; le plus utile est https://dribbble.com/shots/5413993-Birdie-Family-Landing-Page. On y voit un hero photo mère et fille, un CTA turquoise, le téléphone dans l'en-tête, puis un téléphone qui affiche « Fall detected in the living room » à côté de « Wellbeing reports, live updates after every visit », et des formules à 49,99 £. **À reprendre** : la maquette de téléphone à côté d'une courte liste de bénéfices. **À éviter** : une alerte de chute comme exemple de message. Notre compte-rendu doit rassurer (« Repas préparé, courses faites »), pas alerter. |
| 10 | Home care website (dont « Senior Care Website Redesign \| Healthcare UI/UX Project ») | Behance (page de recherche) | https://www.behance.net/search/projects/home%20care%20website | inaccessible | **Inaccessible (erreur HTTP 400)**, non vérifié. Un projet du même titre existe sur Dribbble : voir le n° 10 bis. |
| 10 bis | Senior Care Website Redesign \| Healthcare UI/UX Project (Orbillo) | Dribbble | https://dribbble.com/shots/27644508-Senior-Care-Website-Redesign-Healthcare-UI-UX-Project | [capture](captures/10-dribbble-senior-care-redesign.jpg) | Refonte d'un site d'aide à domicile (« A Day After Day Home Care »). Hero bleu nuit, photo d'une soignante en blouse bleue et d'une dame qui sourient, H1 « Compassionate Home Care Your Loved One Deserves » avec la fin en serif italique. Au-dessus, une pastille « BBB Accredited · A+ Rated · Serving Indiana & Ohio ». CTA vert anis « Get A Free Care Assessment » et le numéro en lien texte juste à côté. Dessous, fond crème, « Personalized Care For Every Need » et 3 cartes photo. **À reprendre** : la pastille preuves + zone au-dessus du H1, le numéro à côté du CTA, un mot en serif italique. **À éviter** : la blouse médicale (on vend de l'aide à domicile, pas du soin). |

## Accessibilité et lisibilité

| # | Titre | Source | URL | Capture | À retenir |
|---|---|---|---|---|---|
| 11 | Eldcare, Senior Living WordPress Theme | Pinterest | https://www.pinterest.com/pin/973340538222802684/ | [capture partielle](captures/11-pinterest-eldcare.jpg) | Mur de connexion : seule la vignette de l'épingle reste lisible, assombrie. Thème vert sapin et jaune moutarde, « Best senior care with love », photos de seniors qui s'enlacent. La description confirme « warm, accessible design that conveys trust, compassion ». La fiche du thème n'a pas pu être ouverte (ThemeForest bloque par Cloudflare) : **contrastes non vérifiables**. **À retenir** : même famille que le n° 6 bis, vert profond et accent chaud. |
| 12 | Health & Healthcare Website Examples | One Page Love | https://onepagelove.com/tag/health | [capture](captures/12-onepagelove-health.jpg) | « 78 Real Examples ». Les premiers : chirurgie, IA, logiciel de santé, appli d'aide à l'arrêt de l'alcool (SafeStep), dentiste. Aucun service d'aide aux seniors, et les recherches « senior », « elderly », « home care » et « retirement » sur le site ne donnent rien de pertinent. **À retenir** : peu utile pour notre secteur, sauf pour la longueur de page. Les n° 17 à 19 sont plus proches. |

## Mobile

| # | Titre | Source | URL | Capture | À retenir |
|---|---|---|---|---|---|
| 13 | O2, aide à domicile des personnes âgées | Site réel (FR) | https://www.o2.fr/aide-aux-personnes-agees/aide-a-domicile | [desktop](captures/13-o2-aide-a-domicile.jpg), [mobile](captures/mobile-o2.jpg) | **Redirigée** vers https://www.o2.fr/aide-aux-personnes-agees. Desktop : hero bleu `#005CB9`, H1 « Aide à domicile pour les personnes âgées » en MontBold sur deux graisses, « plus de 92 000 familles » depuis 1996, grand bouton « Obtenir un devis · Gratuit & sans engagement » en blanc sur jaune `#E7BA63` (1,8:1). Le seul lien `tel:` (02 43 72 02 02) est dans le pied de page. Mobile : voir ci-dessous. **À éviter** : du texte blanc sur jaune clair, et le numéro relégué en pied de page. |

**Observé en 390×844**

| Site | Capture | Ce qu'on observe |
|---|---|---|
| O2 | [capture](captures/mobile-o2.jpg) | Un bandeau « Espace Salarié · Espace Client », puis un en-tête de 80 px (menu, logo, compte). Aucun numéro en haut. Une barre fixe en bas, 50 px, en 3 aplats à icône seule (agence, être rappelé, rendez-vous pour une visite) : les libellés existent dans le code mais ne s'affichent pas, et le combiné mène à une page de rappel, pas à un appel. Le bouton d'accessibilité chevauche le bouton devis. Le seul lien `tel:` est tout en bas de page. |
| Ouihelp | [capture](captures/mobile-ouihelp.jpg) | En-tête collant de 64 px avec un bouton vert à icône de rappel (lien `#`, sans libellé accessible). Le lien `tel:` de l'en-tête est masqué sur mobile. Dans le hero, le numéro en grand bouton vert (vrai lien `tel:`), puis « Être rappelé » en blanc. L'accroche est en 14 px blanc sur photo. Le formulaire n'est pas au premier écran. |
| Petits-fils | [capture](captures/mobile-petits-fils.jpg) | Le bandeau « À la recherche d'un emploi ? » occupe la première ligne. Aucun numéro, ni dans l'en-tête ni ailleurs sur la page. Le premier appel à l'action est l'encart « Rappel immédiat » (bouton orange). La note 4,5/5 visible sur desktop disparaît. |

**À retenir** : aucun des 3 sites ne met un numéro cliquable en haut de l'écran mobile. Les deux qui proposent une action fixe poussent la demande de rappel, pas l'appel. Le numéro en haut de chaque écran, demandé par le brief, est donc un vrai différenciant. Recommandations, confirmées par ces observations :
- une barre d'appel fixe en haut, avec le numéro **écrit en clair** et le libellé « Appeler », jamais une icône seule (contrairement à O2) ;
- un seul numéro, identique partout, en vrai lien `tel:` (Home Instead en affiche deux, n° 7 ; celui de Home Healthcare Connected est cassé, n° 5) ;
- le formulaire de rappel en 2 champs, sans case pré-cochée (contrairement à Ouihelp, n° 3) ;
- un corps de texte d'au moins 18 px, y compris sur photo et avec un voile (Ouihelp descend à 14 px).

## Palette et typographie

| # | Titre | Source | URL | Capture | À retenir |
|---|---|---|---|---|---|
| 14 | Elderly Care Wix Studio Website Template | Pinterest | https://in.pinterest.com/pin/elderly-care-wix-studio-website-template-inhome-caregiver-senior-care-assisted-living-nursing-homes-in-2025--4602749301043693056/ | inaccessible | **Inaccessible : épingle supprimée** (redirection vers https://in.pinterest.com/ideas/). Non vérifié. D'après la session précédente : décrit comme « warm, trustworthy », couleurs douces. Remplacée pour l'ambiance par les n° 6 bis et 17. |
| 15 | 12 Assisted Living Website Themes ideas | Pinterest (tableau) | https://www.pinterest.com/cricketpond/assisted-living-website-themes/ | [capture partielle](captures/15-pinterest-assisted-living.jpg) | Mur de connexion, une colonne reste lisible. Tableau de 12 épingles créé il y a 9 ans (« Mix of templated themes »). On y voit les clichés attendus : gros plans de visages de seniors souriants, équipes en blouse, bandeaux verts et bleus. **Confirmé** : sert à repérer les clichés **pour s'en écarter**. |
| 16 | Health & fitness, galeries filtrables par couleur | Land-book et Lapa Ninja | https://land-book.com/?industry=health-and-fitness et https://www.lapa.ninja/category/health-fitness/ | inaccessible | **Inaccessibles (protection anti-robots)** : challenge Cloudflare persistant sur Land-book, « Sorry, you have been blocked » sur Lapa Ninja. Non vérifié. Les associations crème et terracotta en contexte réel ont été vues ailleurs : Honor (n° 1), Home Instead (n° 7), The Legacy (n° 20). |

---

## Références ajoutées (vues le 2026-11-12)

Requêtes Dribbble : « senior care branding », « home care website », « senior care website », « seniare ». Requêtes Awwwards : « senior », « home care », « elderly ». Les URL sont celles des pages réellement ouvertes.

| # | Titre | Source | URL | Capture | À retenir |
|---|---|---|---|---|---|
| 17 | Family Caregiver Mobile iOS App Design (Purrweb UI/UX Agency) | Dribbble | https://dribbble.com/shots/27740425-Family-Caregiver-Mobile-iOS-App-Design | [capture](captures/17-dribbble-family-caregiver-app.jpg) | Fond olive, titre serif « Care, in relay. », application sombre où la famille se répartit les tâches : « 3/4 care actions covered », « Leo checked in », « Call Mom · 6:30 PM ». **À reprendre** : la carte de résumé de journée (qui est passé, à quelle heure), et l'accord olive + serif, qui valide notre olive. **À éviter** : afficher des médicaments ou des données de santé ; le site n'en collecte aucune. |
| 18 | Sincere In-Home Care, Landing Page Design (Brandframer.com) | Dribbble | https://dribbble.com/shots/27743802-Sincere-In-Home-Care-Landing-Page-Design | [capture](captures/18-dribbble-sincere-in-home-care.jpg) | Fond crème, H1 sans-serif noir, sous-titre vert « The care you need for the life you want. », pastille « Locally owned & family operated ». Le numéro en pilule verte dans l'en-tête, puis 2 boutons : « Call for Care » plein et « Request a Consultation » bordé, et dessous « Speak with a real person: (661) 888-4908 ». Photo naturelle d'une auxiliaire et d'une dame dans un salon. **À reprendre** : la hiérarchie claire (une action pleine, une bordée, le numéro répété en clair) et la formule « parlez à une vraie personne ». C'est le meilleur modèle pour le hero de la direction C. |
| 19 | CareHaven, Senior Care & Home Assistance Website Design (Trexa Lab) | Dribbble | https://dribbble.com/shots/27047677-CareHaven-Senior-Care-Home-Assistance-Website-Design | [capture](captures/19-dribbble-carehaven.jpg) | Hero vert très foncé, H1 « Your Parents Smile. Matters right? », note « 4.9/5 · 810+ Reviews » au-dessus, CTA jaune-vert « Find Your Caregiver Today », numéro en pilule dans l'en-tête. Chiffres « 3,200+ », « 5k% », « 97.5% », puis des logos Slack et Dropbox. **À reprendre** : parler des parents dès le H1 (comme « Vos parents chez eux, bien entourés »), la note au-dessus du titre. **À éviter** : un chiffre absurde (« 5k% ») et des logos de marques tech sans rapport : ça détruit la confiance. |
| 20 | The Legacy Senior Communities (Tegan Digital), Honorable Mention du 24 septembre 2021 | Awwwards | https://www.awwwards.com/sites/the-legacy-senior-communities | [capture](captures/20-awwwards-legacy-senior.jpg) | La version primée : logo serif, titre serif blanc sur photo de jardin (« Reinventing Senior Living »), un couple de seniors actifs qui marchent main dans la main, bouton « Call now » bordé. Palette relevée par Awwwards : `#2779A7`, `#DF6C4F` (un orangé cousin de notre terracotta douce) et blanc. C'est un lieu de vie, pas de l'aide à domicile. **À reprendre** : des seniors actifs plutôt que dépendants, un serif fin pour l'émotion. |
| 21 | The Legacy Senior Communities (site actuel) | Site réel (US) | https://thelegacyseniorcommunities.org/ | [capture](captures/21-legacy-senior-site.jpg) | Le site a changé depuis le prix : H1 « Luxury Senior Living in Dallas, TX » (la ville dans le H1) en Cormorant 600, 65 px, blanc sur photo ; texte en Work Sans 18 px ; bouton « Get in touch » blanc sur bleu nuit `#141C3B` (16,7:1) ; badge « Safest places to live 2026 ». Une rubrique « The Legacy at Home ». **À reprendre** : la ville dans le H1 (SEO local du brief), le corps à 18 px. **À éviter** : un titre blanc fin posé sur une photo sans voile (le brief l'interdit). |

**Plateformes sans référence retenue**
- Behance : inaccessible, erreur HTTP 400 renvoyée au navigateur automatisé (n° 6 et 10).
- Pinterest : mur de connexion obligatoire. Les n° 11 et 15 ne sont lisibles qu'en partie, le n° 14 est supprimé.
- Land-book : inaccessible (challenge Cloudflare persistant). Lapa Ninja : inaccessible (« Sorry, you have been blocked »).
- One Page Love : aucun site d'aide aux seniors (voir n° 12).
- Awwwards : en plus du n° 20, la recherche renvoie un modèle « Senior Care » (wCopilot, nominé en 2023) et Canary Care (télésurveillance, nominé en 2025). Non retenus : un gabarit générique et un autre métier.
- Godly : godly.website redirige vers recent.design, sans recherche.
- ThemeForest : challenge Cloudflare (tenté pour retrouver le thème du n° 11).

**Clichés croisés** : fauteuil roulant et mains sur une canne (n° 2), blouses médicales (n° 2, 5, 10 bis), silhouettes à canne (n° 6 bis), gros plans de visages souriants (n° 15), alerte de chute (n° 9), cœurs dessinés et police manuscrite (n° 5), chiffres absurdes et faux logos clients (n° 19).

---

## Synthèse du moodboard

Les 3 directions sont maintenues et la A reste recommandée. Trois ajustements, justifiés par ce qui a été vu :
- **Chaque direction cite maintenant ses références capturées.**
- **La direction B perd son appui** : aucun site réel vu ne montre un vrai compte-rendu de passage. Home Instead (n° 7) et Home Healthcare Connected (n° 5) décrivent leur application en texte, Birdie (n° 9) montre une alerte de chute. Montrer un exemple de SMS reste notre différence, quelle que soit la direction : c'est un bloc à garder dans la A.
- **Deux modèles concrets pour les sections 5 et 7** : le tableau de Petits-fils avec la colonne « coût réel après crédit d'impôt » (n° 4) et la note d'O2 avec le nombre d'avis et la période de collecte (n° 8).

### Direction A : « Maison chaleureuse » (recommandée)
- Fond crème, titres en Lora, CTA terracotta foncée, olive pour les icônes et les séparateurs. Le secteur a déjà ses meilleurs exemples dans cette veine : Honor (n° 1, fond pêche et CTA brun), Home Instead (n° 7, serif vert foncé sur crème), AgeFree (n° 6 bis, vert profond, crème et orange). Aucun n'associe terracotta et olive : la palette reste distinctive.
- Photos réelles en lumière naturelle, personnes actives, cadres arrondis, beaucoup d'air (Honor, n° 1 ; The Legacy, n° 20).
- Évoque le foyer, pas l'hôpital. Reprend directement le README.

### Direction B : « Carnet de famille »
- Mise en page éditoriale : comptes-rendus de passage présentés comme des notes manuscrites ou des SMS, portraits en polaroïd.
- Met en scène le lien famille, notre différence clé. Seule référence visuelle : un shot d'application (n° 17).
- Risque de mièvrerie : il faut une typo sobre et aucune police manuscrite pour le texte courant (contre-exemple : le titre manuscrit et les cœurs du n° 5).

### Direction C : « Service clair »
- Fond blanc, aplats olive et crème, grandes cartes de service, chiffres et tarifs très visibles.
- Le hero de Sincere (n° 18) en est le meilleur modèle : une action pleine, une bordée, le numéro répété en clair. La ligne de 4 preuves d'Ouihelp (n° 3) et le tableau de Petits-fils (n° 4) complètent.
- Maximise la conversion, au risque de paraître moins humain.

### Palette recommandée (contrastes calculés sur #FBF5EC)

Inchangée : rien de ce qui a été vu ne justifie de modifier une couleur. Les valeurs ont été recalculées et sont exactes. Le titre orange d'Honor à 3,2:1 (n° 1) confirme la règle « décor seulement » pour la terracotta douce.

| Rôle | Hex | Contraste |
|---|---|---|
| Crème (fond) | `#FBF5EC` | fond de référence |
| Crème foncée (sections) | `#F3E6D3` | texte #2B2420 : 12,4:1 |
| Texte | `#2B2420` | 14,1:1 |
| Terracotta foncée (CTA, liens) | `#9E4A2F` | 5,6:1 ; texte blanc sur le bouton : 6,0:1 |
| Terracotta douce (décor) | `#C8775A` | 3,1:1 ; texte blanc dessus : 3,4:1 (**décor ou grands éléments seulement**) |
| Olive foncée (titres secondaires, icônes) | `#4A5628` | 7,3:1 ; texte blanc : 7,9:1 |
| Olive | `#6B7B3A` | 4,3:1 (texte ≥ 24 px ou icônes seulement) |

### Polices (Google Fonts)
- **Lora** (titres, 600 et 700).
- **Atkinson Hyperlegible** (texte et interface, 18 px minimum, 20 px recommandé sur mobile).

### 3 « à ne pas faire »
1. **Des gros plans de mains ridées, de cannes ou de fauteuils roulants, et des blouses médicales** (vus aux n° 2, 5, 6 bis et 10 bis) : ça infantilise, ça angoisse l'acheteur et ça confond aide à domicile et soin.
2. **Un carrousel automatique dans le hero** : illisible pour les seniors, et il masque le numéro.
3. **De la terracotta douce (#C8775A) pour du texte ou un bouton avec texte blanc** : le contraste est insuffisant (3,1:1 sur le crème, 3,4:1 en texte blanc).

---

## Design tokens

> Format design system. Noms en kebab-case, valeurs prêtes à passer en variables CSS (`--color-brand-primary`, etc.). Contrastes calculés sur `#FBF5EC`.

### Couleurs

**Marque**

| Token | Hex | Usage |
|---|---|---|
| `color-brand-primary` | `#9E4A2F` | CTA, liens (5,6:1) |
| `color-brand-primary-hover` | `#7F3A24` | Survol et état pressé (7,7:1 ; texte blanc 8,3:1) |
| `color-brand-primary-soft` | `#C8775A` | Illustrations, filets, puces décoratives |
| `color-brand-secondary` | `#4A5628` | Titres secondaires, icônes (7,3:1) |
| `color-brand-secondary-strong` | `#3A4520` | Texte sur fond olive clair (9,4:1) |
| `color-brand-secondary-soft` | `#6B7B3A` | Icônes, grands chiffres ≥ 24 px |

**Sémantiques** (toujours accompagnées d'une icône et d'un texte, jamais la couleur seule)

| Token | Hex | Contraste |
|---|---|---|
| `color-success` | `#3F6B2A` | 5,8:1 |
| `color-error` | `#A8322A` | 6,1:1. Proche de la terracotta, d'où l'obligation de l'icône et du libellé « Erreur » |
| `color-warning` | `#8A5A00` | 5,5:1 |
| `color-info` | `#2F5A7A` | 6,8:1 |

**Neutres**

| Token | Hex | Usage |
|---|---|---|
| `color-neutral-0` | `#FFFFFF` | Cartes, champs de formulaire |
| `color-neutral-50` | `#FBF5EC` | Fond de page |
| `color-neutral-100` | `#F3E6D3` | Fonds de section alternés |
| `color-neutral-300` | `#D9CBB6` | Bordures décoratives (1,5:1, **pas pour les bordures de champs**) |
| `color-neutral-600` | `#5E534C` | Texte secondaire (6,9:1) et bordures de champs |
| `color-neutral-900` | `#2B2420` | Texte principal (14,1:1) |

### Échelle typographique (base 18 px, ratio ≈ 1,25)

| Token | Police | Taille | Graisse | Interlignage |
|---|---|---|---|---|
| `text-display` | Lora | 48 px (mobile 36) | 700 | 1,15 |
| `text-h1` | Lora | 40 px (mobile 32) | 700 | 1,2 |
| `text-h2` | Lora | 32 px (mobile 28) | 600 | 1,25 |
| `text-h3` | Lora | 24 px | 600 | 1,3 |
| `text-body-lg` | Atkinson Hyperlegible | 20 px | 400 | 1,6 |
| `text-body` | Atkinson Hyperlegible | 18 px | 400 | 1,6 |
| `text-label` | Atkinson Hyperlegible | 18 px | 700 | 1,4 |
| `text-small` | Atkinson Hyperlegible | 16 px | 400 | 1,5. **Mentions légales uniquement** |
| `text-phone` | Atkinson Hyperlegible | 28 px (barre mobile 22) | 700 | 1,2 |

Longueur de ligne : 60 à 70 caractères maximum.

### Espacements (base 8 px)

`space-1` 4 · `space-2` 8 · `space-3` 12 · `space-4` 16 · `space-5` 24 · `space-6` 32 · `space-7` 48 · `space-8` 64 · `space-9` 96 (entre sections, desktop) · gouttière mobile : 16 px (20 px recommandé).

### Rayons

`radius-sm` 6 px (champs, badges) · `radius-md` 12 px (boutons) · `radius-lg` 20 px (cartes, photos) · `radius-full` 999 px (pastilles, avatars).

### Ombres (teintées brun, jamais noir pur)

- `shadow-sm` : `0 1px 2px rgba(43, 36, 32, 0.08)` (champs)
- `shadow-md` : `0 4px 12px rgba(43, 36, 32, 0.10)` (cartes)
- `shadow-lg` : `0 12px 32px rgba(43, 36, 32, 0.14)` (barre d'appel fixe, modale)
- `focus-ring` : `0 0 0 3px #FBF5EC, 0 0 0 6px #2F5A7A` (double anneau visible sur tous les fonds)

### Motion

| Token | Valeur | Usage |
|---|---|---|
| `duration-fast` | 120 ms | Survol, focus |
| `duration-base` | 200 ms | Ouverture d'accordéon (FAQ, tarifs) |
| `duration-slow` | 320 ms | Apparition de la barre d'appel, message de succès |
| `ease-standard` | `cubic-bezier(0.2, 0, 0, 1)` | Par défaut |
| `ease-exit` | `cubic-bezier(0.4, 0, 1, 1)` | Sorties |

`@media (prefers-reduced-motion: reduce)` : toutes les durées passent à 0 ms. Pas de parallaxe, pas d'apparition au scroll sur le texte.

---

## Composants clés

### Bouton primaire (« Être rappelé »)
- Fond `color-brand-primary`, texte blanc `text-label`, hauteur minimale 56 px, padding horizontal 24 px, `radius-md`.
- **États** : *repos* #9E4A2F · *survol* #7F3A24 · *focus* `focus-ring` · *pressé* #7F3A24 avec translation de 1 px · *désactivé* fond #D9CBB6, texte #5E534C, curseur « not-allowed », et la raison expliquée à côté · *chargement* : spinner, libellé « Envoi en cours… », bouton désactivé.

### Bouton secondaire (« Voir les tarifs », « Appeler le 0X XX XX XX XX »)
- Fond transparent, bordure 2 px `color-brand-secondary`, texte `color-brand-secondary`, même hauteur que le primaire.
- **États** : *survol* fond #F3E6D3 · *focus* `focus-ring` · *pressé* fond #E9D9C1 · *désactivé* bordure et texte #5E534C à 60 %.

### Carte de service
- Fond blanc, `radius-lg`, `shadow-md`, padding `space-6`, une icône olive de 40 px, un titre `text-h3` et une phrase `text-body`. Toute la carte est cliquable si elle mène quelque part (et alors un seul lien).

### Formulaire de rappel
- 2 champs : « Votre nom », « Votre téléphone » (`type="tel"`, `autocomplete="tel"`). Libellés **au-dessus** des champs, jamais en placeholder seul.
- Champs de 56 px de haut, bordure 2 px #5E534C, focus `focus-ring`, erreur : bordure `color-error`, icône et message sous le champ.
- Mention RGPD d'une ligne et lien vers la politique de confidentialité.

### Barre d'appel mobile
- Fixée en haut, 56 px, fond `color-neutral-0`, `shadow-lg`, numéro en `text-phone` cliquable (`tel:`), icône téléphone et libellé « Appeler ».

### À faire / À ne pas faire

| À faire | À ne pas faire |
|---|---|
| Libellés de bouton à verbe d'action précis (« Être rappelé aujourd'hui ») | « Envoyer », « Valider », « En savoir plus » |
| Cibles tactiles ≥ 48 × 48 px, espacées d'au moins 8 px | Liens texte collés les uns aux autres dans le pied de page |
| Libellés visibles au-dessus des champs | Placeholder seul comme libellé |
| Erreur = icône + texte + couleur | Bordure rouge seule |
| Numéro cliquable identique partout | Numéro en image, ou différent selon les pages (2 numéros chez Home Instead, n° 7) |
| Case de consentement décochée par défaut | Case pré-cochée (Ouihelp, n° 3) |
| Note des avis avec leur nombre et leur période de collecte (O2, n° 8) | Note seule, sans source ni date |
| Photos réelles avec consentement signé | Banques d'images de seniors stéréotypés |
| Respect de `prefers-reduced-motion` | Carrousels automatiques, parallaxe |
