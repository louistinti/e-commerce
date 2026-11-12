# Benchmark visuel : Veilla (santé / medtech)

> **Veilla est fictive.** Les références ci-dessous sont réelles. La première version (novembre 2026) avait été écrite sans navigateur ; elle a été vérifiée le 2026-11-12 (voir ci-dessous).

## Limites, à lire en premier

Mise à jour du 2026-11-12, faite avec un vrai navigateur (Chrome piloté par Playwright).

- **Ce qui a été vu** : 14 des 20 références d'origine. 10 ont été ouvertes à leur URL (n° 1, 2, 5, 6, 7, 8, 10, 12, 15, 17). Pour 4 autres, la galerie était bloquée, mais le site réel ou la page du studio a été ouvert à la place (n° 3, 13, 14, 20). Les captures sont en 1440 × 900 px, au-dessus de la ligne de flottaison, dans [`captures/`](captures/). Quelques références ont une seconde capture (site réel derrière une fiche Awwwards, ou bloc clé plus bas). Les couleurs et les polices citées ont été relevées dans la page (`getComputedStyle`), ou dans l'image du shot pour Dribbble. Les chiffres cités sont ceux affichés le 2026-11-12.
- **Non vérifié (6)** : Withings n° 4 (challenge Cloudflare, non contourné), Behance n° 9 et 11 (erreur HTTP 400), Carbon Health n° 16 (Land-book et carbonhealth.com bloqués par Cloudflare), épingles Pinterest n° 18 et 19 (mur de connexion : seuls le titre, le texte alternatif de l'image et la description ont pu être lus, pas de capture). Lapa Ninja (n° 3, 13) et Land-book (n° 14) bloquent aussi par Cloudflare.
- **Ajouts (4)** : n° 21 Calmedica (concurrent français direct, télésuivi par SMS), n° 22 et 23 (Dribbble, à la place des Behance n° 11 et 9), n° 24 (Dribbble, sauge, en complément des épingles n° 18 et 19). Plus 4 captures mobiles en 390 × 844 px (Cureety ×2, Resilience, Doxy.me).
- **Corrections importantes** :
  1. Implicity (n° 6) n'utilise pas le format « grand chiffre, légende, source » : ses chiffres sont dans des paragraphes de 14 à 15 px, avec appels de note. Le modèle du format est **Resilience** (n° 5).
  2. Cureety (n° 10) n'a pas de centre d'aide « activer son compte, se connecter » sur la page patient : c'est un formulaire de contact. En revanche, une **fenêtre de choix « patient ou professionnel »** s'ouvre à la première visite, avec un bouton vert pour le patient et un bouton bleu pour le soignant.
  3. Resilience (n° 5) et Implicity (n° 6) ouvrent une **fenêtre « contenu réservé aux professionnels de santé »** avant la page. Ce motif, absent de la version précédente, est le plus utile du bench pour Veilla (voir la synthèse).
  4. Plusieurs sites ont changé depuis leur indexation : Heva (n° 2), Doxy.me (n° 14, titre devenu un superlatif), Fluent Health (n° 3, devenu avaros.ai). Brightlab (n° 12) montre une application patient, pas un cadre navigateur. Institute of Health (n° 7) est un organisme de formation, pas un site institutionnel avec comité scientifique.
  5. Le guide Pinterest (n° 17) conseille un accent chaud pour les CTA : il ne « valide » donc pas tout notre trio. Notre CTA reste bleu, par choix (le rouge et l'orange signalent l'alerte dans le produit).
- **Palette et tokens** : inchangés. Tous les contrastes du tableau ont été recalculés (WCAG 2.1) et sont justes à l'arrondi près.
- **Bannières cookies** : refusées partout où un refus existait (« Reject All », « Decline All », « Deny », « Reject », « Tout rejeter »). Une fenêtre d'inscription plein écran (Heva) a été fermée par « No thanks ». Aucune fenêtre « je suis un professionnel de santé » n'a été validée : le texte des pages a été lu sans cliquer.
- **Vie privée** : les avatars des designers sont floutés sur les captures Dribbble et Awwwards. Les photos de personnes présentées comme patientes ou élèves (Cureety, Institute of Health) sont floutées.

**Répartition** : 24 références, plus 4 captures mobiles : sites réels 5, Dribbble 5, Awwwards 3, Pinterest 3, Behance 3 (bloqués ; le n° 20 a été vu sur la page du studio), Land-book 2 et Lapa Ninja 2 (bloqués ; les n° 3, 13 et 14 ont été vus sur le site réel), One Page Love 1. Godly : aucun résultat.

---

## Hero

| # | Titre | Source | URL | Capture | À retenir |
|---|---|---|---|---|---|
| 1 | Medical Website Design (Hero Section), Isfak Sarder | Dribbble | https://dribbble.com/shots/19190049-Medical-Website-Design-Hero-Section | [capture](captures/01-dribbble-isfak-hero.jpg) | Maquette « Mediex » : titre noir à gauche (« Working for Your Better Health. »), texte de remplissage en latin, bouton bleu « Meet Our Specialists », photo détourée d'un médecin souriant dans une arche bleue `#4566BF` et jaune `#F3D348`, bulles d'avis flottantes, et sous le CTA « 2,491 Happy Customers » et « 4.9/5 Rating ». Fond `#F4F6FA`. **À reprendre** : la mise en page titre à gauche, visuel à droite, preuve courte sous le CTA. **À éviter** : la photo de banque d'images d'un médecin, les chiffres sans source et le jaune vif. |
| 2 | Heva Health, Site of the Day (26/07/2024) | Awwwards | https://www.awwwards.com/sites/heva-health | [capture](captures/02-awwwards-heva-health.jpg) · [site](captures/02b-heva-site.jpg) | SOTD confirmé (7,11/10). Palette Awwwards à 2 couleurs : crème `#FDFDF1` et vert olive `#39442B`, retrouvées sur le site réel (https://www.hevahealth.com/). Le site a changé depuis 2024 : « Vitality, refined. » en PP Editorial New (104 px, graisse 300, crème `#FDFDF1`) sur une photo plein écran, texte en Inter, boutons olive à texte crème (10,1:1). Une fenêtre plein écran « 30 % off » réclame l'e-mail dès l'arrivée. « 4.9/5 from 12,000+ successful consultations » sans source. **À reprendre** : le couple vert sombre et crème, très proche de notre sauge foncée sur blanc chaud. **À éviter** : la fenêtre d'inscription à l'arrivée et le ton bien-être. |
| 3 | Fluent Health (devenu avaros.ai) | Lapa Ninja (bloqué), site réel | Lapa : https://www.lapa.ninja/post/fluent/ (Cloudflare). Vu à la place : https://www.fluent.health/ qui redirige vers https://avaros.ai/ | [capture](captures/03-fluent-avaros.jpg) | Le produit a été renommé. Fond bleu nuit `#051023`, titre « It's time to look up » en Montserrat 88 px, graisse 500, lavande `#C6CEF0`. La phrase « Have a natural conversation with your patients. We'll take care of the note. » est bien là, mais en **sous-titre**. Au centre, un téléphone qui enregistre et deux bulles « Patient » et « Doctor ». CTA vert pomme `#BFFF99` à texte sombre (16,3:1). **À reprendre** : un sous-titre qui dit le bénéfice soignant en une phrase. **À éviter** : le thème sombre et le vert fluo, loin du ton calme de Veilla. |
| 4 | Withings Health Solutions, Remote Patient Monitoring | Site réel | https://www.withings.com/us/en/health-solutions/remote-patient-monitoring | Aucune | **Non vérifié** : page bloquée par un challenge Cloudflare (« Performing security verification »), non contourné. Le texte précédent (appareil + tableau de bord + charge de travail) reste une hypothèse. Pour un hero établissement sur le même sujet, voir Calmedica (n° 21). |

## Réassurance et preuves

| # | Titre | Source | URL | Capture | À retenir |
|---|---|---|---|---|---|
| 5 | Resilience Oncology | Site réel | https://www.resilience.care/healthcare-providers/oncology | [capture](captures/05-resilience-oncology.jpg) | **La page s'ouvre sur une fenêtre** : « This site is intended for healthcare professionals », avec « Not a healthcare professional? Visit patients.resilience.care » et deux boutons (« I am / I am not a healthcare professional »). Derrière : titre serif EB Garamond 64 px, graisse 400, brun très sombre `#282421` sur blanc, bouton « Request a demo » `#282421` à texte `#F4F1E9` (13,6:1). Le bloc preuves est le meilleur du panel : 4 grands chiffres (« +5,2 Months in overall survival », « +1,9 Months of treatment duration », « +88 % », « -25 % severe toxicities ») avec appels de note et un lien « See sources » (Basch, JCO 2017 ; Basch et al., JAMA 2022 ; Mir et al., 2020 ; Patt, 2023). En pied de page : « Class IIa medical device », « CE 0459 », « reimbursed by the French Assurance Maladie », « Update : March 2026 ». Rubrique « Latest Publications » et lien « Scientifics publications ». **À reprendre** : la fenêtre pro avec renvoi vers le chemin patient, les grands chiffres sourcés, la mention réglementaire datée. |
| 6 | Implicity, CIED Remote Monitoring | Site réel | https://implicity.com/cied-remote-monitoring/ | [capture](captures/06-implicity-cied.jpg) | Fenêtre « This content is intended for US Healthcare Professionals only. Do you wish to continue? » (Oui / Non). Hero bleu nuit, titre Montserrat 48 px, graisse 700, blanc. Bouton d'en-tête turquoise `#5DC8D2` à texte `#2C304E` (6,5:1), mais bouton « Request a demo » à texte blanc sur `#2B8F9C` : **3,8:1, sous le seuil AA**. « No software to install and no update needed » confirmé. **Correction** : les chiffres (-79 % de faux positifs, -85 % d'alertes FA inutiles, 28 % de patients reconnectés) sont dans des paragraphes de 14 à 15 px, pas en grand. Chaque chiffre a un appel de note vers une référence publiée, et les notes donnent le statut réglementaire des modules (classe, marquage CE ou FDA). **À reprendre** : les notes et le statut par fonctionnalité. **À éviter** : des chiffres forts noyés dans le texte. |
| 7 | Institute of Health, Honorable Mention (05/02/2026) | Awwwards | https://www.awwwards.com/sites/institute-of-health | [capture](captures/07-awwwards-institute-of-health.jpg) · [site](captures/07b-institute-of-health-site.jpg) | Mention confirmée. Palette Awwwards : `#F8F4ED` et `#242424` ; Webflow, GSAP, WebGL. **Correction** : c'est un organisme de formation en médecine fonctionnelle pour praticiens, pas un site institutionnel ; pas de comité scientifique visible. Site réel (https://www.instituteofhealth.com/) : vidéo plein écran, titre Lay Grotesk 58 px, graisse 500, blanc, et 3 chiffres empilés à droite (966, 46, 22) séparés par de fins filets. Ton promotionnel : « Global leaders », « The only… », « over 2,000 published medical journals ». **À reprendre** : la colonne de chiffres à filets fins. **À éviter** : les superlatifs et les chiffres sans source, interdits par le brief. |
| 8 | MyHealthPrac, Site of the Day (11/07/2025) | Awwwards | https://www.awwwards.com/sites/myhealthprac | [capture](captures/08-awwwards-myhealthprac.jpg) · [site](captures/08b-myhealthprac-site.jpg) | SOTD confirmé (7,24/10), même designer que le n° 7. Palette Awwwards `#F1F1F1` et `#010101`. Site réel (https://www.myhealthprac.com/) : photo plein écran d'un œil aux tons cuivrés, « See Beyond. Unlock Your Health » en Neue Montreal 72 px, blanc. Les deux publics sont séparés **dans le menu** (« For you », « For professionals »), avec un seul CTA « Join Waitlist » (pilule noire). Plus bas, des cartes de biomarqueurs avec valeur et unité. **À reprendre** : deux entrées de menu nommées par public. **À éviter** : le texte blanc posé sur une photo, dont le contraste varie selon l'image. |
| 21 | Calmedica, télésuivi patient (ajout) | Site réel (FR) | https://calmedica.com/ | [capture](captures/21-calmedica.jpg) · [chiffres](captures/21b-calmedica-chiffres.jpg) | Concurrent direct : questionnaire par SMS, « sans application » (memoQuest). Dans notre navigateur, le hero est resté sur l'image du logo (vidéo d'intro) et le titre « Tous les patients, tous les parcours » (Inter 64 px, graisse 300, orange `#F64E15`) ne s'est pas affiché (opacité 0). Plus bas : 3 grands chiffres orange en 60 px, « 22M+ patients télésuivis », « 200+ établissements partenaires », « 13 ans », **sans source**. L'orange sur `#F6F6F6` fait 3,2:1 (acceptable en très grand seulement). Témoignage d'une cadre de chirurgie ambulatoire : « on ne passe plus que 1 ou 2 appels par jour ». Bloc sécurité exemplaire : ISO 27001 avec organisme, numéro et date du certificat (29 octobre 2025), HDS, RGPD avec DPO. **À reprendre** : le témoignage chiffré d'une cadre (persona Claire) et le bloc certifications avec numéro et date. **À éviter** : les chiffres sans source et l'animation d'entrée qui cache le titre. |

## Parcours (comment ça marche)

| # | Titre | Source | URL | Capture | À retenir |
|---|---|---|---|---|---|
| 9 | Medtech, Healthcare Service Landing Page, MultiQoS | Behance | https://www.behance.net/gallery/182360867/Medtech-Healthcare-Service-Landing-Page | Aucune | **Non vérifié** : Behance renvoie une erreur HTTP 400. Remplacé par le n° 23. |
| 10 | Cureety, espace patient | Site réel | https://www.cureety.com/en-us/patient | [choix](captures/10-cureety-patient.jpg) · [page patient](captures/10b-cureety-patient-hero.jpg) | À la première visite, une fenêtre propose deux cartes : « Patient or caregiver » (bouton vert `#487D4C`, texte blanc 4,9:1) et « Healthcare professional » (bouton bleu `#354D8C`, 8,1:1). La page patient : fond beige rosé, titre Seasonmix 68 px, graisse 420, `#080517`, texte en Ppmori (18 px relevés sur mobile). « You're not on your own between appointments », boutons « Contact us » (`#565269`, 7,5:1) et « Ask a question ». Puis « 94 % of patients feel more supported… » **sans source visible**, « $0 Free for patients », « Rx Available by prescription », 4 étapes numérotées (01 à 04) et un bloc **aidants** (« Report symptoms on their behalf »). **Correction** : pas de centre d'aide « activer son compte, se connecter », mais un formulaire de contact. La page rappelle que l'équipe soignante crée le compte. **À reprendre** : le choix de public à deux couleurs, le bloc aidants (Sophie), la phrase « votre équipe doit d'abord créer votre compte ». |
| 23 | Medical Test Kit Website, How It Works Section, Creliq (ajout) | Dribbble | https://dribbble.com/shots/26450174-Medical-Test-Kit-Website-How-It-Works-Section | [capture](captures/23-dribbble-creliq-how-it-works.jpg) | Remplace le n° 9. « Simple Steps », « How it works », « No confusion or delays ». Étapes en liste verticale reliées par un filet, l'étape active marquée par une icône sur fond vert clair et un trait noir, les autres en icône grise. À gauche, un visuel qui suit l'étape (photo et carte d'interface). Fond blanc, bleu-vert très clair en bord. **À reprendre** : la liste verticale avec l'étape active marquée par la forme (trait) et pas seulement la couleur ; 4 étapes pour Veilla, avec une illustration par étape. **À éviter** : la photo de banque d'images. |

## Tableau de bord soignant (produit)

| # | Titre | Source | URL | Capture | À retenir |
|---|---|---|---|---|---|
| 11 | Real-Time Patient Monitoring Dashboard, MD Jubaer Riyad | Behance | https://www.behance.net/gallery/213693587/Real-Time-Patient-Monitoring-Dashboard-UXUI-Design | Aucune | **Non vérifié** : erreur HTTP 400. Remplacé par le n° 22. |
| 22 | Remote Patient Monitoring Dashboard, Sayem (ajout) | Dribbble | https://dribbble.com/shots/27191544-Remote-Patient-Monitoring-Dashboard | [capture](captures/22-dribbble-rpm-dashboard.jpg) | Remplace le n° 11. Rangée de 4 indicateurs (patients suivis, alertes critiques, appareils hors ligne, nouvelles alertes) avec tendance, puis un tableau patients : statut en **pastille avec libellé** (« Critical » sur rose `#FFDCDC`, « Stable » sur vert d'eau, « Warning » sur ambre `#F3BA5B`), courbe de rythme cardiaque colorée selon le statut, bouton « View » bleu `#1E6BB3`. Noms fictifs. **À reprendre** : la rangée d'indicateurs et la pastille couleur + texte pour la capture annotée de Veilla. **À éviter** : la courbe colorée sans libellé et un rouge vif répété partout. |
| 12 | Medical Web Application, Brightlab | Dribbble | https://dribbble.com/shots/23641909--Medical-Web-Application-Changing-Healthcare-with-Web-App | [capture](captures/12-dribbble-brightlab-medical-webapp.jpg) | **Correction** : ce n'est pas une interface dans un cadre navigateur. C'est une application **côté patient** (« HealNetica », « Welcome, Ellis » : résultats en PDF, rendez-vous, ordonnances, blog, calendrier, réductions) posée en carte arrondie sur un fond dégradé lavande, accents violets (couleurs estimées à l'œil). **À reprendre** : la capture posée en carte sur un fond doux, sans chrome de navigateur. **À éviter** : la densité (7 blocs) et les rubriques commerciales. |
| 13 | Canvas Medical | Lapa Ninja (bloqué), site réel | Lapa : https://www.lapa.ninja/post/canvasmedical/ (Cloudflare). Vu à la place : https://www.canvasmedical.com/ | [capture](captures/13-canvas-medical.jpg) | Fond `#030B14`, hero dans une grande carte arrondie en dégradé bleu nuit, violet puis bordeaux. « Expect more from your EMR » en Open Sans 48 px, graisse 700, blanc. CTA orange `#FB923C` à texte sombre (8,7:1). L'interface est **schématisée** : des lignes grises à la place du texte, et 3 fragments mis en avant par un contour vert ou cyan (« Allergies », « Conditions »). Badge « Best in KLAS 2026 » sous le hero. **À reprendre** : le principe confirmé, montrer des fragments mis en avant plutôt qu'une capture entière et illisible. **À éviter** : le thème sombre et l'orange. |

## Accessibilité et clarté

| # | Titre | Source | URL | Capture | À retenir |
|---|---|---|---|---|---|
| 14 | Doxy.me | Land-book (bloqué), site réel | Land-book : https://land-book.com/websites/50420-the-simple-free-and-secure-telemedicine-platform-doxy-me (Cloudflare). Vu à la place : https://doxy.me/ qui redirige vers https://doxy.me/site/ | [capture](captures/14-doxy-me.jpg) | **Correction** : le titre n'est plus « simple, gratuit, sûr ». C'est un superlatif, « The world's most loved telehealth platform » (Suisse Int'l 58 px, graisse 450, `#232323`) ; les trois adjectifs ne restent que dans la balise `<title>`. Sous-titre « Join over 1.8M providers… », CTA turquoise `#5FD0C2` à texte sombre (8,5:1), vidéo d'une consultation. Sous le hero, une rangée de badges : « HIPAA-compliant », « SOC 2-certified », « GDPR-compliant »… Plus bas : « One URL », « No downloads », « No patient login ». Le site vise les soignants, pas les patients. **À reprendre** : la rangée de badges de conformité sous le hero, et la formule « rien à télécharger, pas de compte » pour le bloc patient. **À éviter** : le superlatif. |
| 15 | Medical Website Examples (29 sites) | One Page Love | https://onepagelove.com/tag/medical | [capture](captures/15-onepagelove-medical.jpg) | Confirmé : « 29 Real Examples », chaque fiche avec capture complète et points notables. Exemples affichés : Neuropelvic Surgery, CardiaTec (grands chiffres « 20M Lives Claimed Per Year »), Script Runner, Eigen Therapeutics, Aether Bio, TelMD. **À reprendre** : banque de comparaison pour la longueur de page et l'ordre des sections. |

## Mobile

Les 4 captures ci-dessous ont été faites en 390 × 844 px. Elles remplacent la référence Carbon Health, qui n'a pas pu être vue.

| # | Titre | Source | URL | Capture | À retenir |
|---|---|---|---|---|---|
| 16 | Carbon Health, modern primary & urgent care | Land-book | https://land-book.com/websites/14601-carbon-health-modern-primary-urgent-care | Aucune | **Non vérifié** : Land-book et https://carbonhealth.com/ sont bloqués par Cloudflare. Les tags cités (« Big Footer, Pastel Colors ») n'ont pas pu être confirmés. |
| M1 | Cureety, choix du public | Site réel | https://www.cureety.com/en-us/patient | [capture](captures/mobile-cureety-choix.jpg) | Sur mobile, la carte **patient passe en premier**, avec un bouton vert pleine largeur (276 × 48 px). La carte soignant suit, bouton bleu. Libellés « Enter » en 14 px. **À reprendre** : patient en premier et pleine largeur, exactement la règle du README. Veilla va plus loin : 64 px de haut et un libellé explicite en 20 px (« Je suis un patient »), pas « Enter ». |
| M2 | Cureety, page patient | Site réel | https://www.cureety.com/en-us/patient | [capture](captures/mobile-cureety.jpg) | Texte courant en 18 px, titre fin sur 2 lignes. Deux boutons côte à côte (118 × 48 et 127 × 48 px, libellés en 14 px). Le bouton de connexion est caché dans le menu. **À éviter** : cacher « Log in » dans le menu ; pour Veilla, « Accéder à mon espace » reste visible sans ouvrir le menu. |
| M3 | Resilience Oncology | Site réel | https://www.resilience.care/healthcare-providers/oncology | [capture](captures/mobile-resilience.jpg) | La fenêtre « professionnels de santé » ne s'est **pas affichée** sur mobile lors de notre visite (présente dans la page, mais masquée). Titre serif centré sur 3 lignes, un seul CTA centré « Request a demo », bande de photos. **À retenir** : si Veilla filtre un contenu pro, le filtre doit marcher aussi sur mobile, ou ne pas exister. |
| M4 | Doxy.me | Site réel | https://doxy.me/ | [capture](captures/mobile-doxy-me.jpg) | Titre en 52 px sur 4 lignes, sous-titre centré, puis la vidéo et le début des badges de conformité. Deux CTA côte à côte de **37 px de haut**, sous la cible tactile de 44 px. **À éviter** : c'est le contre-exemple de notre règle « deux CTA côte à côte de 40 px sur mobile ». |

## Palette et typographie

| # | Titre | Source | URL | Capture | À retenir |
|---|---|---|---|---|---|
| 17 | A Color Palette for a Medical Website That Feels Trustworthy, Not Icy | Pinterest (guide) | https://guide.pinterest.com/design/color-palette-for-medical-website/ | [capture](captures/17-pinterest-guide-palette.jpg) | Lisible sans compte. Confirmé : base neutre, un bleu dominant, le vert en second pour les signaux de soutien (succès, badges, séparateurs) ; « a full green and white palette » ferait penser aux compléments alimentaires. Le guide cite aussi des neutres chauds (« Champagne and Oxford Blue », « Eggshell ») contre l'éblouissement du blanc pur. **Correction** : il conseille un accent chaud (orange ou jaune) pour les CTA. Veilla ne le suit pas sur ce point : CTA bleu, car l'orange et le rouge signalent les alertes dans le produit. |
| 18 | Sage Organic Branding, dental clinic | Pinterest | https://www.pinterest.com/pin/wellness-branding-and-squarespace-design-for-organic-dental-clinic--609534130826660036/ | Aucune | **Non vérifié** : mur de connexion, pas de capture. Lisible : le titre de l'épingle a changé (« Custom Dental Squarespace Website layout medical logo design branding… ») et le texte alternatif décrit un logo « in green and white colors ». L'image entrevue derrière le mur est vert d'eau soutenu, pas sauge. Voir le n° 24. |
| 19 | Healthcare webdesign homepage green hex colors | Pinterest | https://www.pinterest.com/pin/816699713670139085/ | Aucune | **Non vérifié** visuellement (mur de connexion). La description confirme les codes `#b2dabc` et `#add4c5`, dans une bande de 5 verts (avec `#61af4b`, `#0c784b`, `#7cb464`) issue de ColorsWall. C'est un nuancier générique, pas une page d'accueil santé. La règle tient : tons pâles pour les fonds, **jamais pour le texte**. |
| 20 | Visilant, Transatlantico Studio | Behance (bloqué), page du studio | Behance : https://www.behance.net/gallery/237984219/Visilant (erreur 400). Vu à la place : https://transatlantico.studio/visilant/ | [capture](captures/20-transatlantico-visilant.jpg) | Étude de cas du studio. Visilant est une **association** de dépistage visuel par IA et smartphone ; le studio parle d'une « early-stage brand », d'une petite équipe sans marketing interne et d'un délai court. Identité construite sur la grille 5 × 5 des lettres de Sloan, symbole mi-œil mi-fleur, déclinée en marque, site, infographies et motion. Page en blanc chaud `#F2F0ED`, titres Söhne Buch 90 px, hero bleu nuit avec logo blanc. Résultat annoncé : « Increased credibility with investors and healthcare partners ». **À reprendre** : partir d'un détail médical réel pour fonder l'identité (pour Veilla, l'échelle de douleur ou le rythme quotidien). |
| 24 | Carely, Modern Healthcare Landing Page, Peter Jackson (ajout) | Dribbble | https://dribbble.com/shots/27709011-Carely-Modern-Healthcare-Landing-Page | [capture](captures/24-dribbble-carely-sage.jpg) | Complète les n° 18 et 19. Fond blanc cassé, titre noir très gras « Healthcare Made Human » avec « Made » en vert-de-gris pâle, CTA pilule vert sombre « Book an Appointment », icônes de services dans des cercles sauge pâle, rangée de chiffres (20k+, 98 %, 15+, 10+) sans source (couleurs estimées à l'œil). **À reprendre** : la sauge réservée aux fonds d'icônes et le vert sombre pour l'action. **À éviter** : un mot du titre en sauge pâle (contraste insuffisant), la photo de médecin souriant, les chiffres sans source. |

---

## Synthèse du moodboard

> **Ajustements du 2026-11-12**, justifiés par les captures : (1) la direction A intègre une **porte d'entrée à deux choix**, vue chez Cureety, Resilience et Implicity ; (2) la direction B est jugée moins froide que prévu, car Resilience et Cureety associent un titre serif ou semi-serif à un fond chaud sans paraître distants ; (3) la référence Withings de la direction C n'a pas pu être vérifiée. La palette et les tokens ne changent pas : les sites observés confirment le blanc chaud (`#F2F0ED` à `#FDFDF1` chez Visilant, Institute of Health, Heva) et un vert sombre pour l'action (Heva, Cureety).

### Direction A : « Clinique chaleureuse » (recommandée)
- Blanc chaud dominant, bleu profond pour les titres et les CTA, sauge pour les fonds de section et les badges de conformité.
- Choix du public dès le hero : « Je suis un patient » en sauge foncée, « Je suis un établissement » en bleu profond. Cureety (n° 10) fait exactement ce codage, vert pour le patient et bleu pour le soignant. Sur mobile, la carte patient passe en premier (M1).
- Captures produit nettes dans des cadres arrondis, fragments mis en avant plutôt qu'écran entier (n° 13, 22), illustrations au trait du parcours (4 étapes, n° 23).
- Rassurant, factuel, très lisible. Correspond au README et à la base neutre, bleu dominant, vert en soutien du guide n° 17.

### Direction B : « Éditorial scientifique »
- Grille éditoriale, titres en serif (Source Serif 4), chiffres en très grand avec appel de note et lien « Voir les sources », comme Resilience (n° 5).
- La section Preuves et Publications devient la colonne vertébrale (style revue médicale).
- Crédibilité maximale auprès des établissements. Moins froid que prévu si le fond reste chaud et le texte généreux (Resilience, Cureety), mais le bloc patient doit rester en sans-serif.

### Direction C : « Produit au premier plan »
- Hero en split : téléphone patient à gauche, tableau de bord soignant à droite. La référence Withings (n° 4) n'a pas pu être vue ; le principe reste à valider sur maquette. avaros.ai (n° 3) montre un téléphone central avec des bulles patient et médecin.
- Micro-animations sobres montrant le trajet d'une alerte, du patient à l'infirmière.
- Très démonstratif pour la levée, mais il faut veiller à `prefers-reduced-motion` et à la sobriété. Calmedica (n° 21) montre le risque : une animation d'entrée qui laisse le titre invisible.

### Palette recommandée (contrastes calculés sur #FAF8F4)

| Rôle | Hex | Usage | Contraste |
|---|---|---|---|
| Fond blanc chaud | `#FAF8F4` | Fond principal | Fond de référence |
| Texte | `#1E2A33` | Corps de texte | 13,8:1 |
| Bleu profond | `#1F3A5F` | Titres, CTA principal (texte blanc : 11,5:1) | 10,8:1 |
| Sauge foncée | `#4E6B57` | Liens secondaires, icônes, badges | 5,6:1 (AA) |
| Sauge | `#7A9A82` | Décor, illustrations uniquement | 2,9:1 (**jamais pour le texte**) |
| Sauge pâle | `#E3EBE4` | Fonds de section | texte #1E2A33 : 12,0:1 |
| Alerte | `#B3261E` | **Uniquement** pour les alertes dans l'interface montrée | 6,2:1 |

### Polices (Google Fonts)
- **Atkinson Hyperlegible** : corps de texte et interface, 18 px minimum (20 px pour le bloc patient).
- **Source Sans 3** : titres (graisses 600 et 700) ; en alternative pour la direction B : **Source Serif 4**.

### 3 « à ne pas faire »
1. **Du rouge ou de l'orange vif pour les CTA** : le rouge signifie « alerte » dans le produit, il ne doit pas apparaître ailleurs. Le guide n° 17 conseille l'inverse ; Canvas (n° 13) et Calmedica (n° 21) le font. Veilla ne suit pas.
2. **Des photos de banque d'images de médecins ou de patients souriants** : préférer l'équipe réelle, des captures et des illustrations. Le motif est partout dans les shots Dribbble (n° 1, 23, 24).
3. **Du texte gris clair ou sauge sur fond blanc cassé** pour faire « doux » : la cible patient âgée exige un contraste ≥ 4,5:1 partout. Implicity (n° 6) a un bouton à 3,8:1, Carely (n° 24) un mot du titre en sauge pâle.

---

## Design tokens

> Format design system. Noms en kebab-case, prêts pour des variables CSS. Contrastes calculés sur `#FAF8F4` (revérifiés le 2026-11-12).

### Couleurs

**Marque**

| Token | Hex | Usage |
|---|---|---|
| `color-brand-primary` | `#1F3A5F` | CTA principal, titres (10,8:1 ; texte blanc 11,5:1) |
| `color-brand-primary-hover` | `#162B47` | Survol et état pressé (13,5:1 ; texte blanc 14,3:1) |
| `color-brand-primary-light` | `#2D5A8A` | Liens (6,7:1) |
| `color-brand-secondary` | `#4E6B57` | Badges de conformité, icônes, liens secondaires (5,6:1) |
| `color-brand-secondary-strong` | `#3F5E49` | Fond du CTA patient (texte blanc 7,2:1) |
| `color-brand-secondary-soft` | `#7A9A82` | Décor et illustrations uniquement (2,9:1) |
| `color-brand-secondary-tint` | `#E3EBE4` | Fonds de section (texte #1E2A33 : 12,0:1) |

**Sémantiques** (toujours couleur + icône + libellé)

| Token | Hex | Contraste | Remarque |
|---|---|---|---|
| `color-success` | `#2E6B47` | 6,0:1 | Statut « conforme », envoi réussi |
| `color-alert` | `#B3261E` | 6,2:1 | **Seul rouge autorisé** : alertes patient dans les captures et erreurs de formulaire |
| `color-warning` | `#8A5A00` | 5,6:1 | Alerte modérée (niveau orange du tableau de bord) |
| `color-info` | `#1F5F8B` | 6,5:1 | Encadrés d'information (« En cas d'urgence, appelez le 15 ») |

**Neutres**

| Token | Hex | Usage |
|---|---|---|
| `color-neutral-0` | `#FFFFFF` | Cartes, champs |
| `color-neutral-50` | `#FAF8F4` | Fond de page (blanc chaud) |
| `color-neutral-100` | `#EEEAE3` | Fonds alternés |
| `color-neutral-300` | `#D6D0C6` | Séparateurs décoratifs (1,5:1, pas pour les bordures de champs) |
| `color-neutral-600` | `#5A6670` | Texte secondaire, bordures de champs (5,6:1) |
| `color-neutral-900` | `#1E2A33` | Texte principal (13,8:1) |

### Échelle typographique (base 18 px, ratio ≈ 1,25)

| Token | Police | Taille | Graisse | Interlignage |
|---|---|---|---|---|
| `text-display` | Source Sans 3 | 52 px (mobile 36) | 700 | 1,1 |
| `text-h1` | Source Sans 3 | 40 px (mobile 32) | 700 | 1,2 |
| `text-h2` | Source Sans 3 | 32 px (mobile 26) | 600 | 1,25 |
| `text-h3` | Source Sans 3 | 24 px | 600 | 1,3 |
| `text-stat` | Source Sans 3 | 56 px (mobile 40) | 700 | 1,0 (grands chiffres de la section Preuves) |
| `text-body-lg` | Atkinson Hyperlegible | 20 px | 400 | 1,6 (bloc patient) |
| `text-body` | Atkinson Hyperlegible | 18 px | 400 | 1,6 |
| `text-label` | Atkinson Hyperlegible | 18 px | 700 | 1,4 |
| `text-caption` | Atkinson Hyperlegible | 16 px | 400 | 1,5 (sources des chiffres, mentions) |

Repère observé : Doxy.me met son titre en 52 px sur mobile, sur 4 lignes, et ses CTA n'arrivent qu'à 474 px du haut (M4). Le `text-display` de Veilla passe à 36 px sur mobile pour laisser monter le CTA patient.

### Espacements (base 8 px)

`space-1` 4 · `space-2` 8 · `space-3` 12 · `space-4` 16 · `space-5` 24 · `space-6` 32 · `space-7` 48 · `space-8` 64 · `space-9` 96 · `space-10` 128 (entre sections, desktop) · gouttière mobile : 16 px.

### Rayons

`radius-sm` 4 px (badges, champs) · `radius-md` 8 px (boutons) · `radius-lg` 16 px (cartes, captures) · `radius-full` 999 px (avatars de l'équipe).

### Ombres (teintées bleu nuit)

- `shadow-sm` : `0 1px 2px rgba(30, 42, 51, 0.06)`
- `shadow-md` : `0 4px 16px rgba(30, 42, 51, 0.08)` (cartes de preuve)
- `shadow-lg` : `0 16px 40px rgba(30, 42, 51, 0.12)` (captures du tableau de bord, mockups)
- `focus-ring` : `0 0 0 3px #FAF8F4, 0 0 0 6px #2D5A8A`

### Motion

| Token | Valeur | Usage |
|---|---|---|
| `duration-fast` | 120 ms | Survol, focus |
| `duration-base` | 200 ms | Accordéons (FAQ, conformité) |
| `duration-slow` | 400 ms | Apparition de l'alerte dans la démo du parcours (direction C) |
| `ease-standard` | `cubic-bezier(0.2, 0, 0, 1)` | Par défaut |
| `ease-emphasized` | `cubic-bezier(0.3, 0, 0, 1.0)` | Entrées de mockups |
| `ease-exit` | `cubic-bezier(0.4, 0, 1, 1)` | Sorties |

`prefers-reduced-motion: reduce` : durées à 0 ms, la démo animée est remplacée par 4 images statiques numérotées. Le titre du hero n'est jamais animé à l'entrée : il doit être visible même si le script ne se lance pas (contre-exemple : Calmedica, n° 21).

---

## Composants clés

### Choix du public (hero)
- Deux cartes côte à côte sur desktop, empilées sur mobile avec **la carte patient en premier** (modèle : Cureety, n° 10 et M1).
- Carte patient : bouton `color-brand-secondary-strong` « Je suis un patient ». Carte établissement : bouton `color-brand-primary` « Je suis un établissement ». Libellés explicites, jamais « Entrer ».
- Intégré au hero, pas en fenêtre bloquante : le visiteur voit la promesse avant de choisir. Si un contenu doit être réservé aux professionnels (régime de publicité des DM, à valider avec les affaires réglementaires), la fenêtre de filtre propose toujours une sortie claire vers le chemin patient, comme Resilience (n° 5), et marche aussi sur mobile (M3).

### Bouton primaire (« Demander une présentation », « Je suis un établissement »)
- Fond `color-brand-primary`, texte blanc `text-label`, hauteur 52 px (56 px sur mobile), padding horizontal 24 px, `radius-md`.
- **États** : *repos* #1F3A5F · *survol* #162B47 · *focus* `focus-ring` · *pressé* #162B47 et translation de 1 px · *désactivé* fond #D6D0C6, texte #5A6670, raison affichée · *chargement* : spinner et « Envoi en cours… ».

### Bouton patient (« Je suis un patient », « Accéder à mon espace »)
- Fond `color-brand-secondary-strong` #3F5E49, texte blanc 20 px, hauteur **64 px** sur mobile, pleine largeur. Premier bouton sur mobile.
- Repère observé : Cureety fait 48 px de haut avec un libellé de 14 px (M1). Veilla vise plus grand pour des patients âgés.

### Bouton secondaire (« Voir les publications »)
- Transparent, bordure 2 px #1F3A5F, texte #1F3A5F. *Survol* fond #E3EBE4 · *focus* `focus-ring` · *désactivé* opacité 60 % et raison affichée.

### Carte de preuve
- Fond blanc, `radius-lg`, `shadow-md`, padding `space-6`. Contenu : un chiffre en `text-stat`, une légende en `text-body`, puis **obligatoirement** une ligne `text-caption` « Source : [étude], n = [x], [date] » avec un lien.
- Modèle observé : Resilience (n° 5), appel de note sur chaque chiffre et lien « Voir les sources ». Contre-exemples : Calmedica (n° 21), Institute of Health (n° 7), Cureety (« 94 % », n° 10).

### Badge de conformité
- Pastille `radius-sm`, fond #E3EBE4, icône et texte #3F5E49 (5,9:1) (« Hébergeur certifié HDS », « RGPD »). Un statut en cours s'affiche en style warning : « Marquage CE : en cours ».
- Une rangée de badges sous le hero, comme Doxy.me (n° 14). Dans la section Conformité, chaque certification porte son organisme, son numéro et sa date, comme Calmedica (n° 21).

### Mention réglementaire (pied de page)
- Une ligne `text-caption` sous le pied de page : statut du DM, classe, numéro de l'organisme notifié une fois obtenu, fabricant, date de mise à jour. Modèle : Resilience (« Class IIa medical device… CE 0459… Update : March 2026 »). Avant le marquage : « Logiciel en cours de marquage CE ».

### Formulaire établissement
- Champs : nom, établissement, fonction, e-mail professionnel, téléphone (facultatif), message (facultatif). Libellés au-dessus, champs de 52 px, bordure 2 px #5A6670.
- Aucune donnée de santé. Une mention le rappelle à côté du formulaire (« Patients : n'indiquez aucune information médicale ici »).

### À faire / À ne pas faire

| À faire | À ne pas faire |
|---|---|
| Chaque chiffre accompagné de sa source, son n et sa date | Grands chiffres sans légende ni source (Calmedica, Institute of Health) |
| Rouge réservé aux alertes (captures et erreurs) | Rouge ou orange vif pour les CTA ou la décoration |
| Statut réglementaire exact (« en cours » si c'est en cours) | « Certifié », « remboursé » par anticipation |
| Mention réglementaire datée en pied de page | Statut du DM introuvable sur le site |
| Niveau d'alerte = couleur + icône + texte | Pastille de couleur seule |
| CTA patient en premier et pleine largeur sur mobile | Deux CTA côte à côte de 40 px sur mobile (Doxy.me : 37 px) |
| Choix du public visible dans le hero, avec sortie vers le chemin patient | Fenêtre bloquante sans sortie pour le patient |
| Titre du hero visible sans attendre une animation | Intro vidéo ou animation qui masque le titre |
| Captures avec des données fictives clairement anonymisées | Captures avec de vrais noms de patients, même floutés |
| Libellés visibles au-dessus des champs | Placeholders utilisés comme libellés |
