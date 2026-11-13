# Benchmark visuel : Les Jours Tranquilles (silver économie / aide à domicile)

Le bench suit le brief client bloc par bloc : chaque inspiration est rattachée à une exigence précise de [`BRIEF-CLIENT.md`](BRIEF-CLIENT.md), les autres références sont rangées à côté avec leur raison.

> **Les Jours Tranquilles est fictive.** Les références sont réelles. Les URL d'origine viennent de résultats de recherche (novembre 2026), les références ajoutées ont été ouvertes le 2026-11-12.

## Limites, à lire en premier

- **Sites ouverts et capturés le 2026-11-12**, dans un navigateur Chrome piloté (viewport 1440×900, au-dessus de la ligne de flottaison, et 390×844 pour le mobile). Les couleurs et les polices citées ont été relevées dans la page (styles calculés), pas devinées. Les contrastes sont recalculés selon la formule WCAG 2.1.
- **Refonte du 2026-11-12** : les références ont été triées en **11 inspirations** et **13 références à côté**. Les captures sont rangées dans [`captures/inspis/`](captures/inspis/) et [`captures/a-cote/`](captures/a-cote/), sans changer les noms de fichiers ni les numéros. Le bench est réorganisé selon l'arborescence du brief. Rien n'a été supprimé : chaque référence à côté garde sa ligne et sa raison.
  - Le n° 9 est scindé : la page de tag Dribbble va à côté (contexte seulement), le shot Birdie qu'elle contient est une inspiration.
  - Les captures mobiles sont triées sur leur propre contenu : celle d'Ouihelp va dans `inspis/`, celles d'O2 et de Petits-fils dans `a-cote/` (contre-exemples), même si Petits-fils (n° 4) est une inspiration sur desktop.
  - La direction B est retirée et la direction C corrigée (voir « Directions »).
  - **Tokens corrigés** pour la cible du brief (corps de texte ≥ 7:1, ≥ 18 px partout) : `color-neutral-600`, les 4 couleurs sémantiques, l'anneau de focus, un nouveau `color-link`, et la suppression de `text-small` (16 px). Le détail est dans « Palette, polices, design tokens, composants ».
  - Deux composants du kit demandé par le brief (livrable 4) manquaient : le bloc tarif et le bloc avis. Ils sont ajoutés.
  - **Aucune nouvelle référence** : Dribbble renvoie désormais une page « Let's confirm you are human » (HTTP 405), non contournée. One Page Love ne contient rien d'utilisable pour les blocs manquants (détail dans « Galeries : requêtes lancées »).
- **12 références sur 16 vues et capturées** dans la session d'origine, dont 2 épingles Pinterest seulement en partie (n° 11 et 15 : le mur de connexion assombrit la page). **4 inaccessibles**, aucune protection n'a été contournée : n° 6 et 10 (Behance, erreur HTTP 400, remplacées par les n° 6 bis et 10 bis), n° 14 (épingle Pinterest supprimée), n° 16 (Land-book : challenge Cloudflare ; Lapa Ninja : « Sorry, you have been blocked »).
- **Corrections de la vérification** (détail dans chaque ligne) :
  - Petits-fils (n° 4) travaille en **mode mandataire** (la famille est l'employeur), l'inverse de notre modèle. La page services ne parle ni d'expérience, ni d'auxiliaire attitrée, ni de prix : critères et tarifs sont sur d'autres pages.
  - Cera (n° 5) redirige vers Home Healthcare Connected ; l'application famille n'y a aucun visuel.
  - O2 (n° 8) : visite et devis gratuits confirmés, pas de « contrat résiliable sans frais » ni de « remplaçante ». O2 (n° 13) : sur mobile, aucun numéro en haut.
  - Home Instead (n° 7) : 7 étapes non numérotées, pas 4.
  - Dribbble (n° 9) : 245 shots ; le téléphone de Birdie affiche une alerte de chute, pas un compte-rendu.
- **7 références ajoutées** dans la session d'origine (n° 6 bis, 10 bis, 17 à 21).
- **Passe du 2026-11-13** (entreprise fictive, aucun chiffre inventé) :
  - Il n'y a pas de client : l'ancienne liste de questions ouvertes devient la section **Arbitrages**, où chaque point est une décision.
  - Les chiffres propres à l'entreprise fictive (délais promis, note d'avis, taux de continuité, montants attendus de l'entreprise) sont retirés. Les chiffres observés sur les pages du bench restent.
  - **Photos d'équipe** : recherche de photos de banque d'images bloquée, Unsplash renvoie « Access Denied » et Pexels une vérification Cloudflare, non contournées. Décision : un bloc « Qui sommes-nous » court sans photo, et aucune photo de personne sur la démo (illustrations au trait). Les exigences de photo réelle sont retirées du bench.
- Aucun formulaire n'a été rempli ni envoyé. Sur Dribbble, les avatars et les noms de designers ont été masqués avant la capture. Les personnes visibles sont celles des photos publiées par les entreprises.

**Répartition** : 16 entrées d'origine (17 URL) et 7 ajoutées. Sites réels 8, Dribbble 7 (dont 1 page de tag), Pinterest 3, Behance 2 (inaccessibles), One Page Love 1, Awwwards 1, Land-book et Lapa Ninja 1 (inaccessibles, regroupés dans l'entrée 16).

---

## Couverture du brief

| Exigence du brief | Inspirations | Manque |
|---|---|---|
| 1. Hero (illustration au trait, « Vos parents chez eux, bien entourés », CTA « Être rappelé aujourd'hui », téléphone en grand) | 1, 3, 7, 10 bis, 18, 20 | Les inspirations sont photographiques : on en reprend la mise en page et le cadrage, pas la photo (voir « Arbitrages »). |
| 2. Les services (6 cartes : icône, titre, phrase) | 6 bis, 8 | Aucune grille de 6 cartes vue : seulement des pastilles (n° 6 bis) et un bandeau de 5 engagements (n° 8). |
| 3. Comment ça se passe (4 étapes numérotées, puis un premier point avec la famille) | 8, 7 | Aucun parcours numéroté en 4 étapes. Le seul process vu (n° 7) compte 7 étapes sans numéro. |
| Bloc transverse « Votre parent sort de l'hôpital ? » | 4 (forme de l'encart), 3 (délai affiché) | Aucun bloc sortie d'hôpital vu, ni délai de démarrage pour les prescripteurs. À écrire depuis le brief (option C de l'UX copy). |
| 4. Le lien avec la famille (maquette de téléphone, exemple de compte-rendu, choix SMS ou application) | 9 (Birdie), 17, 7 | Aucun vrai compte-rendu de passage vu, ni de choix SMS ou application. Les sites réels décrivent leur appli en texte (n° 5, 7). |
| 5. Tarifs et aides (tarif TTC, exemple de calcul, APA, crédit d'impôt, avance immédiate, sources officielles, devis gratuit) | 4, 3, 8 | Aucune explication APA et crédit d'impôt avec liens officiels n'a été relevée. |
| 6. Qui sommes-nous (bloc court sans photo : 2 ou 3 phrases, logo) | 4 (critères de formation) | Rien de bloquant : le bloc est du texte. |
| 7. Avis des familles (3 à 5 avis d'exemple, emplacement de la source et de la période, sans note ni nombre) | 8, 3 | Aucun bloc d'avis détaillé relevé : seulement des notes agrégées. |
| 8. Zone d'intervention et contact (carte illustrée, communes fictives, téléphone en très grand, formulaire nom + téléphone, horaires, adresse) | 18, 3 | Aucune carte ni liste de communes. Aucun bon formulaire à 2 champs (le n° 3 en a 4). |
| Pages annexes (Nous rejoindre, mentions, accessibilité, modération des avis) | 4 (critères de recrutement) | Rien sur les mentions, la déclaration d'accessibilité ou la modération des avis. |
| Mobile : `tel:` en haut de chaque écran, barre fixe | 3 (mobile), 7, 18 | Aucun site vu ne met un numéro cliquable en haut de l'écran mobile (voir « Mobile »). |
| Marque : crème, terracotta douce, olive ; Lora et Atkinson Hyperlegible | 1, 6 bis, 7, 17, 20 | Aucune référence n'utilise Atkinson Hyperlegible. Aucune n'associe terracotta et olive. |
| Visuels : illustrations au trait, personnes actives, aucune photo de personne | 6 bis (icônes au trait) | Aucune illustration de scène vue. Les photos des n° 1, 7, 18 et 20 servent pour le cadrage et l'ambiance, pas comme source d'image. |
| Accessibilité : corps ≥ 7:1 et ≥ 18 px, pas de texte sur photo sans voile, pas de carrousel | 1, 3, 7 | Le corps de 18 px n'a été relevé que sur le n° 21 (à côté). |
| Preuve « La même auxiliaire, semaine après semaine » | 8 (engagement « continuité de service ») | Aucun taux de continuité publié par un concurrent ; la démo n'en affiche pas non plus (voir « Arbitrages »). |
| Preuve « Le vrai prix, aides déduites » | 4 | Rien de bloquant. |
| Preuve « On vous rappelle aujourd'hui » (sans délai chiffré) | 4, 3 | Rien de bloquant. |
| Preuve « Les familles en parlent » (format vérifiable, avis d'exemple) | 8, 3 | Rien de bloquant. |
| Preuve « Service autorisé par le Département » | 3 (« Certifié SAD » dans la ligne de preuves) | Aucun numéro d'autorisation ni SAP affiché vu. La démo affiche « numéro de démonstration ». |
| RGPD : formulaire minimal, aucune case pré-cochée | aucune | Seul contre-exemple vu : le n° 3 (4 champs, case pré-cochée). |
| SEO local (ville, zone) | 10 bis (zone dans la pastille) | La ville dans le H1 (n° 21, à côté) heurte le titre imposé : voir « Arbitrages ». |

---

## Inspirations, bloc par bloc

### 1. Hero

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 1 | Honor, « Quality of life has no expiration date » (site réel, US), https://www.honorcare.com/home-care/ | [capture](captures/inspis/01-honor-home-care.jpg) | Fond pêche `#FFF6F0`, un seul bouton blanc sur brun `#662A12` (11,0:1), photo de deux hommes âgés qui rient dans un cadre arrondi, ton digne. À éviter : l'accroche orange `#E76124` à 3,2:1 et l'absence de numéro sur la page. | Visuel chaleureux dans un cadre arrondi (repris pour l'illustration) ; CTA unique ; duo crème + terracotta foncée. |
| 3 | Ouihelp, landing « aide à domicile de confiance » (site réel, FR), https://lp.ouihelp.fr/l/aide-domicile-confiance | [capture](captures/inspis/03-ouihelp-landing.jpg) | Pas de menu : le logo et « 01 89 72 41 76, numéro gratuit ». Le numéro en gros bouton-pilule dans le hero, texte bleu nuit `#002C5A` sur vert `#3ED096` (7,1:1). Sous le hero, une ligne de 4 preuves. À éviter : le sous-titre en 14 px blanc sur photo. | « Le téléphone en grand » dans le hero. |
| 7 | Home Instead, « Our process to provide quality senior care » (site réel, US), redirigée vers l'agence de St Charles | [hero](captures/inspis/07-home-instead-process.jpg) | H1 « Creating the Right Care Plan » en PP Editorial New (serif), 48 px, vert foncé `#2C4F26` (7,6:1), fond de page crème `#FAFFEE`, texte `#2C4F26` (9,1:1). Le numéro en pilule blanche dans l'en-tête. Photo d'une auxiliaire en polo qui montre un vase à une dame. À éviter : deux numéros différents sur la même page. | Titre en serif (Lora) sur crème ; téléphone en haut de l'écran ; personne active (scène à transposer en illustration). |
| 10 bis | Senior Care Website Redesign (Orbillo), Dribbble, https://dribbble.com/shots/27644508-Senior-Care-Website-Redesign-Healthcare-UI-UX-Project | [capture](captures/inspis/10-dribbble-senior-care-redesign.jpg) | Une pastille preuves + zone au-dessus du H1 (« BBB Accredited · A+ Rated · Serving Indiana & Ohio »), le numéro en lien texte juste à côté du CTA, un mot du H1 en serif italique. À éviter : la blouse médicale. | Preuves et zone visibles dès le hero ; CTA + téléphone côte à côte. |
| 18 | Sincere In-Home Care, Landing Page Design (Brandframer.com), Dribbble, https://dribbble.com/shots/27743802-Sincere-In-Home-Care-Landing-Page-Design | [capture](captures/inspis/18-dribbble-sincere-in-home-care.jpg) | Fond crème, numéro en pilule dans l'en-tête, puis « Call for Care » plein et « Request a Consultation » bordé, et dessous « Speak with a real person: (661) 888-4908 ». Photo naturelle d'une auxiliaire et d'une dame dans un salon. Le meilleur modèle de hiérarchie vu. | CTA « Être rappelé aujourd'hui » + téléphone en grand ; scène de salon à transposer en illustration. |
| 20 | The Legacy Senior Communities (Tegan Digital), Honorable Mention Awwwards du 24 septembre 2021, https://www.awwwards.com/sites/the-legacy-senior-communities | [capture](captures/inspis/20-awwwards-legacy-senior.jpg) | Un couple de seniors actifs qui marchent main dans la main dans un jardin, logo et titre en serif fin. Palette relevée par Awwwards : `#2779A7`, `#DF6C4F` (cousin de notre terracotta douce), blanc. À éviter : le titre blanc posé sur la photo ; avec nous, il faut un voile. | Personnes actives (à transposer en illustration) ; serif pour l'émotion. |

Détails repris de références à côté : un seul champ ou un seul bouton dans le hero (n° 2, Agedly) ; la note des avis au-dessus du titre (n° 19, CareHaven).

### 2. Les services

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 6 bis | AgeFree, Elder Care Branding and Identity Design (Techwitpro), Dribbble, https://dribbble.com/shots/27547230-AgeFree-Elder-Care-Branding-and-Identity-Design | [capture](captures/inspis/06-dribbble-agefree.jpg) | Pastilles de services à icône au trait avec un titre court (Free Consultation, Daily Support, Home Visits…). Accord vert sapin, crème, orange et jaune doux. À éviter : les silhouettes à canne et le mot « elders » (équivalent de « nos aînés », interdit). | Cartes « une icône, un titre, une phrase » ; palette olive + crème + terracotta. |
| 8 | O2, la méthode O2 (site réel, FR), https://www.o2.fr/aide-aux-personnes-agees/selon-o2/la-methode-o2 | [hero](captures/inspis/08-o2-methode.jpg) | Bandeau « Choisir O2 c'est » : 5 engagements à icône au trait, libellés courts. La méthode écrit « Ne pas infantiliser la personne ». À éviter : le H2 vert `#00BFA2` sur blanc (2,3:1). | Format des cartes de service ; ton respectueux. |

### 3. Comment ça se passe

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 8 | O2, la méthode O2 | [hero](captures/inspis/08-o2-methode.jpg) | « Visite gratuite et sans engagement » et « devis personnalisé, gratuit et sans engagement » écrits en toutes lettres, avec des micro-réassurances sous le CTA. | Étape 2 « visite d'évaluation gratuite à domicile » ; devis gratuit (arrêté du 17 mars 2015). |
| 7 | Home Instead, page process | [étapes](captures/inspis/07-home-instead-etapes.jpg) | Une liste d'étapes à icônes au trait. À éviter : 7 étapes sans numéro ; le brief en veut 4, numérotées. | Mise en forme des 4 étapes. |

### Bloc transverse : « Votre parent sort de l'hôpital ? »

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 4 | Petits-fils, nos services d'aide à domicile (site réel, FR), https://www.petits-fils.com/nos-services-aide-a-domicile/ | [services](captures/inspis/04-petits-fils-services.jpg) | Un encart de couleur pleine « Rappel immédiat, dans les 2 heures ouvrables » avec un bouton, détaché du reste de la page. À éviter : le bouton orange `#EF7D00` à texte blanc (2,8:1). | Forme de l'encart pour « Organiser une aide dès cette semaine », placé entre les sections 3 et 4. |
| 3 | Ouihelp, hero | [capture](captures/inspis/03-ouihelp-landing.jpg) | Le délai écrit dans le sous-titre : « disponible en 48h ». À éviter : ce sous-titre en 14 px blanc sur photo. | Un délai écrit dans l'encart, chez nous sans chiffre : « dès cette semaine » (option C de l'UX copy). |

### 4. Le lien avec la famille

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 9 | Birdie Family Landing Page (Koncepted), Dribbble, https://dribbble.com/shots/5413993-Birdie-Family-Landing-Page | [Birdie](captures/inspis/09-dribbble-birdie-famille.jpg) | Une maquette de téléphone à côté d'une courte liste de bénéfices (« Wellbeing reports, live updates after every visit »). À éviter : l'alerte « Fall detected in the living room » ; notre message doit rassurer, pas alerter. | Maquette de téléphone avec un exemple de compte-rendu. |
| 17 | Family Caregiver Mobile iOS App Design (Purrweb UI/UX Agency), Dribbble, https://dribbble.com/shots/27740425-Family-Caregiver-Mobile-iOS-App-Design | [capture](captures/inspis/17-dribbble-family-caregiver-app.jpg) | Une carte de résumé de journée : qui est passé, à quelle heure (« Leo checked in », « 3/4 care actions covered »). Fond olive et titre serif « Care, in relay. ». À éviter : les médicaments et toute donnée de santé ; le site n'en collecte aucune. | Contenu du compte-rendu (horaire, actions faites) ; olive + serif. |
| 7 | Home Instead, « Honor Family App » en bas de page | [étapes](captures/inspis/07-home-instead-etapes.jpg) | 6 puces de bénéfices (« Get a comprehensive update after every visit »…). Elles n'ont aucun visuel : c'est là que notre maquette fait la différence. | Liste de bénéfices à côté du téléphone. |

Détail repris d'une référence à côté : l'idée « chaque visite est enregistrée et visible par la famille » (n° 5, Home Healthcare Connected), à montrer et non à décrire.

### 5. Tarifs et aides

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 4 | Petits-fils, tarifs par agence, https://www.petits-fils.com/tarifs-petits-fils/ | [tarifs](captures/inspis/04-petits-fils-tarifs.jpg) | Le tableau de tarifs avec une colonne « Coût indicatif réel après crédit d'impôt » : à Bordeaux Chartrons, 35,50 € TTC de l'heure jusqu'à 25 h par semaine, et 17,75 € après crédit d'impôt. À éviter : l'en-tête blanc sur jaune `#F9AE00` (1,9:1). Modèle mandataire : on reprend la forme, et ce tarif public (revu le 2026-11-13 sur la [page de l'agence](https://www.petits-fils.com/nos-agences/agence-aide-a-domicile-bordeaux-chartrons/#tarifs)) sert de repère au tarif de démonstration du brief, marqué « tarif d'exemple ». | Tarif horaire TTC et exemple de calcul « aides déduites ». |
| 3 | Ouihelp, ligne de preuves sous le hero | [capture](captures/inspis/03-ouihelp-landing.jpg) | « Chèques CESU » et « avance immédiate » cités en une ligne, avec des pictos. | Mention de l'avance immédiate, **seulement si le service est inscrit auprès de l'Urssaf** (brief). |
| 8 | O2, la méthode O2 | [hero](captures/inspis/08-o2-methode.jpg) | « Devis personnalisé, gratuit et sans engagement » écrit en clair. | CTA « Recevoir un devis gratuit » ; devis gratuit obligatoire. |

### 6. Qui sommes-nous

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 4 | Petits-fils, page auxiliaires de vie, https://www.petits-fils.com/auxiliaires-de-vie/ | pas de capture (texte relevé sur la page) | Des critères écrits noir sur blanc : formation qualifiante ou certification Croix-Rouge, 3 ans d'expérience minimum, 3 références vérifiées. | Une phrase sur la formation des auxiliaires : diplômes nommés (DEAES, titre ADVF), sans chiffre inventé. |

Les n° 7 et 18 servaient de direction photo pour les portraits : sans objet depuis la décision « Qui sommes-nous » sans photo (voir « Arbitrages »). Ils restent des inspirations pour le hero.

### 7. Avis des familles

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 8 | O2, la méthode O2 | [avis](captures/inspis/08-o2-methode-avis.jpg) | « 4,7/5 sur 589 avis Google récoltés entre le 01/03/2026 et le 31/03/2026 » : note, nombre, source et période. | Format de l'en-tête du bloc avis : source et période de collecte (sans note ni nombre sur la démo) ; information sur le contrôle des avis (art. L111-7-2). |
| 3 | Ouihelp, ligne de preuves | [capture](captures/inspis/03-ouihelp-landing.jpg) | « Google 4,5/5 » et « plus de 2400 avis » repris juste sous le hero. | Position de la preuve sous le hero ; chez nous, la ligne cite la source des avis, sans note. |

### 8. Zone d'intervention et contact

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 18 | Sincere In-Home Care | [capture](captures/inspis/18-dribbble-sincere-in-home-care.jpg) | Le numéro répété en clair sous les boutons, avec « Speak with a real person », et la pastille « Locally owned & family operated ». | Téléphone en très grand ; ancrage local. |
| 3 | Ouihelp | [capture](captures/inspis/03-ouihelp-landing.jpg) | Le numéro écrit en clair avec « numéro gratuit » à côté. À éviter : le formulaire à 4 champs et la case de consentement **pré-cochée**. | Téléphone en très grand ; contre-exemple pour le formulaire nom + téléphone. |

Détail repris d'une référence à côté : la ville écrite dans le titre principal (n° 21, The Legacy), utile au SEO local mais incompatible avec le H1 imposé (voir « Arbitrages »).

### Pages annexes

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 4 | Petits-fils, page auxiliaires de vie | pas de capture | Les critères de recrutement chiffrés. À éviter : « Accessibilité : Non conforme » en pied de page. | Page « Nous rejoindre » ; déclaration d'accessibilité. |

---

## Mobile

Exigences du brief : numéro `tel:` **en haut de chaque écran**, en barre fixe sur mobile ; formulaire de rappel en 2 champs envoyé en moins de 20 s ; corps ≥ 18 px ; cibles ≥ 48 px ; prix réel trouvé en moins de 30 s sur mobile.

**Observé en 390×844**

| Site | Capture | Ce qu'on observe | Exigence du brief |
|---|---|---|---|
| Ouihelp (n° 3) | [capture](captures/inspis/mobile-ouihelp.jpg) | En-tête collant de 64 px avec un bouton vert à icône de rappel (lien `#`, sans libellé accessible). Le lien `tel:` de l'en-tête est masqué sur mobile. Dans le hero, le numéro en grand bouton vert (vrai lien `tel:`), puis « Être rappelé » en blanc. L'accroche est en 14 px blanc sur photo. Le formulaire n'est pas au premier écran. | Inspiration pour le bouton-numéro du hero ; contre-exemple pour l'en-tête et le 14 px. |
| O2 (n° 13) | [capture](captures/a-cote/mobile-o2.jpg) | Un bandeau « Espace Salarié · Espace Client », puis un en-tête de 80 px. Aucun numéro en haut. Une barre fixe en bas, 50 px, en 3 aplats à icône seule : les libellés existent dans le code mais ne s'affichent pas, et le combiné mène à une page de rappel, pas à un appel. Le bouton d'accessibilité chevauche le bouton devis. Le seul lien `tel:` est tout en bas. | Contre-exemple : barre fixe sans numéro, icône seule. |
| Petits-fils (n° 4) | [capture](captures/a-cote/mobile-petits-fils.jpg) | Le bandeau « À la recherche d'un emploi ? » occupe la première ligne. Aucun numéro sur la page. Le premier appel à l'action est l'encart « Rappel immédiat ». La note 4,5/5 visible sur desktop disparaît. | Contre-exemple : aucun numéro, preuve perdue sur mobile. |

**À retenir** : aucun des 3 sites ne met un numéro cliquable en haut de l'écran mobile, et les deux qui proposent une action fixe poussent la demande de rappel, pas l'appel. L'exigence du brief est donc un vrai différenciant. Recommandations :
- une barre d'appel fixe en haut, avec le numéro **écrit en clair** et le libellé « Appeler le 0X XX XX XX XX » (UX copy du brief), jamais une icône seule (contrairement à O2) ;
- un seul numéro, identique partout, en vrai lien `tel:` (Home Instead en affiche deux, n° 7 ; celui de Home Healthcare Connected est cassé, n° 5) ;
- le formulaire de rappel en 2 champs, sans case pré-cochée (contrairement à Ouihelp, n° 3) ;
- un corps d'au moins 18 px, y compris sur photo et avec un voile (Ouihelp descend à 14 px) ;
- la preuve des avis gardée sur mobile (Petits-fils perd sa note).

---

## Directions

Le brief ne fixe pas de nombre de pistes. Deux directions restent, toutes deux dans la marque (crème, terracotta douce, olive, Lora et Atkinson Hyperlegible) et dans le ton du brief. Quelle que soit la direction, le bloc « lien avec la famille » montre un vrai exemple de compte-rendu : c'est la différence clé de l'entreprise et aucun concurrent vu ne la montre.

**Direction B « Carnet de famille » retirée** : elle reposait sur des comptes-rendus présentés comme des notes manuscrites et des portraits en polaroïd, ce qui demande une écriture manuscrite hors des deux polices imposées par le brief. Son seul élément fort, l'exemple de compte-rendu, est obligatoire dans toutes les directions (bloc 4).

### Direction A : « Maison chaleureuse » (recommandée)
- Fond crème, titres en Lora, CTA terracotta foncée, olive pour les icônes et les séparateurs. Le secteur a ses meilleurs exemples dans cette veine : Honor (n° 1, fond pêche et CTA brun), Home Instead (n° 7, serif vert foncé sur crème), AgeFree (n° 6 bis, vert profond, crème et orange). Aucun n'associe terracotta et olive : la palette reste distinctive.
- Illustrations au trait, personnes actives, cadres arrondis, beaucoup d'air ; cadrage et ambiance repris des photos d'Honor (n° 1), The Legacy (n° 20) et Sincere (n° 18). Aucune photo de personne.
- Lien famille en maquette de téléphone à côté d'une courte liste (n° 9, n° 17).
- Évoque le foyer, pas l'hôpital.

### Direction C : « Service clair »
- Fond crème `#FBF5EC`, cartes blanches, aplats olive, grandes cartes de service, tarifs très visibles. **Corrigé** : la version précédente posait un fond blanc, hors de la palette crème du brief.
- Le hero de Sincere (n° 18) en est le meilleur modèle : une action pleine, une bordée, le numéro répété en clair. La pastille preuves + zone d'Orbillo (n° 10 bis), la ligne de preuves d'Ouihelp (n° 3) et le tableau de Petits-fils (n° 4) complètent.
- Maximise la conversion, au risque de paraître moins humain.

---

## Palette, polices, design tokens, composants

### Palette recommandée (contrastes calculés sur #FBF5EC)

Les couleurs de marque ne changent pas. **Corrigé** : la terracotta foncée `#9E4A2F` servait aussi aux liens, à 5,6:1, sous la cible de 7:1 du brief pour le corps de texte. Les liens passent sur une terracotta plus sombre. Le titre orange d'Honor à 3,2:1 (n° 1) confirme la règle « décor seulement » pour la terracotta douce.

| Rôle | Hex | Contraste |
|---|---|---|
| Crème (fond) | `#FBF5EC` | fond de référence |
| Crème foncée (sections) | `#F3E6D3` | texte #2B2420 : 12,4:1 |
| Texte | `#2B2420` | 14,1:1 |
| Terracotta foncée (boutons) | `#9E4A2F` | texte blanc sur le bouton : 6,0:1. **Pas pour du texte courant** (5,6:1) |
| Terracotta sombre (liens dans le texte) | `#743522` | 8,5:1 ; 7,5:1 sur la crème foncée |
| Terracotta douce (décor) | `#C8775A` | 3,1:1 ; texte blanc dessus : 3,4:1 (**décor ou grands éléments seulement**) |
| Olive foncée (titres secondaires, icônes) | `#4A5628` | 7,3:1 (6,4:1 sur la crème foncée, titres ≥ 24 px seulement) ; texte blanc : 7,9:1 |
| Olive | `#6B7B3A` | 4,3:1 (texte ≥ 24 px ou icônes seulement) |

### Polices (Google Fonts)
- **Lora** (titres, 600 et 700).
- **Atkinson Hyperlegible** (texte et interface, 18 px minimum partout, y compris mentions légales ; 20 px recommandé sur mobile).

### 3 « à ne pas faire »
1. **Des gros plans de mains ridées, de cannes ou de fauteuils roulants, et des blouses médicales** (vus aux n° 2, 5, 6 bis et 10 bis) : ça infantilise, ça angoisse l'acheteur et ça confond aide à domicile et soin.
2. **Un carrousel automatique dans le hero** : interdit par le brief, illisible pour les seniors, et il masque le numéro.
3. **De la terracotta douce (#C8775A) pour du texte ou un bouton avec texte blanc** : le contraste est insuffisant (3,1:1 sur le crème, 3,4:1 en texte blanc).

### Design tokens

> Format design system. Noms en kebab-case, valeurs prêtes à passer en variables CSS (`--color-brand-primary`, etc.). Contrastes calculés sur `#FBF5EC`, puis sur `#F3E6D3` quand le texte peut y être posé. Cible du brief : ≥ 7:1 pour tout texte de taille courante sur les deux fonds.

#### Couleurs

**Marque**

| Token | Hex | Usage |
|---|---|---|
| `color-brand-primary` | `#9E4A2F` | Fond des boutons (texte blanc 6,0:1). Pas pour du texte |
| `color-brand-primary-hover` | `#7F3A24` | Survol et état pressé des boutons (texte blanc 8,3:1) |
| `color-link` | `#743522` | **Ajouté.** Liens dans le texte courant, soulignés (8,5:1 ; 7,5:1 sur la crème foncée). Survol : soulignement épaissi |
| `color-brand-primary-soft` | `#C8775A` | Illustrations, filets, puces décoratives |
| `color-brand-secondary` | `#4A5628` | Titres secondaires, icônes (7,3:1) |
| `color-brand-secondary-strong` | `#3A4520` | Texte sur fond olive clair (9,4:1) |
| `color-brand-secondary-soft` | `#6B7B3A` | Icônes, grands chiffres ≥ 24 px |

**Sémantiques** (toujours accompagnées d'une icône et d'un texte, jamais la couleur seule). **Corrigées** : les messages d'erreur sont en 18 px (brief), donc du texte courant ; les anciennes valeurs étaient entre 5,5 et 6,8:1.

| Token | Hex | Contraste | Ancienne valeur |
|---|---|---|---|
| `color-success` | `#2E521C` | 8,3:1 ; 7,3:1 sur la crème foncée | `#3F6B2A` (5,8:1) |
| `color-error` | `#86281F` | 8,3:1 ; 7,3:1 sur la crème foncée. Proche de la terracotta, d'où l'obligation de l'icône et du libellé « Erreur » | `#A8322A` (6,1:1) |
| `color-warning` | `#664300` | 8,2:1 ; 7,2:1 sur la crème foncée | `#8A5A00` (5,5:1) |
| `color-info` | `#264B66` | 8,5:1 ; 7,5:1 sur la crème foncée | `#2F5A7A` (6,8:1) |

**Neutres**

| Token | Hex | Usage |
|---|---|---|
| `color-neutral-0` | `#FFFFFF` | Cartes, champs de formulaire |
| `color-neutral-50` | `#FBF5EC` | Fond de page |
| `color-neutral-100` | `#F3E6D3` | Fonds de section alternés |
| `color-neutral-300` | `#D9CBB6` | Bordures décoratives (1,5:1, **pas pour les bordures de champs**) |
| `color-neutral-600` | `#504641` | Texte secondaire et bordures de champs (8,5:1 ; 7,4:1 sur la crème foncée). **Corrigé** : `#5E534C` était à 6,9:1 |
| `color-neutral-900` | `#2B2420` | Texte principal (14,1:1) |

#### Échelle typographique (base 18 px, ratio ≈ 1,25)

| Token | Police | Taille | Graisse | Interlignage |
|---|---|---|---|---|
| `text-display` | Lora | 48 px (mobile 36) | 700 | 1,15 |
| `text-h1` | Lora | 40 px (mobile 32) | 700 | 1,2 |
| `text-h2` | Lora | 32 px (mobile 28) | 600 | 1,25 |
| `text-h3` | Lora | 24 px | 600 | 1,3 |
| `text-body-lg` | Atkinson Hyperlegible | 20 px | 400 | 1,6 |
| `text-body` | Atkinson Hyperlegible | 18 px | 400 | 1,6. Sert aussi aux mentions légales et au pied de page |
| `text-label` | Atkinson Hyperlegible | 18 px | 700 | 1,4 |
| `text-phone` | Atkinson Hyperlegible | 28 px (barre mobile 22) | 700 | 1,2 |

**Corrigé** : `text-small` (16 px, mentions légales) est supprimé. Le brief demande un corps de texte ≥ 18 px partout (critères de réussite).

Longueur de ligne : 60 à 70 caractères maximum.

#### Espacements (base 8 px)

`space-1` 4 · `space-2` 8 · `space-3` 12 · `space-4` 16 · `space-5` 24 · `space-6` 32 · `space-7` 48 · `space-8` 64 · `space-9` 96 (entre sections, desktop) · gouttière mobile : 16 px (20 px recommandé).

#### Rayons

`radius-sm` 6 px (champs, badges) · `radius-md` 12 px (boutons) · `radius-lg` 20 px (cartes, photos) · `radius-full` 999 px (pastilles, avatars).

#### Ombres (teintées brun, jamais noir pur)

- `shadow-sm` : `0 1px 2px rgba(43, 36, 32, 0.08)` (champs)
- `shadow-md` : `0 4px 12px rgba(43, 36, 32, 0.10)` (cartes)
- `shadow-lg` : `0 12px 32px rgba(43, 36, 32, 0.14)` (barre d'appel fixe, modale)
- `focus-ring` : `0 0 0 3px #FBF5EC, 0 0 0 6px #264B66` (double anneau visible sur tous les fonds ; suit le nouveau `color-info`)

#### Motion

| Token | Valeur | Usage |
|---|---|---|
| `duration-fast` | 120 ms | Survol, focus |
| `duration-base` | 200 ms | Ouverture d'accordéon (FAQ, tarifs) |
| `duration-slow` | 320 ms | Apparition de la barre d'appel, message de succès |
| `ease-standard` | `cubic-bezier(0.2, 0, 0, 1)` | Par défaut |
| `ease-exit` | `cubic-bezier(0.4, 0, 1, 1)` | Sorties |

`@media (prefers-reduced-motion: reduce)` : toutes les durées passent à 0 ms. Pas de parallaxe, pas d'apparition au scroll sur le texte.

### Composants clés

#### Bouton primaire (« Être rappelé aujourd'hui »)
- Fond `color-brand-primary`, texte blanc `text-label`, hauteur minimale 56 px, padding horizontal 24 px, `radius-md`.
- **États** : *repos* #9E4A2F · *survol* #7F3A24 · *focus* `focus-ring` · *pressé* #7F3A24 avec translation de 1 px · *désactivé* fond #D9CBB6, texte #504641, curseur « not-allowed », et la raison expliquée à côté · *chargement* : spinner, libellé « Envoi en cours… », bouton désactivé.

#### Bouton secondaire (« Voir les tarifs », « Appeler le 0X XX XX XX XX »)
- Fond transparent, bordure 2 px `color-brand-secondary`, texte `color-brand-secondary`, même hauteur que le primaire.
- **États** : *survol* fond #F3E6D3 · *focus* `focus-ring` · *pressé* fond #E9D9C1 · *désactivé* bordure et texte #504641 à 60 %.

#### Carte de service
- Fond blanc, `radius-lg`, `shadow-md`, padding `space-6`, une icône olive au trait de 40 px (n° 6 bis, n° 8), un titre `text-h3` et une phrase `text-body`. Toute la carte est cliquable si elle mène quelque part (et alors un seul lien).

#### Bloc tarif (ajouté : demandé dans le kit du brief)
- Tarif horaire TTC en `text-h2`, puis un exemple de calcul en tableau à 3 colonnes : prix TTC, aides déduites (APA si perçue, crédit d'impôt de 50 %), coût réel. Forme reprise du tableau de Petits-fils (n° 4). Montants : le tarif de démonstration du brief (35,50 € TTC, calé sur le tarif public de Petits-fils Bordeaux Chartrons, vu le 2026-11-13), marqué « tarif d'exemple ».
- En-têtes de tableau en `color-neutral-900` sur `color-neutral-100`, jamais de texte blanc sur une couleur claire (contre-exemple n° 4, 1,9:1).
- Mention « sous réserve de la législation en vigueur », lien vers la [fiche F12 de Service Public](https://www.service-public.gouv.fr/particuliers/vosdroits/F12) en `color-link`, CTA primaire « Recevoir un devis gratuit ».

#### Bloc avis (ajouté : demandé dans le kit du brief)
- En tête : source et période de collecte, sur le modèle d'O2 (n° 8), avec un lien vers la source. Pas de note ni de nombre d'avis : la démo n'a pas de vrais avis.
- 3 à 5 cartes blanches `radius-lg` : texte de l'avis en `text-body`, prénom ou initiale, date, et l'étiquette « avis d'exemple ». Pas de carrousel automatique.
- Une ligne qui dit si les avis sont contrôlés et comment, avec un lien vers la page de modération (art. L111-7-2).

#### Formulaire de rappel
- 2 champs : « Votre nom », « Votre téléphone » (`type="tel"`, `autocomplete="tel"`). Libellés **au-dessus** des champs, jamais en placeholder seul.
- Champs de 56 px de haut, bordure 2 px #504641, focus `focus-ring`, erreur : bordure `color-error`, icône et message de 18 px sous le champ, annoncé avec `aria-live="polite"`, aucune donnée effacée.
- Mention RGPD d'une ligne et lien vers la politique de confidentialité. Aucune case pré-cochée.

#### Barre d'appel mobile
- Fixée en haut, 56 px, fond `color-neutral-0`, `shadow-lg`, numéro en `text-phone` cliquable (`tel:`), icône téléphone et libellé « Appeler le 0X XX XX XX XX ».

#### À faire / À ne pas faire

| À faire | À ne pas faire |
|---|---|
| Libellés de bouton à verbe d'action précis (« Être rappelé aujourd'hui ») | « Envoyer », « Valider », « En savoir plus » |
| Cibles tactiles ≥ 48 × 48 px, espacées d'au moins 8 px | Liens texte collés les uns aux autres dans le pied de page |
| Libellés visibles au-dessus des champs | Placeholder seul comme libellé |
| Erreur = icône + texte + couleur | Bordure rouge seule |
| Numéro cliquable identique partout | Numéro en image, ou différent selon les pages (2 numéros chez Home Instead, n° 7) |
| Case de consentement décochée par défaut | Case pré-cochée (Ouihelp, n° 3) |
| Source et période de collecte des avis (O2, n° 8) ; avis d'exemple marqués comme tels | Note seule, sans source ni date |
| Illustrations au trait de personnes actives | Photos de seniors stéréotypés (visages en gros plan, blouses, cannes) |
| Respect de `prefers-reduced-motion` | Carrousels automatiques, parallaxe |

---

## Arbitrages

- **H1 et SEO local** : on garde le H1 « Vos parents chez eux, bien entourés », sans ville, et on place la ville dans un surtitre au-dessus du H1 et dans la balise `title`. Le titre reste simple pour les seniors et la requête locale reste couverte. La démo n'a pas de ville réelle : le surtitre affiche « Aide à domicile · votre ville ».
- **Libellé du CTA du hero** : « Être rappelé aujourd'hui » partout, parce que c'est la version la plus précise (UX copy, section 9). L'arborescence du brief est alignée.
- **Preuves** : on n'affiche aucun taux de continuité, parce qu'aucun chiffre réel n'existe. « La même auxiliaire » s'appuie sur la remplaçante présentée à l'avance, et le bloc 4 montre un exemple de compte-rendu rédigé par nous, marqué « exemple ».
- **Photos d'équipe** : Unsplash et Pexels ont bloqué le navigateur le 2026-11-13. On fait un bloc « Qui sommes-nous » de 3 phrases avec le logo, sans photo, et le hero passe à une illustration au trait.
- **Tarif** : on affiche un tarif de démonstration calé sur le tarif public de Petits-fils Bordeaux Chartrons (35,50 € TTC de l'heure, vu le 2026-11-13), marqué « tarif d'exemple ». L'exemple de calcul est notre différence la plus utile, et un prix inventé est exclu.
- **Avis** : le bloc avis garde son format vérifiable (source, période, modération) mais ne contient que des avis d'exemple, étiquetés, sans note ni nombre. Un faux score serait une donnée inventée.

---

## À côté

| # | Référence | Capture | Pourquoi à côté |
|---|---|---|---|
| 2 | Agedly, a Home Care Service for Seniors Landing Page (10am Studio), Dribbble, https://dribbble.com/shots/16641466-Agedly-a-Home-Care-Service-for-Seniors-Landing-Page-Animated | [capture](captures/a-cote/02-dribbble-agedly.jpg) | Photo d'une soignante en blouse qui enlace une dame en fauteuil roulant, gros plan de mains sur une canne : le brief veut des personnes actives et jamais de gros plans sur des mains ridées. Vidéo animée de 30 s. Seul détail repris : un seul champ ou bouton dans le hero (bloc 1). |
| 5 | Cera, Care at Home, https://ceracare.co.uk/home-care, redirigée vers https://homehealthcareconnected.co.uk/home-care | [capture](captures/a-cote/05-cera-home-care.jpg) | H1 en police manuscrite Kinder Boy et cœurs dessinés : hors des deux polices de marque. Auxiliaire en blouse. La « Family App » tient en une phrase, sans visuel, alors que le bloc 4 demande une maquette. Lien `tel:` cassé (`tel:"0330 123 9180"`). Le CQC n'est pas cité. Détail repris : l'idée de visite enregistrée et visible par la famille (bloc 4). |
| 6 | Senior care branding (dont « Seniare »), Behance, https://www.behance.net/search/projects/senior%20care%20branding | inaccessible | Non vérifié : erreur HTTP 400 renvoyée au navigateur automatisé. Remplacée par le n° 6 bis. |
| 9 | Elderly care tag (page de tag), Dribbble, https://dribbble.com/tags/elderly-care | [tag](captures/a-cote/09-dribbble-elderly-care.jpg) | Contexte seulement : 245 shots mêlant sites, illustration d'un robot qui aide une dame à traverser et un logo sans rapport. Le shot Birdie qu'elle contient est une inspiration (bloc 4). |
| 10 | Home care website (dont « Senior Care Website Redesign »), Behance, https://www.behance.net/search/projects/home%20care%20website | inaccessible | Non vérifié : erreur HTTP 400. Le projet du même titre est le n° 10 bis. |
| 11 | Eldcare, Senior Living WordPress Theme, Pinterest, https://www.pinterest.com/pin/973340538222802684/ | [capture partielle](captures/a-cote/11-pinterest-eldcare.jpg) | Non vérifié : mur de connexion, seule la vignette reste lisible ; la fiche ThemeForest bloque par Cloudflare, contrastes non vérifiables. Même famille que le n° 6 bis (vert profond, accent chaud). |
| 12 | Health & Healthcare Website Examples, One Page Love, https://onepagelove.com/tag/health | [capture](captures/a-cote/12-onepagelove-health.jpg) | Contexte seulement : « 78 Real Examples » (chirurgie, IA, dentiste, SafeStep…), aucun service d'aide aux seniors ; les recherches « senior », « elderly », « home care », « retirement » ne donnent rien. |
| 13 | O2, aide à domicile des personnes âgées, https://www.o2.fr/aide-aux-personnes-agees/aide-a-domicile, redirigée vers https://www.o2.fr/aide-aux-personnes-agees | [desktop](captures/a-cote/13-o2-aide-a-domicile.jpg), [mobile](captures/a-cote/mobile-o2.jpg) | Contre-exemple : bouton « Obtenir un devis » en blanc sur jaune `#E7BA63` (1,8:1), sous le minimum AA du brief ; le seul lien `tel:` (02 43 72 02 02) est en pied de page, et sur mobile aucun numéro en haut, alors que le brief l'exige en haut de chaque écran. Cité dans « Mobile ». |
| 4 (mobile) | Petits-fils en 390×844 | [mobile](captures/a-cote/mobile-petits-fils.jpg) | Contre-exemple : aucun numéro sur la page mobile (brief : `tel:` en haut de chaque écran), note des avis perdue. Le n° 4 reste une inspiration sur desktop. Cité dans « Mobile ». |
| 14 | Elderly Care Wix Studio Website Template, Pinterest, https://in.pinterest.com/pin/elderly-care-wix-studio-website-template-inhome-caregiver-senior-care-assisted-living-nursing-homes-in-2025--4602749301043693056/ | inaccessible | Non vérifié : épingle supprimée (redirection vers https://in.pinterest.com/ideas/). |
| 15 | 12 Assisted Living Website Themes ideas, Pinterest (tableau), https://www.pinterest.com/cricketpond/assisted-living-website-themes/ | [capture partielle](captures/a-cote/15-pinterest-assisted-living.jpg) | Contre-exemple : gros plans de visages de seniors souriants, équipes en blouse, thèmes génériques d'il y a 9 ans ; le brief veut des personnes actives, et la démo n'utilise aucune photo de personne. Sert à repérer les clichés. |
| 16 | Health & fitness, Land-book et Lapa Ninja, https://land-book.com/?industry=health-and-fitness et https://www.lapa.ninja/category/health-fitness/ | inaccessible | Non vérifié : challenge Cloudflare persistant sur Land-book, « Sorry, you have been blocked » sur Lapa Ninja. |
| 19 | CareHaven, Senior Care & Home Assistance Website Design (Trexa Lab), Dribbble, https://dribbble.com/shots/27047677-CareHaven-Senior-Care-Home-Assistance-Website-Design | [capture](captures/a-cote/19-dribbble-carehaven.jpg) | Un chiffre absurde (« 5k% ») et des logos Slack et Dropbox sans rapport : contraire aux preuves vérifiables que demande le brief (section 5, avis au format vérifiable). Détail repris : la note des avis au-dessus du H1 (bloc 1). |
| 21 | The Legacy Senior Communities (site actuel), https://thelegacyseniorcommunities.org/ | [capture](captures/a-cote/21-legacy-senior-site.jpg) | H1 blanc en Cormorant 600, 65 px, posé sur photo sans voile : le brief interdit le texte sur photo sans voile. Lieu de vie de luxe (« Luxury Senior Living in Dallas, TX »), hors du ton du brief. Détails repris : la ville dans le titre (bloc 8, voir « Arbitrages ») ; corps en Work Sans 18 px. |

**Clichés croisés** : fauteuil roulant et mains sur une canne (n° 2), blouses médicales (n° 2, 5, 10 bis), silhouettes à canne (n° 6 bis), gros plans de visages souriants (n° 15), alerte de chute (n° 9), cœurs dessinés et police manuscrite (n° 5), chiffres absurdes et faux logos clients (n° 19).

---

## Galeries : requêtes lancées

| Plateforme | Requêtes ou pages | Résultat |
|---|---|---|
| Dribbble (session d'origine) | « senior care branding », « home care website », « senior care website », « seniare », tag « elderly-care » | Retenues : n° 6 bis, 9, 10 bis, 17, 18, 19. Aucun shot « Seniare ». |
| Dribbble (refonte, 2026-11-12) | Recherche « home care how it works », tag « home-care » | Page « Let's confirm you are human » (HTTP 405). Non contournée, aucune référence. |
| Awwwards | « senior », « home care », « elderly » | Retenu : n° 20. Non retenus : un modèle « Senior Care » (wCopilot, nominé en 2023, gabarit générique) et Canary Care (télésurveillance, nominé en 2025, autre métier). |
| One Page Love (session d'origine) | Tag « health », recherches « senior », « elderly », « home care », « retirement » | Aucun site d'aide aux seniors (n° 12). |
| One Page Love (refonte, 2026-11-12) | Sections « How It Works » (56 premiers exemples chargés) et « Team » (39 premiers) ; recherches « care », « nursing », « carer », « family », « cleaning », « therapy » | Rien d'utilisable pour les blocs 3, 6 et 8 : agences, SaaS et studios. « Team » de LAVA dental Studio : portraits en tenue médicale, hors du brief. Putzengel (ménage, Vienne) : site hors ligne, style illustratif hors ton. « nursing » et « carer » : aucun résultat. |
| Behance | Recherches des n° 6 et 10 | Inaccessible, erreur HTTP 400. |
| Pinterest | Épingles et tableau des n° 11, 14, 15 | Mur de connexion ; n° 11 et 15 lisibles en partie, n° 14 supprimé. |
| Land-book, Lapa Ninja | Catégorie santé (n° 16) | Inaccessibles (Cloudflare, « Sorry, you have been blocked »). |
| Godly | Accueil | godly.website redirige vers recent.design, sans recherche. |
| ThemeForest | Thème du n° 11 | Challenge Cloudflare. |
