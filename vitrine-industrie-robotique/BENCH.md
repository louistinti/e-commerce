# Benchmark visuel : Vibra (entreprise fictive)

## Limites, à lire en premier

Mise à jour du 2026-11-12, faite avec un vrai navigateur (Chrome piloté par Playwright).

- **Ce qui a été vu** : 14 des 19 références d'origine ont été ouvertes et capturées (n° 1 à 14). Pour le n° 2, la fiche Lapa Ninja est bloquée : c'est le site réel d'Intrepid Automation qui a été vu. Pour le n° 12, le PDF est mort : c'est la version HTML de la même étude de cas qui a été vue. Les captures sont en 1440 × 900 px, au-dessus de la ligne de flottaison, dans [`captures/`](captures/), avec une seconde capture ciblée pour 3 éléments clés (n° 2, 7 et 11). Les couleurs et les polices citées ont été relevées dans la page (`getComputedStyle`). Les chiffres cités sont ceux affichés le 2026-11-12.
- **Ce qui reste bloqué** (5 références, marquées « non vérifié ») :
  - n° 15 et 16 (Behance) : « HTTP ERROR 400 » renvoyé au navigateur automatisé ;
  - n° 17 et 18 (Pinterest) : fenêtre de connexion sur toute la page, aucune URL d'épingle exposée ;
  - n° 19 (Lapa Ninja) : challenge Cloudflare, « Sorry, you have been blocked ». Le site réel de Vibor n'a pas été retrouvé.
- **Références ajoutées** : 4 (n° 20 à 23, Dribbble et One Page Love), pour remplacer les références bloquées des sections « Preuve » et « Palette et typo ». La section « Mobile » est remplacée par 3 sites réels vus en 390 × 844 px.
- **Corrections importantes** :
  - n° 7, Tractian : la page ne parle ni de passerelle (c'est le capteur lui-même qui émet en 4G/LTE) ni de « rapport initial en 5 jours ». Et la fiche technique est **bloquée derrière un formulaire de 5 champs**, l'exact contre-exemple de notre brief.
  - n° 10, Siemens : il n'y a **aucun pourcentage** sur les arrêts non planifiés, seulement « Significant reduction ». Les seuls chiffres sont « plus de 90 machines » et « des coûts 3 à 5 fois plus élevés ».
  - n° 1, 2, 6, 14 : les phrases citées dans la version précédente (« Industrial AI for Uptime & Productivity », « from signal to measured gains », « Born at CEA-Leti, made in Grenoble ») sont les **titres d'onglet**, pas les titres affichés. Le n° 2 n'a pas « weeks, not months » en titre de hero : c'est le titre de la 2e section.
  - n° 5 : ce n'est pas une illustration 3D ombrée, c'est un dessin au trait noir (rendu « Sketch and Toon » de Cinema 4D).
  - n° 9 : rien ne permet de dire que c'est « le shot le plus vu du tag ». Il n'y a ni score de santé ni courbe de tendance.
  - n° 11 : les chiffres de Sereact ne sont pas en tête de page, ils forment la 2e section.
  - Contraste du jaune : texte `#111418` sur `#FFC20E` = **11,4:1**, pas 13:1. La couleur ne change pas, seul le calcul est corrigé.
- **URL mortes ou redirigées** : n° 12, le PDF I-care renvoie une erreur 404 (avec ou sans le double `.pdf`). n° 10, l'URL redirige vers `references.siemens.com/en/reference/siemens-cham?id=44824`. n° 2, `intrepidautomation.com` redirige vers `www.`.
- **Bannières cookies** : refusées partout où un refus existait (« Reject all », « Tout rejeter », « Deny »). Sur Augury, refus par « Use necessary cookies only ». Les fenêtres promotionnelles (webinaire Augury, visite d'usine Tractian) ont été fermées.
- **Données personnelles** : les avatars des auteurs Dribbble et One Page Love sont floutés sur les captures. Aucun formulaire n'a été rempli.

Répartition après mise à jour : sites réels 10 · Awwwards 1 · Dribbble 6 · One Page Love 2 · Behance 2 (non vérifiés) · Pinterest 2 (non vérifiés) · Lapa Ninja 1 (non vérifié). **Total : 23, dont 18 vus.**

---

## Hero

| # | Référence | URL | Source | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 1 | Augury : accueil | https://www.augury.com/ | Site réel (US) | [capture](captures/01-augury.jpg) | En-tête blanc, puis photo d'usine pétrochimique sous un voile bleu nuit. Titre centré en Inter 700, 60 px, blanc : « Industrial AI Agents That Work for You. From Uptime to Unstoppable. » Un seul bouton, orange `#EB7633`, texte blanc à 2,9:1 (sous le seuil AA). Une fenêtre de webinaire s'ouvre à l'arrivée. Plus bas, un tableau « Legacy Tools / With Augury » et une phrase qui résume notre message : « Predictive intelligence alerts your team to exactly what's failing, how urgent it is, and what to do. » **Correction** : « Industrial AI for Uptime & Productivity » est le titre d'onglet ; le titre affiché parle d'« agents IA ». La gamme en 2 produits n'apparaît pas dans le hero. **À reprendre** : la phrase « quoi, quelle urgence, quoi faire » pour l'alerte. **À éviter** : le vocabulaire « agents IA », le bouton orange à 2,9:1 et la fenêtre à l'arrivée. |
| 2 | Intrepid Automation | Lapa Ninja bloquée : https://www.lapa.ninja/post/intrepidautomation/ (non vérifié, Cloudflare). Vu à la place : https://www.intrepidautomation.com/ | Site réel (US) | [capture](captures/02-intrepid-automation.jpg), [section « weeks »](captures/02-intrepid-automation-weeks.jpg) | Hero quasi noir, rendu 3D de 4 machines alignées, titre « Are you ready for perfectly made parts? » (65 px, graisse 500, `#E2ECE2`). Étiquettes en monospace (« A01 », « SCROLL DOWN », « REQUEST A DEMO »), repères d'angle comme sur un plan. **Correction** : « Manufacturing measured in weeks, not months » est le titre de la 2e section, sur fond vert-gris très pâle `#EEF3ED`, avec 3 colonnes (« Up to 10X Faster », « Automated », « Scalable »). **À reprendre** : la formule « en semaines, pas en mois », reprise en « 3 semaines d'avance », et les étiquettes monospace. **À éviter** : le hero noir en rendu 3D. |
| 3 | Manufacturing Business Website Landing Page (Modall) | https://dribbble.com/shots/24381180-Manufacturing-Business-Website-Landing-Page | Dribbble | [capture](captures/03-dribbble-modall.jpg) | Site de Rider Tool Manufacturing (Oshawa, Ontario). Le hero est une **photo de l'équipe en tenue de travail** sous un filtre bleu foncé, avec « Your Trusted Heavy Machining and Fabrication Facility Since 1968 », un bouton bleu et une rangée de logos clients (« Trusted by the best »). La description parle bien d'une typo « aussi solide que les machines ». **Correction** : le titre est centré, de taille moyenne, en grotesque arrondie : il ne sert pas de référence de poids typographique. **À reprendre** : l'ancienneté dans le titre et les logos clients juste sous le hero. **À éviter** : le filtre bleu uniforme qui éteint la photo. |
| 4 | Path Robotics | https://www.awwwards.com/sites/path-robotics | Awwwards, site du jour (23 septembre 2021), 7,34/10 | [capture](captures/04-awwwards-path-robotics.jpg) | Studio Freight. Fond noir, cellule de soudage photographiée seule, titre géant blanc « Truly Autonomous Welding » et **grille de colonnes visible** (filets verticaux qui découpent l'en-tête et l'image). Palette déclarée : `#000`. Le site actuel a changé : « Physical AI for Manufacturing », fond `#151515`, Suisse Intl. **À reprendre** : la grille visible et la machine seule, détourée, pour la direction A (en version claire). **À noter** : une fiche Awwwards montre la version primée, pas le site actuel. |

## Explication technologique / installation

| # | Référence | URL | Source | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 5 | Sensor installation (Franco Bertoncini Andrade, pour Nordsense) | https://dribbble.com/shots/8762795-Sensor-installation | Dribbble | [capture](captures/05-dribbble-sensor-installation.jpg) | Description : « Illustration for Nordsense installation manual », faite avec Sketch et le rendu Toon de Cinema 4D. **Correction** : le résultat est un dessin isométrique au trait noir sur blanc, pas une 3D ombrée. Une pièce, ses vis en vue éclatée, un plan vert translucide (`#BFDCBF`). **À reprendre** tel quel pour les 3 étapes d'installation si les photos ne suffisent pas : un objet, le geste, aucun décor, un seul aplat de couleur. |
| 6 | Wormsensing : Plateforme | https://www.wormsensing.com/platform | Site réel (FR) | [capture](captures/06-wormsensing-platform.jpg) | **La référence la plus proche du hero voulu** : photo serrée, réelle, du capteur Dragonfly collé sur un carter, avec sa plaque signalétique et son câble. Fond `#06060F`, titre en capitales « From mechanical signals to industrial insight. » (police maison « WS Reg », graisse 800, 46 px), boutons à contour, angles droits, capitales espacées. Plus bas, la chaîne en 5 verbes (Sense, Connect, Acquire, Interpret, Decide) avec des chiffres d'unité (10 µm, 150 µm, 100 kHz, 1000×). **Correction** : « from signal to measured gains » est le titre d'onglet ; la section dit « From the machine to measured gains ». **À reprendre** : le cadrage du hero et la chaîne en verbes pour « Ce que voit le responsable maintenance ». **À éviter** : les gains en fourchettes sans périmètre (« Up to 280% », « −50 to −99% ») et le rendu 3D en carte de chaleur plus bas. |
| 7 | Tractian : Condition Monitoring | https://tractian.com/en/solutions/condition-monitoring | Site réel (US) | [capture](captures/07-tractian-condition-monitoring.jpg), [spécifications](captures/07-tractian-specs.jpg) | Hero clair : encart blanc sur une photo de raffinerie, mains qui tiennent le capteur et un téléphone. Titre « Condition Monitoring for Reliable Plants » en Inter, texte `#334155`, boutons bleu `#2563EB` (texte blanc 5,2:1) à rayon de 2 px. Sous le hero : « Trusted by 2,000 U.S. and global manufacturers ». Bloc « Technical Specifications » sur fond `#1E293B` : 6 tuiles avec icône (batterie 3 à 5 ans, -40 °F à 250 °F, Class 1 Div 1 ATEX/IECEx, IP69K, 4G/LTE, échantillonnage jusqu'à 64 kHz). **Corrections** : aucune passerelle n'est mentionnée, c'est le capteur qui émet en 4G/LTE (« No IT setup, no Wi-Fi needed ») ; aucun « rapport initial en 5 jours » sur la page. « Download Spec Sheet » ouvre un formulaire de 5 champs (nom, e-mail pro, téléphone, fonction, secteur). **À reprendre** : le bloc de 6 tuiles pour le résumé HTML de la fiche, et la FAQ « combien de temps pour installer ? ». **À éviter** : la fiche technique derrière un formulaire. |
| 8 | Industrial Internet of Things, icônes (Katie Collins) | https://dribbble.com/shots/22710707-Industrial-Internet-of-Things-IIoT-icons | Dribbble | [capture](captures/08-dribbble-iiot-icons.jpg) | Description : « Simple illustrations with thick outlines for easy identification ». Monochrome bleu sur bleu pâle : engrenages, globe en réseau, satellite, nuage « IIoT », ampoule, bras robot, liés par des pointillés. **À reprendre** : le trait épais, lisible en petit. **À éviter** : le répertoire d'icônes lui-même, générique (aucun capteur, moteur ni roulement). Les pictos de Vibra doivent montrer les vrais objets : capteur, moteur, pompe, passerelle. |

## Données / tableau de bord

| # | Référence | URL | Source | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 9 | Preventive Maintenance Dashboard (Jagath Selvan) | https://dribbble.com/shots/9109597-Preventive-Maintenance-Dashboard | Dribbble | [capture](captures/09-dribbble-maintenance-dashboard.jpg) | Tableau de bord pour l'industrie chimique. En haut, « 25 Total Machines » puis des compteurs par type d'alerte (pression, température, vibration, débit de gaz). Dessous, une grille de cartes machine avec 4 valeurs et leur unité. Une alerte = bordure rouge, valeur en rouge et petite pastille. Horodatage « Last Updated ». **Corrections** : ni score de santé, ni courbe de tendance ; « le plus vu du tag » n'est pas vérifiable. La vibration est affichée en « hz », pas en mm/s. **À reprendre** : la grille « une carte = une machine » et l'horodatage. **À éviter** : l'alerte signalée surtout par la couleur. Pour la capture annotée de Vibra, ajouter le score et la tendance, et une icône plus un libellé pour chaque statut. |
| 10 | Siemens Senseye : référence usine de Cham | https://references.siemens.com/en/reference/44824?id=44824 (redirige vers `/siemens-cham?id=44824`) | Site réel (DE) | [capture](captures/10-siemens-senseye-cham.jpg) | Hero bleu nuit `#000028`, titre « Siemens Cham, Germany - Reduced unplanned downtime with Senseye Predictive Maintenance » en police Siemens, **photo de banque d'images** (bokeh de lumières). Le corps suit 3 rubriques : « Customer objectives », « Solution and Service », « Customer benefits ». **Correction** : pas de résultat chiffré sur les arrêts (« Significant reduction »). Chiffres présents : plus de 90 machines suivies sur la ligne pilote, coûts 3 à 5 fois plus élevés en cas de panne, usine de 470 salariés. C'est aussi une référence interne (Siemens chez Siemens). **À reprendre** : les 3 rubriques objectifs, solution, bénéfices, et le site nommé. **À éviter** : la photo d'ambiance sans rapport et le résultat sans chiffre. |
| 11 | Sereact : Pick and Place | https://sereact.ai/product/pick-and-place | Site réel (DE) | [capture](captures/11-sereact-pick-and-place.jpg), [KPI](captures/11-sereact-kpis.jpg) | Hero en vidéo réelle de la cellule robot (bandes jaune et noir au sol), titre « Reliable Picking. At Any Scale. » en Montserrat 300, 72 px, blanc. **Correction** : les chiffres sont dans la 2e section, « Key Production KPIs » : 8,000+ prises par jour, 600+ unités par heure en pointe, > 99 % de prises réussies. Chacun a son étiquette en monospace 12 px bleu `#0284C7`, un grand chiffre en Montserrat 300 de 60 px et une phrase de contexte (« When your system can feed fast enough. »). **À reprendre** pour la section « coût d'un arrêt » : grand chiffre, unité en étiquette monospace, phrase de périmètre, filets fins. Cela valide l'option IBM Plex Mono pour les étiquettes de données. |

## Preuve et témoignages

| # | Référence | URL | Source | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 12 | I-care : étude de cas Barry Callebaut (Louviers) | PDF mort : https://www.icareweb.com/wp-content/uploads/2022/06/FR-I-care-Barry-Callebaut-Success-Story.pdf.pdf (erreur 404). Vu à la place : https://www.icareweb.com/knowledge/predictive-maintenance/success-story-barry-callebaut/ | Site réel (BE), en anglais | [capture](captures/12-icare-barry-callebaut.jpg) | L'étude existe maintenant **en HTML**. Titre Poppins 600 en `#0E1132`, photo réelle d'un opérateur sur la ligne, secteur et taille de l'entreprise en icônes. Structure : citation du responsable fiabilité du site, puis « Challenges », « Solutions », « Benefits », chacune avec une liste d'étiquettes. Faits confirmés : site de 350 salariés, environ 4 000 équipements, capteurs Wi-care loués, moteur suivi jusqu'à l'arrêt programmé. Chiffres : 30 h d'arrêt évitées sur les broyeurs, 1 h d'arrêt = 5 000 $, réducteurs à 2 ans de durée de vie au lieu de 3 mois. Le bouton « Contact us » orange `#F7941D` a un texte blanc à 2,3:1. **À reprendre** : la structure et le chiffre d'arrêt évité mis en regard du coût horaire, pour les cartes « Retours d'usine ». **À éviter** : les chiffres enfouis en fin de page et le bouton orange illisible. |
| 13 | Exotec : Ressources | https://www.exotec.com/fr/ressources/ | Site réel (FR) | [capture](captures/13-exotec-ressources.jpg) | Titre « Ressources » en Inter, 90 px, puis des blocs alternés gris clair et blanc (Articles, Cas clients, Talks, Livres blancs, Visite d'entrepôt), boutons turquoise `#28AFB9` à texte blanc (2,7:1, sous le seuil). La **visite à 360°** est confirmée : « Explorez nos entrepôts à 360° depuis chez vous ». L'en-tête propose aussi « Visiter un site ». **À reprendre** en phase 2 : la photo à 360° d'une ligne équipée, et l'idée « visiter un site client ». **À éviter** : le turquoise à texte blanc. |
| 14 | Wormsensing : About us | https://www.wormsensing.com/about-us | Site réel (FR) | [capture](captures/14-wormsensing-about.jpg) | Hero : photo aérienne de Grenoble et des Alpes, titre « A science park called Grenoble. ». Le texte dit : fondée en 2020 par deux ingénieurs de recherche du CEA, « Engineered in Grenoble ». **Correction** : « Born at CEA-Leti, made in Grenoble » est le titre d'onglet. **À reprendre** : l'ancrage territorial en une ligne et une photo de la ville. Pour Vibra : Saint-Étienne, en photo réelle. |
| 15 | Industrial Internet of Things Corporate Website (Zajno pour KONUX) | https://www.behance.net/gallery/53536049/Industrial-Internet-of-Things-Corporate-Website | Behance | Non vérifié | **Non vérifié** : Behance renvoie « HTTP ERROR 400 ». La page du projet sur zajno.com n'existe plus (404) et konux.com parle aujourd'hui de ferroviaire. L'idée de « deux lectures » est reprise par le n° 21, vu. |
| 21 | AI Infrastructure Website (UX MIND agency, NIXTA Power Fabric) | https://dribbble.com/shots/27803560-AI-Infrastructure-Website-Energy-Tech-UI-UX | Dribbble (ajouté) | [capture](captures/21-dribbble-uxmind-nixta.jpg) | Remplace le n° 15. La description pose exactement notre problème : éviter de faire « soit une fiche technique, soit un site vague ». La page commence par l'échelle de l'idée, puis explique le système pas à pas ; la profondeur technique reste, sans obliger à tout décoder avant de comprendre la valeur. Visuel : maquette mobile blanche, bloc « The numbers » en chiffres monospace pointillés, palette `#09090A`, `#F9F9F9`, jaune `#FDE400`. **À reprendre** : l'ordre « valeur pour la directrice, puis détail pour le maintenancier ». |
| 22 | Plastics Unlimited (Nerdwerx) | https://onepagelove.com/plastics-unlimited | One Page Love (ajouté, publié le 15 février 2016) | [capture](captures/22-onepagelove-plastics-unlimited.jpg) | Plasturgiste américain, site aujourd'hui hors ligne (capture conservée par One Page Love). Bandeau noir fixe avec **le numéro de téléphone en premier**, puis « Capabilities » en accordéon (Thermoforming, Composites…), en capitales sur fond rouge, et « Sales representatives as well as technical advisors are available ». One Page Love signale une galerie d'équipe avec e-mail et poste téléphonique. **À reprendre** : le téléphone toujours visible, la liste de savoir-faire en accordéon pour les secteurs, et les interlocuteurs nommés par région. **À éviter** : les aplats rouge et bleu saturés. |

## Palette et typo

| # | Référence | URL | Source | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 16 | Speak Up Africa, identité (Éditions Pépé) | https://www.behance.net/gallery/71073479/Speak-Up-Africa-Visual-identity-for-Social-Media | Behance | Non vérifié | **Non vérifié** : Behance renvoie « HTTP ERROR 400 ». Remplacé par le n° 20 pour tester une condensée avec du jaune en grand format. |
| 17 | Industrial Company Website Inspiration | https://www.pinterest.com/ideas/industrial-company-website-inspiration/897062612591/ | Pinterest (page d'idées) | Non vérifié | **Non vérifié** : une fenêtre de connexion couvre la page et aucune URL d'épingle n'est exposée. Derrière la fenêtre (non capturé, page de connexion), les vignettes visibles sont surtout anthracite et orange, quelques-unes bleues : pas le partage « bleu et blanc / jaune et gris » annoncé. Le code « jaune = chantier » est en revanche confirmé sur Dribbble (voir n° 20 et « Galeries »). |
| 18 | 34 Website Design – Industrial ideas | https://www.pinterest.com/jclewis33/website-design-industrial/ | Pinterest (tableau) | Non vérifié | **Non vérifié** : même fenêtre de connexion. Derrière, des templates génériques (rouge, orange, jaune et marine). L'objectif « repérer les templates et s'en éloigner » reste valable, sans référence vue. |
| 20 | Sterial, site de désinfection (Pxcraftt) | https://dribbble.com/shots/27613985-Worker-in-Hazmat-Suit-Spraying-Disinfectant-Website-Design | Dribbble (ajouté) | [capture](captures/20-dribbble-pxcraftt-disinfection.jpg) | Remplace le n° 16. Titre en capitales condensées très grasses, noir sur blanc (« Extreme Clean. Total Disinfection. »), un mot en contour, le dernier surligné de jaune. Moitié droite en aplat jaune avec une grille fine et une photo détourée. Étiquettes monospace (« 01 Services », « SYS.CHECK - OK »), téléphone et bouton jaune « Emergency » dans l'en-tête, bande de hachures noir et jaune en séparateur. **À reprendre** : la condensée noire en grand, les étiquettes monospace, le téléphone dans l'en-tête. **À éviter** : la moitié de page en aplat jaune et les hachures, qui font basculer dans la signalétique (cf. « à ne pas faire » n° 2). |
| 23 | B-Metal | https://onepagelove.com/b-metal | One Page Love (ajouté, publié le 17 décembre 2019) | [capture](captures/23-onepagelove-b-metal.jpg) | Métallurgie (Italie). Logo en très grande grotesque noire (Acumin) sur fond blanc avec un carré beige, une phrase d'accroche en grand corps, puis une photo plein cadre de meulage avec des étincelles. **À reprendre** : le grand titre noir sur blanc avec beaucoup d'air, proche de la direction A. **À éviter** : la photo d'étincelles, devenue le cliché du secteur métal. |

## Mobile

| # | Référence | URL | Source | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 19 | Vibor (capteurs industriels) | https://www.lapa.ninja/post/vibor/ | Lapa Ninja | Non vérifié | **Non vérifié** : challenge Cloudflare. Le site réel de Vibor n'a pas été retrouvé par la recherche web. Remplacé par les 3 sites réels vus en 390 × 844 px ci-dessous. |

Trois sites vus en 390 × 844 px le 2026-11-12 :

| Site | Capture | Ce qu'on observe |
|---|---|---|
| Tractian : Condition Monitoring | [capture](captures/mobile-tractian.jpg) | Le texte passe au-dessus de la photo, les 2 boutons « See Pricing » et « Book a Demo » restent côte à côte. Seule la barre de navigation est collante. « Contact us », visible avec une icône de téléphone sur desktop, disparaît dans le menu burger. Aucun lien `tel:` sur la page. |
| Wormsensing : Plateforme | [capture](captures/mobile-wormsensing.jpg) | La photo est recadrée sur le capteur, qui reste lisible au-dessus du titre. Les 2 boutons passent l'un sous l'autre en pleine largeur, 48 px de haut. En-tête fixe réduit à « Menu ». Aucun lien `tel:`. |
| I-care : Barry Callebaut | [capture](captures/mobile-icare.jpg) | La photo passe au-dessus du titre, puis secteur et taille en icônes. Le seul élément fixe est une bulle de chat orange en bas à droite (plus le bouton de consentement). Aucun lien `tel:` ; les chiffres clés (30 h, 5 000 $ de l'heure) sont tout en bas de la page. |

Ce que ces observations confirment pour Vibra :
- **aucun des 3 sites ne propose d'appel en 1 tap**. La barre fixe « Appeler un technicien » avec un vrai lien `tel:` devient un point de différence, pas une simple reprise. Elle ne se cache jamais dans le menu. Parmi les sites réels vus, seul Plastics Unlimited (n° 22, desktop, 2016) mettait le téléphone en premier ;
- recadrer la photo du hero sur le capteur posé, comme Wormsensing, pour qu'il reste visible en 390 px ;
- boutons empilés en pleine largeur, 48 px minimum (Wormsensing est exactement à 48 px) ;
- le chiffre clé d'un témoignage remonte en tête de carte, au lieu d'être en fin d'article comme chez I-care ;
- la fiche technique en 1 tap, sans formulaire : c'est l'inverse de Tractian (n° 7).

---

## Galeries : requêtes lancées

| Plateforme | Requêtes ou pages | Résultat |
|---|---|---|
| Behance | n° 15 et 16 | Inaccessible : « HTTP ERROR 400 » au navigateur automatisé. |
| Pinterest | n° 17 et 18 | Inaccessible sans compte : fenêtre de connexion, aucune URL d'épingle exposée. Pas de capture (page de connexion). |
| Lapa Ninja | n° 2 et 19 | Inaccessible : challenge Cloudflare. |
| Dribbble | n° 3, 5, 8, 9 ; recherche « industrial yellow website » | 2 retenues (n° 20, 21). Sur la première page de résultats, la grande majorité des sites jaunes sont du BTP, de la toiture ou des engins : le jaune vif dit « chantier ». |
| Awwwards | n° 4 | Fiche vue. Pas de nouvelle recherche. |
| One Page Love | tag « industrial » (8 fiches) | 2 retenues (n° 22, 23). Les autres sont hors sujet (blog, restauration écologique), hors ligne depuis 2012-2013, ou au style « futuriste 3D » (Aevion, drone). |
| Land-book, Godly | non relancés | Bloqués sur ce projet (Cloudflare, redirection vers recent.design). |

---

## Synthèse du moodboard

**Ajustements après observation (2026-11-12)**
- Les heros du secteur sont sombres : Augury (voile bleu nuit), Intrepid (quasi noir), Path Robotics (`#000`, puis `#151515`), Wormsensing (`#06060F`), Sereact (vidéo d'atelier), Siemens (`#000028`). Seuls Tractian et I-care ont un hero clair. La direction B est donc le registre par défaut du secteur, et la direction A s'en démarque : la recommandation est maintenue, avec cette raison en plus.
- Aucun site vu ne propose d'appel en 1 tap sur mobile, et Tractian bloque sa fiche technique derrière un formulaire. Les trois actions de Vibra (tester, appeler, télécharger sans formulaire) deviennent des arguments de différence.
- Sur Dribbble, le jaune vif sert surtout au BTP et aux engins. La règle « jaune en accent, jamais en aplat » est confirmée, et le n° 20 montre ce qui arrive quand on la dépasse.
- La palette et les tokens ne changent pas : aucune observation ne le justifie. Seul le contraste du jaune est recalculé (11,4:1 au lieu de 13:1), sans changer la couleur.
- Trois boutons du panel sont sous le seuil AA avec du texte blanc : orange Augury (2,9:1), orange I-care (2,3:1), turquoise Exotec (2,7:1). Cela confirme la règle « texte foncé sur jaune ».

**Direction A : « Fiche technique »** (recommandée)
- Fond blanc et gris acier, grille visible, grands chiffres en Barlow Condensed, photos serrées sur le capteur posé.
- Le jaune est réservé au CTA et aux repères d'étapes.
- Rassure le maintenancier : on dirait un document de travail, pas une pub.
- Références vues : Wormsensing (n° 6) pour le cadrage du hero, Sereact (n° 11) pour les chiffres et leurs étiquettes monospace, Tractian (n° 7) pour le bloc de spécifications, Path Robotics (n° 4) pour la grille visible, le dessin au trait du n° 5 pour les étapes.

**Direction B : « Atelier de nuit »**
- Fond graphite, photos d'atelier contrastées, le jaune en bandes de balisage.
- Plus d'impact au salon et sur LinkedIn.
- Risque l'effet « gaming industriel » s'il est surdosé.
- C'est le registre de la majorité du panel (n° 1, 2, 4, 6, 11) : Vibra s'y fondrait.

**Direction C : « Carnet de terrain »**
- Photos documentaires des techniciens en intervention, légendes manuscrites ou monospace, témoignages en avant.
- Très crédible, mais dépend entièrement de la séance photo et des accords clients.
- Référence vue : l'étude I-care (n° 12), avec une photo réelle d'opérateur et une citation nommée.

## Palette recommandée

| Rôle | Hex | Note |
|---|---|---|
| Acier foncé (titres, pied de page) | `#2B3036` | |
| Acier | `#4A525B` | texte secondaire sur blanc, contraste de 7,9:1 (recalculé le 2026-11-12) |
| Gris moyen (filets) | `#8A939C` | décor uniquement, pas de texte |
| Gris clair (fonds de section) | `#ECEEF0` | |
| Blanc | `#FFFFFF` | |
| Jaune sécurité | `#FFC20E` | proche des RAL 1003 et 1023 (valeur RVB indicative). **Fond de bouton avec texte `#111418`** (contraste de 11,4:1, recalculé le 2026-11-12 ; la version précédente indiquait 13:1 par erreur) ; **jamais en texte sur blanc** (1,6:1) |

## Polices (Google Fonts)

- **Barlow Condensed** : 600 et 700 pour les titres, les chiffres-clés et les étiquettes.
- **Barlow** : 400 et 500 pour le texte, 600 pour les boutons.
- Option données : **IBM Plex Mono** 500 pour les valeurs de capteurs (mm/s, °C) dans les captures annotées.

## 3 « à ne pas faire »

1. Pas de photo de banque d'images (ouvrier souriant avec tablette, usine teintée en bleu) : ce public la repère immédiatement.
2. Pas de jaune en aplat sur toute la page ni de rayures noir et jaune partout : on bascule dans le code BTP et signalétique.
3. Pas de vocabulaire IA ni de tableau de bord « futuriste » (néon, 3D) : la capture doit ressembler au vrai logiciel.

---

## Design tokens

### Couleurs

| Token | Hex | Usage |
|---|---|---|
| `color.brand.primary` | `#FFC20E` | fond du CTA principal, repères d'étapes |
| `color.brand.primary-hover` | `#E5AC00` | survol du CTA |
| `color.brand.ink` | `#111418` | texte sur jaune, titres |
| `color.neutral.900` | `#2B3036` | titres, pied de page |
| `color.neutral.700` | `#4A525B` | texte courant secondaire |
| `color.neutral.400` | `#8A939C` | filets, icônes inactives |
| `color.neutral.100` | `#ECEEF0` | fonds de section |
| `color.neutral.0` | `#FFFFFF` | fond principal |
| `color.semantic.success` | `#1E7F4F` | machine OK, envoi réussi (texte blanc, 5,0:1) |
| `color.semantic.warning` | `#B45309` | dégradation à surveiller (le jaune de marque n'est pas utilisé pour l'alerte, pour éviter la confusion) |
| `color.semantic.error` | `#C62828` | défaut critique, erreur de formulaire |
| `color.focus` | `#1F6FEB` | anneau de focus clavier (distinct du jaune) |

Les statuts sont toujours doublés d'une icône et d'un libellé, jamais signalés par la couleur seule.

### Typographie

| Token | Police | Taille (desktop / mobile) | Graisse | Interlignage |
|---|---|---|---|---|
| `type.display` | Barlow Condensed | 72 / 44 px | 700 | 1,0 |
| `type.h1` | Barlow Condensed | 48 / 34 px | 700 | 1,05 |
| `type.h2` | Barlow Condensed | 36 / 28 px | 600 | 1,1 |
| `type.h3` | Barlow | 22 / 20 px | 600 | 1,3 |
| `type.body` | Barlow | 18 / 17 px | 400 | 1,55 |
| `type.small` | Barlow | 15 / 15 px | 500 | 1,45 |
| `type.label` | Barlow Condensed | 14 px, majuscules, interlettrage 0,04 em | 600 | 1,2 |
| `type.data` | IBM Plex Mono | 16 px | 500 | 1,4 |

### Espacement (base 4 px)

`space.1` 4 · `space.2` 8 · `space.3` 12 · `space.4` 16 · `space.6` 24 · `space.8` 32 · `space.12` 48 · `space.16` 64 · `space.24` 96 (marge verticale entre sections sur desktop ; 64 sur mobile).

### Rayons

`radius.none` 0 (photos, sections) · `radius.sm` 2 px (boutons, champs) · `radius.md` 4 px (cartes). Des angles presque vifs, pour un registre industriel.

### Ombres

`shadow.none` par défaut (on préfère les filets) · `shadow.sm` `0 1px 2px rgba(17,20,24,.08)` pour les cartes au survol · `shadow.sticky` `0 -2px 8px rgba(17,20,24,.12)` pour la barre d'appel fixe sur mobile.

### Motion

| Token | Valeur | Usage |
|---|---|---|
| `motion.duration.fast` | 120 ms | survol, focus |
| `motion.duration.base` | 200 ms | ouverture d'accordéon, changement d'onglet |
| `motion.duration.slow` | 400 ms | apparition des 3 étapes au défilement (une fois) |
| `motion.easing.standard` | `cubic-bezier(.2,0,0,1)` | |
| `motion.easing.exit` | `cubic-bezier(.4,0,1,1)` | |

`prefers-reduced-motion` : toutes les durées passent à 0, sans apparition au défilement.

### Composants clés

**Bouton primaire** (« Tester sur une machine »)
- Fond `brand.primary`, texte `brand.ink`, Barlow 600 en 17 px, hauteur 48 px minimum, `radius.sm`.
- États :
  - survol : `primary-hover` ;
  - focus : anneau `color.focus` de 3 px, décalé de 2 px ;
  - actif : enfoncé de 1 px ;
  - désactivé : `neutral.100` avec texte `neutral.400` et `aria-disabled` ;
  - chargement : spinner avec le libellé « Envoi… ».

**Bouton secondaire** (« Appeler un technicien », « Télécharger la fiche technique »)
- Contour de 2 px `neutral.900`, texte `neutral.900`, fond transparent.
- États :
  - survol : fond `neutral.100` ;
  - focus : identique au primaire ;
  - désactivé : contour `neutral.400`.
- Sur mobile, « Appeler » devient une barre fixe en bas d'écran (`tel:`).

**Carte témoignage**
- Photo réelle 4:3 sans rayon, citation en `type.h3`, puis nom, fonction, site et ville en `type.small`.
- Une pastille machine et défaut en `type.label`.
- Filet `neutral.100` et `radius.md`.

**Formulaire pilote**
- 5 champs maximum, un libellé au-dessus de chaque champ (jamais seulement un placeholder), champs de 48 px de haut.
- Erreurs sous le champ en `semantic.error` avec une icône, et `aria-describedby`.
- Le téléphone est obligatoire, l'e-mail facultatif.

### À faire / À ne pas faire

| À faire | À ne pas faire |
|---|---|
| Jaune en fond de bouton avec texte foncé | Jaune en texte ou en icône sur fond blanc |
| Statuts couleur, plus icône, plus libellé | Statut indiqué seulement par du rouge ou du vert |
| Photos réelles, cadrage serré sur la machine | Images de banque ou rendus 3D génériques d'usine |
| Un seul CTA primaire par écran | Trois boutons jaunes côte à côte |
| Cibles tactiles de 48 px minimum (usage avec des gants) | Liens texte de 14 px comme seul moyen d'action |
| Fiche technique téléchargeable sans formulaire | Fiche technique bloquée derrière un formulaire de 8 champs |
| Chiffres avec unité et périmètre (« 19 jours, médiane sur 20 pilotes ») | « Jusqu'à 100 % de pannes évitées » |
