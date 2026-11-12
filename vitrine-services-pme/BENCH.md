# Benchmark : site vitrine Brillance Pro (nettoyage B2B, Bordeaux, entreprise fictive)

## Limites, à lire en premier

- **Sites ouverts et capturés le 2026-11-12**, dans un navigateur Chrome piloté (viewport 1440×900, au-dessus de la ligne de flottaison, et 390×844 pour le mobile). Les captures sont dans [`captures/`](captures/). Les couleurs et les polices citées ont été relevées dans la page (styles calculés), pas devinées. Les contrastes sont recalculés selon la formule WCAG 2.1.
- **14 références sur 16 vues et capturées.** Les 2 pages Stratus (n° 9 et 10) sont **inaccessibles (protection anti-robots)** : un challenge Cloudflare « Verify you are human » s'affiche, et il n'a pas été contourné. Leur texte reste celui de la session précédente, **non vérifié**.
- **La première version se trompait sur plusieurs points**, corrigés ci-dessous. Lebontri est une plateforme d'annonces (intervenants vérifiés, acompte de 10 %), pas une entreprise de nettoyage. Aucun « {city} » n'est visible sur ses pages. Son « simulateur » n'a ni champ ni prix : l'estimation est floutée et demande un compte. L'« estimation instantanée » de Coverall exige les coordonnées avant le prix. Les titles « devis sous 24h » et la mention « free, no-obligation » d'Office Pride n'existent plus.
- **9 références de galerie ajoutées** (7 Dribbble, 1 One Page Love, 1 composant réel). Pinterest exige un compte, Land-book et Lapa Ninja bloquent par Cloudflare, Behance renvoie une erreur 400, Awwwards ne renvoie rien de pertinent et Godly redirige vers un autre site. Le détail est en fin de section « Galeries d'inspiration ».
- Aucun formulaire n'a été rempli ni envoyé. Les captures ne montrent pas de données personnelles (les signatures d'auteurs et les avatars ont été masqués avant la capture).

---

## Hero et SEO local

| # | Référence | URL | Source | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 1 | Lebontri : Nettoyage de bureau à Bordeaux | https://lebontri.fr/nettoyage-bureau/bordeaux | Plateforme FR (annonces et devis d'intervenants) | [capture](captures/01-lebontri-bordeaux.jpg) | Hero vert foncé sur photo floutée, H1 blanc « Nettoyage de bureaux à Bordeaux – Service sur mesure pour entreprises » en Bricolage Grotesque 700, 48 px, texte en Hanken Grotesk. Au-dessus du H1, une pastille « Bordeaux et alentours · intervenants vérifiés ». CTA vert clair `#D1ED92`, texte `#12372A` (10,1:1), puis « Gratuit · 3 minutes · une photo suffit » et 5 coches. Pas de délai dans le H1. Aucun « {city} » dans le texte de la page. **À reprendre** : la pastille de zone au-dessus du H1 et la micro-ligne sous le CTA. **À éviter** : le gabarit dupliqué (Bordeaux, Tours et Valenciennes ont le même hero, seuls la ville et la fin du H1 changent, voir n° 2 et 6). |
| 2 | Lebontri : Nettoyage de bureau à Tours | https://lebontri.fr/nettoyage-bureau/tours | Plateforme FR | [capture](captures/02-lebontri-tours.jpg) | Le title a changé : « Nettoyage de bureaux Tours (37) : devis de pros \| LeBonTri ». La promesse « devis sous 24h » a disparu, mais le numéro de département entre parenthèses reste un bon signal local. Seuls la ville, la fin du H1 et le département de la coche changent. **À reprendre** : « Nettoyage de bureaux Bordeaux (33) : devis en 24 h \| Brillance Pro » pour le title. |
| 3 | Onet : agence de Lyon | https://www.onet.fr/en/agencies/onet-proprete-et-services-lyon/ | Site réel (FR, version anglaise) | [capture](captures/03-onet-lyon.jpg) | L'URL mène à la version anglaise. Une vraie photo d'agent Onet en tenue sur tout le hero, le H1 centré en Montserrat 700, une pastille « Open » et 2 boutons-pilules de même taille : « Ask for a quote » blanc sur `#F34028` (3,8:1) et « Give us a call » blanc sur `#41C5E7` (2,0:1). Plus bas : horaires (lundi au vendredi, 8 h-12 h et 14 h-17 h), adresse, téléphone et une carte OpenStreetMap. Les données `LocalBusiness` sont présentes. **À reprendre** : le bloc horaires, adresse et carte OSM légère. **À éviter** : 2 CTA au même poids, et du blanc sur des couleurs vives sous 4,5:1. |
| 4 | Onet : agence du Mans | https://www.onet.fr/en/agencies/onet-proprete-et-services-le-mans/ | Site réel (FR, version anglaise) | [capture](captures/04-onet-le-mans.jpg) | Même gabarit, avec la photo du bâtiment de l'agence (à Arnage, comme le dit le title). Le label Qualipropre n'est pas près du CTA : il est dans une section « Certifications » plus bas, avec son logo et une phrase. **À reprendre** : un bloc « Certifications » avec logo et phrase d'explication, seulement si le label est obtenu. |
| 5 | Office Pride : Colorado Springs Downtown | https://officepride.com/colorado-springs-downtown/ | Site réel (US) | [capture](captures/05-office-pride-colorado-springs.jpg) | Photo d'équipe en polos verts sous un dégradé bleu, H1 « Professional Cleaners » en CeraPro, la ville sous le H1 et un repère de lieu au-dessus. Deux boutons : « Request a Quote » blanc sur `#00964D` (3,8:1) et le téléphone en bouton blanc. À droite, une carte « Step 1 of 3 » avec barre de progression, 4 champs (nom, e-mail, société, téléphone) et « Next » bleu nuit `#12345A`, puis 3 réassurances (« Highly reviewed · Locally owned · Professional crews »). La mention « free, no-obligation » n'apparaît plus, seulement « Free Quote ». **À reprendre** : « Étape 1 sur 3 » avec barre de progression, la ligne de 3 réassurances sous le bouton. **À éviter** : les coordonnées dès l'étape 1. |

## Devis et estimateur

| # | Référence | URL | Source | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 6 | Lebontri : simulateur (Valenciennes) | https://lebontri.fr/nettoyage-bureau/valenciennes | Plateforme FR | [hero](captures/06-lebontri-valenciennes.jpg), [estimation](captures/06-lebontri-valenciennes-estimation.jpg) | **Correction** : pas de simulateur dans la page, ni champ ni prix (les « 180 € et 720 € » de la première version n'existent pas). La section « Quel budget… » montre 4 cartes à icône (la surface, la fréquence, les prestations, les horaires) et une carte sombre « Votre estimation personnalisée » où le prix est flouté (« ••• € »), avec « Gratuit et sans engagement · compte requis ». Plus haut, une photo de techniciens en combinaison dans une salle de bain moisie illustre une page de bureaux. **À reprendre** : les 4 facteurs de prix en cartes à icône. **À éviter** : le prix caché derrière un compte, et une photo hors sujet. |
| 7 | Coverall : estimateur janitorial | https://www.coverall.com/commercial-cleaning-services/janitorial/ | Site réel (US) | [hero](captures/07-coverall-janitorial.jpg), [estimateur](captures/07-coverall-janitorial-estimateur.jpg) | H1 « COMMERCIAL JANITORIAL SERVICES » en Roboto Condensed 900, 80 px, capitales blanches sur une photo d'équipe posée. CTA d'en-tête blanc sur `#00AB48` (3,0:1). L'encart « Get an instant cleaning quote » est un formulaire de 10 champs : prénom, nom, e-mail, téléphone, code postal, société, type de lieu, type de nettoyage, surface, passages par semaine. La fourchette mensuelle n'apparaît qu'après l'envoi. Sous l'encart, le périmètre en 5 tâches (sols, déchets, aspirateur, poussière, surfaces). **À reprendre** : la liste courte du périmètre. **À éviter** : une estimation « instantanée » qui exige les coordonnées avant le prix. |
| 8 | Coverall : Get a Quote | https://www.coverall.com/get-a-quote/ | Site réel (US) | [capture](captures/08-coverall-get-a-quote.jpg) | Photo de 4 agents souriants face à l'objectif, gants verts en avant : un cliché de banque d'images. Le formulaire a 6 champs obligatoires (prénom, nom, e-mail, code postal, téléphone, type de lieu). Pas de lien « besoin ponctuel » visible. La section « How we determine your quote » explique la visite : état et agencement des locaux, surface nettoyable, zones de passage, fréquence, complexité, budget. **À reprendre** : un paragraphe « Comment on calcule votre devis » qui justifie la visite. |
| 9 | Stratus : Get a Quote | https://www.stratusclean.com/get-quote/ | Site réel (US) | inaccessible | **Inaccessible (protection anti-robots, Cloudflare)**, non vérifié. D'après la session précédente : un formulaire court (nom, société, téléphone, e-mail, code postal, service) et l'argument « devis bâti sur vos locaux, pas sur des hypothèses ». |
| 10 | Stratus : devis Miami | https://www.stratusclean.com/locations/miami/get-quote/ | Site réel (US) | inaccessible | **Inaccessible (protection anti-robots, Cloudflare)**, non vérifié. Une page devis par implantation : pour Brillance Pro, une seule page suffit, le code postal peut pré-remplir la commune. |
| 11 | Companeo : devis express nettoyage | https://www.companeo.com/nettoyage-de-locaux/devis-express | Plateforme FR | [capture](captures/11-companeo-devis-express.jpg) | H1 « Entreprise de nettoyage, comparez les prix et faites jusqu'à 55 % d'économies ! » en bleu `#00A3E4` (2,8:1 sur blanc). Promesses : « les devis de 4 sociétés de nettoyage », « 60 secondes chrono », « 157 entreprises ». Aucun délai de 48 h n'est affiché. L'étape 1 demande le type de local en 7 cartes à icône, puis « Continuer » blanc sur orange `#F89827` (2,2:1). Photo de banque d'images et carte de France à figurines 3D. **À reprendre** : le type de local en cartes à icône à l'étape 1. **À retenir** : Companeo promet la rapidité de la demande, pas de la réponse. Afficher « devis en 24 h » et un interlocuteur unique reste différenciant. |

## Preuves et avis

| # | Référence | URL | Source | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 12 | Coverall Fresno : plus de 100 avis Google 5 étoiles | https://www.coverall.com/in-the-news/coverall-of-fresno-reinforces-role-as-the-best-commercial-cleaning-provider-with-5-star-rating-and-over-100-google-reviews/ | Site réel (US) | [capture](captures/12-coverall-fresno-avis.jpg) | Un communiqué du 19 août 2026, en texte seul : pas d'étoiles, pas de widget. Le seul verbatim est anonyme et non daté (« One recent reviewer shared… »). **À reprendre** : la note et le nombre d'avis dans un titre. **À éviter** : un verbatim sans prénom ni date. |
| 13 | Coverall Gainesville : 40e avis 5 étoiles | https://www.coverall.com/in-the-news/coverall-of-gainesville-celebrates-40th-5-star-review-and-perfect-5-star-google-rating-reinforcing-role-as-best-commercial-cleaning-service-in-gainesville-fl/ | Site réel (US) | [capture](captures/13-coverall-gainesville-avis.jpg) | Même format, daté du 2 septembre 2026. La citation vient de la direction, pas d'un client. **À retenir** : 40 avis suffisent à faire une annonce locale, ce qui confirme l'objectif de 30 avis du brief. |

## Pédagogie du prix et prestations

| # | Référence | URL | Source | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 14 | Coverall : Pricing Commercial Cleaning Services | https://www.coverall.com/commercial-cleaning-services/pricing-commercial-cleaning-services-for-your-business/ | Site réel (US) | [capture](captures/14-coverall-pricing.jpg) | **Correction** : c'est un article de blog en texte seul, sans icônes ni estimateur. Il cite la surface (au m² ou à l'heure), la fréquence et le nombre de tâches. Les 4 facteurs en icônes ont en fait été vus chez Lebontri (n° 6). **À reprendre** : le ton « questions à poser à votre prestataire », en 3 ou 4 lignes sous l'estimateur. |
| 15 | Coverall : FAQ nettoyage commercial | https://www.coverall.com/faqs/commercial-cleaning/ | Site réel (US) | [capture](captures/15-coverall-faq.jpg) | 14 questions en accordéon, en capitales, sous une photo de foule de banque d'images. Pas de données structurées FAQPage dans la page. La réponse sur le prix est repliée et n'a pas été lue. **À reprendre** : une FAQ de 5 questions, avec FAQPage (Coverall ne le fait pas). **À éviter** : la photo de foule sans rapport avec le métier. |
| 16 | Lebontri : fin de chantier à Bordeaux | https://lebontri.fr/nettoyage-fin-chantier/bordeaux | Plateforme FR | [capture](captures/16-lebontri-fin-chantier-bordeaux.jpg) | Même gabarit que les pages bureaux, mais un sous-titre propre au métier : « Poussières de plâtre, voiles de ciment, traces de peinture ». Une coche précise « Revêtements fragiles et date de livraison ». **À reprendre** : la carte « Fin de chantier » renvoie vers une page dédiée « Nettoyage fin de chantier en Gironde », avec les salissures et la date de livraison dans les premières lignes. |

---

## Galeries d'inspiration

Requêtes lancées le 2026-11-12 : « cleaning service website », « commercial cleaning landing page », « office cleaning website », « multi step quote form », « before after slider ». Les URL sont celles des pages de shot ou de site réellement ouvertes. Les numéros suivent ceux du bench.

| # | Référence | URL | Source | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 17 | PartnerPlus, Commercial Cleaning Service Website (Wavespace) | https://dribbble.com/shots/27382820-PartnerPlus-Commercial-Cleaning-Service-Website | Dribbble | [capture](captures/17-dribbble-partnerplus.jpg) | Le plus proche de la direction A pour la couleur : fond blanc, un bleu franc pour le seul CTA « Check Our Prices », le téléphone juste dessous en texte. Une pastille « The standard for commercial » au-dessus du H1. Les illustrations de bâtiments remplacent les photos. **À reprendre** : un seul CTA bleu, le téléphone dessous, la pastille. **À éviter** : l'illustration à la place de vraies photos d'équipe. |
| 18 | Polar, Commercial Cleaning Website Design (Systra Studios) | https://dribbble.com/shots/27768209-Polar-Commercial-Cleaning-Website-Design | Dribbble | [capture](captures/18-dribbble-polar.jpg) | Hero sombre (contraire à la direction A), mais la preuve est bien placée : « 5,0 basierend auf 36 Google-Bewertungen » et des cartes d'avis sous le CTA, puis un carrousel de prestations avec de vraies photos de lieux (cage d'escalier, bureaux). Promesse « Wir sind fertig, bevor Ihr Tag beginnt ». **À reprendre** : la note Google et le nombre d'avis sous le CTA, et la promesse horaire (« Tout est propre avant votre arrivée »). |
| 19 | Cleaning Lead Generation Landing Page (WPLanding) | https://dribbble.com/shots/27223369-Cleaning-Lead-Generation-Landing-Page | Dribbble | [capture](captures/19-dribbble-cleanpolish.jpg) | La ville en couleur dans le H1 (« Cleaning for busy people in New York »), 2 boutons, puis « 4.9/5 » avec étoiles et pastilles d'avatars, et une bande de logos clients. **À reprendre** : la ligne note et nombre de clients sous les boutons. **À éviter** : les logos factices (« Logoipsum ») tant qu'il n'y a pas de vrais clients à citer. |
| 20 | Local Cleaning Service Website, Flatiron Maids (Jabel Ahmed) | https://dribbble.com/shots/27650887-Local-Cleaning-Service-Website-Landing-Page-UI | Dribbble | [capture](captures/20-dribbble-flatiron-maids.jpg) | L'estimateur est dans le hero : 4 listes (ville, type de logement, pièces, formule) et un bouton orange. Un argument « Want the same team? » et la note « 4.8/5, 1000+ reviews ». C'est le meilleur exemple pour la direction C. **À reprendre** : l'argument « la même équipe chaque semaine », et des champs dans le hero si on choisit la direction C. |
| 21 | Multistep request quote form (Amine) | https://dribbble.com/shots/24125199-Multistep-request-quote-form | Dribbble | [capture](captures/21-dribbble-multistep-quote-form.jpg) | Une barre d'étapes nommées (type, préférences, recommandation, coordonnées), des cartes à grande icône pour le type, et la recommandation affichée **avant** les coordonnées. **À reprendre** : exactement cet ordre pour le devis en 3 étapes, avec des étapes nommées plutôt que des points. |
| 22 | Before/After slider (Diana Fabiańczuk) | https://dribbble.com/shots/27731233-Before-After-slider | Dribbble | [capture](captures/22-dribbble-before-after-slider.jpg) | Une ligne de séparation fine, une poignée ronde avec 2 flèches, et 2 étiquettes en pilule « Before us » et « After us » dans les coins hauts. **À reprendre** : la poignée à flèches (elle dit qu'on peut glisser) et les étiquettes « Avant » et « Après » toujours visibles. |
| 23 | KD Enterprises, Commercial Cleaning & Facility Landing page (Carlos Pessane) | https://dribbble.com/shots/27818578-KD-Enterprises-Commercial-Cleaning-Facility-Landing-page | Dribbble | [capture](captures/23-dribbble-kd-enterprises.jpg) | **Contre-exemple** : tous les clichés du secteur réunis. Femme en tablier avec éponge et gants rouges, étincelles dorées, « We provide Efficient Cleaning Services ». Rien ne dit qui, où ni à quel prix. |
| 24 | Cleaning Service Website Examples | https://onepagelove.com/tag/cleaning-service | One Page Love | [capture](captures/24-onepagelove-cleaning-service.jpg) | Seulement 4 exemples, tous de 2012-2013 et aujourd'hui hors ligne. Ils montrent un autre cliché : la mascotte (super-héros « Schluss mit Schmutzig », chapeau haut-de-forme). **À retenir** : la galerie confirme que le secteur a peu de références soignées, donc une vitrine nette se démarque vite. |
| 25 | img-comparison-slider (composant open source) | https://img-comparison-slider.sneas.io/ | Site réel (composant web) | [capture](captures/25-img-comparison-slider.jpg) | Un vrai curseur avant/après, testé dans la page : après un clic, les flèches du clavier déplacent la séparation (de 4 % à 95 % en maintenant la flèche droite). C'est un composant web, compatible avec un site statique. L'élément n'expose pas de rôle ARIA. **À reprendre** : ce composant ou équivalent, avec un `aria-label` (« Comparer avant et après, bureaux Chartrons, mars 2027 ») et une légende visible. |

**Plateformes sans référence retenue**
- Behance : inaccessible, erreur HTTP 400 renvoyée au navigateur automatisé.
- Pinterest : la recherche « cleaning business website design blue » s'affiche derrière une fenêtre de connexion obligatoire. Inaccessible sans compte, aucun lien de pin lisible.
- Land-book : inaccessible (protection anti-robots, challenge Cloudflare persistant).
- Lapa Ninja : inaccessible (protection anti-robots, page « Sorry, you have been blocked »).
- Awwwards : la recherche « cleaning » renvoie des sites d'agences et de portfolios sans rapport. Aucun retenu.
- Godly : godly.website redirige vers recent.design, sans recherche et sans site de services locaux.

**Clichés croisés** : agents souriants face à l'objectif avec gants colorés (n° 8, 23), femme à l'éponge et étincelles (n° 23), mascotte (n° 24), foule de banque d'images (n° 15), carte de France à figurines 3D (n° 11), photo spectaculaire hors sujet (n° 6), logos factices (n° 19).

## Avant/après et mobile

**Avant/après.** Aucun site réel de nettoyage avec un curseur n'a été trouvé (recherches web en anglais et en français, et une page Jan-Pro qui renvoie une erreur 403). Les deux références vues sont le shot n° 22 pour le dessin et le composant n° 25 pour le comportement au clavier. Les recommandations restent :
- un curseur utilisable au clavier, avec une légende (lieu, date, type de chantier) et 3 ou 4 cas maximum ;
- une poignée ronde à flèches et les étiquettes « Avant » et « Après » toujours visibles (n° 22) ;
- un `aria-label` explicite, car le composant n'en fournit pas (n° 25).

**Mobile (390×844).**

| Site | Capture | Ce qu'on observe |
|---|---|---|
| Lebontri, Bordeaux | [capture](captures/mobile-lebontri-bordeaux.jpg) | Une barre fixe en bas, un seul bouton pleine largeur « Estimer mon nettoyage · Gratuit ». Pas de bouton d'appel. Au premier écran, le même CTA apparaît 2 fois (hero et barre). |
| Office Pride | [capture](captures/mobile-office-pride.jpg) | Dans le hero, 2 boutons de même largeur : « Request a Quote » vert et le téléphone en blanc. Le formulaire « Step 1 of 3 » suit. La barre fixe « Ready to get started? Request a Quote » reste visible même quand le formulaire est à l'écran, et le bouton d'accessibilité la chevauche. |
| Coverall, janitorial | [capture](captures/mobile-coverall-janitorial.jpg) | Pas de barre fixe. Le numéro est en lien `tel:` dans le bandeau du haut. Le H1 en capitales prend 3 lignes et la photo occupe presque tout l'écran. |

**À retenir** : aucun des 3 ne met « Appeler » et « Devis » côte à côte dans la barre fixe. La barre en 2 boutons égaux du brief reste un vrai plus. Office Pride montre pourquoi il faut la masquer quand le formulaire est visible (règle déjà dans les tokens). Recommandations inchangées :
- une barre mobile fixe en bas, en 2 boutons égaux (« Appeler » en blanc bordé de bleu, « Devis » en bleu plein) ;
- un formulaire en 3 écrans, avec une barre de progression, des boutons-cartes pour le type de local et des pastilles pour la fréquence ;
- l'estimation s'affiche avant les coordonnées.

---

## Synthèse du moodboard

Les 3 directions sont maintenues. Deux ajustements, justifiés par ce qui a été vu : la direction C ne s'appuie plus sur Coverall (son estimateur n'est pas dans le hero et demande les coordonnées avant le prix), et chaque direction cite maintenant ses références capturées.

**Direction A : « Net et lumineux »** (recommandée)
- Beaucoup de blanc, le bleu franc pour le seul CTA, le vert en pastilles de validation (« ✓ sans engagement »). Références : PartnerPlus (n° 17) pour le blanc et le bleu.
- De vraies photos de l'équipe en tenue, en lumière naturelle, et des icônes au trait. Références : Onet (n° 3), un agent au travail, de dos, logo visible, et Office Pride (n° 5), une équipe en tenue. C'est plus crédible que les poses face à l'objectif de Coverall (n° 8).
- La note Google sous le CTA (n° 18, 19) et le formulaire « Étape 1 sur 3 » visible dès le hero (n° 5), mais avec le type de local en premier.
- C'est la plus sûre pour inspirer confiance et la plus facile à décliner pour d'autres métiers.

**Direction B : « Artisan de quartier »**
- Un fond très légèrement teinté, des photos de lieux bordelais reconnaissables, la carte des communes mise en avant (le bloc horaires et carte OSM d'Onet, n° 3, en version chaleureuse).
- Ton chaleureux, prénoms, citation de la gérante.
- Le risque est que ce soit moins décliné tel quel pour un autre métier ou une autre ville.

**Direction C : « Le comparateur »**
- L'estimateur occupe le hero, comme le shot Flatiron Maids (n° 20), avec une fourchette tout de suite et sans coordonnées.
- Une interface très fonctionnelle, avec des cartes de prestations sous forme de « produits ».
- La plus efficace pour la conversion, mais la moins différenciante émotionnellement.

**Palette recommandée** (contrastes WCAG calculés)

Inchangée. Les observations la confortent : les CTA verts des concurrents portent du texte blanc à 3,0:1 (Coverall, `#00AB48`) et 3,8:1 (Office Pride, `#00964D`), le bouton orange de Companeo tombe à 2,2:1. Garder le vert pour les pastilles et le bleu `#1D4ED8` (6,7:1) pour les CTA évite ce défaut.

| Rôle | Hex | Usage |
|---|---|---|
| Blanc | `#FFFFFF` | Fond principal |
| Bleu franc | `#1D4ED8` | CTA, liens, titres d'accent. Contraste de 6,7:1 sur blanc, blanc sur bleu : 6,7:1 |
| Bleu très clair | `#EFF6FF` | Fonds de section, cartes. Le bleu y garde un contraste de 6,2:1 |
| Vert frais | `#22C55E` | Pastilles, icônes, bordures. **Jamais du texte sur blanc** (2,3:1). Texte foncé sur vert : 7,8:1 |
| Vert texte | `#15803D` | Mentions « ✓ » en texte sur blanc (5,0:1) |
| Encre | `#0F172A` | Corps de texte (17,9:1) |
| Gris | `#475569` | Texte secondaire (7,6:1) |

**Polices Google Fonts**
- **Figtree** (700 et 800) pour les titres, **Figtree** (400 et 500) pour le texte. Une seule famille.
- Alternative : **Nunito Sans**.
- Relevé chez les concurrents : Bricolage Grotesque et Hanken Grotesk (Lebontri), Montserrat (Onet), Roboto Condensed en capitales (Coverall), CeraPro (Office Pride), Roboto (Companeo). Rien ne justifie de changer : Figtree reste plus lisible que les capitales condensées de Coverall et se distingue de Montserrat.

**3 choses à ne pas faire**
1. Pas de banque d'images (main gantée, éponge, sourire face à l'objectif, foule) : de vraies photos de l'équipe et des chantiers, sinon rien. Vu chez Coverall (n° 8, 15) et Companeo (n° 11).
2. Pas de pages-villes générées en masse ni de texte dupliqué. Le « {city} » visible n'a pas été constaté, mais les pages Lebontri de Bordeaux, Tours et Valenciennes ont le même hero, à la ville et à la fin du H1 près (n° 1, 2, 6).
3. Pas de vert en texte sur fond blanc, pas de prix caché derrière un compte ou des coordonnées (n° 6, 7), et pas d'avis sans source ni date (n° 12).

---

## Design tokens (format design system)

Contrastes calculés selon la formule WCAG 2.1. Le fond de référence est `bg.default` (`#FFFFFF`).

### Couleurs

| Token | Hex | Usage | Contraste |
|---|---|---|---|
| `brand.blue` | `#1D4ED8` | CTA, liens, accents de titre | 6,7:1. Blanc sur bleu : 6,7:1 |
| `brand.blue-hover` | `#1E40AF` | Survol du CTA | 8,7:1 |
| `brand.blue-50` | `#EFF6FF` | Fonds de section, cartes | Le bleu y garde 6,2:1 |
| `brand.green` | `#22C55E` | Pastilles, icônes, bordures | **2,3:1 sur blanc, donc jamais en texte**. Texte encre sur vert : 7,8:1 |
| `brand.green-50` | `#F0FDF4` | Fond des encarts « sans engagement » | sans objet |
| `semantic.success` | `#15803D` | Messages de succès, coches en texte | 5,0:1 |
| `semantic.error` | `#B91C1C` | Erreurs de formulaire | 6,5:1 |
| `semantic.warning` | `#B45309` | Avertissements (« estimation indicative ») | 5,0:1 |
| `neutral.900` | `#0F172A` | Corps de texte | 17,9:1 |
| `neutral.600` | `#475569` | Texte secondaire | 7,6:1 |
| `neutral.400` | `#7A8699` | Bordures de champs (≥ 3:1) | 3,7:1 |
| `neutral.200` | `#CBD5E1` | Séparateurs décoratifs | décoratif |
| `bg.default` | `#FFFFFF` | Fond | sans objet |

Déclinaison métier : seul `brand.green` change (par exemple un orange pour la maintenance, un vert plus profond pour les espaces verts). Il faut alors revérifier le contraste.

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

**Barre mobile fixe** : 2 boutons de largeur égale (secondaire « Appeler », primaire « Devis »), hauteur 56 px, `safe-area-inset-bottom` respecté. Elle est masquée quand le formulaire de devis est visible.

**Carte de prestation** : fond `bg.default`, bordure `neutral.200`, `radius.lg`, icône au trait sur pastille `brand.green-50`. Elle contient un titre `h3`, une ligne « pour qui », un « à partir de » optionnel et un lien d'action. Au survol : `shadow.md`.

**Formulaire de devis en 3 étapes** :
- barre de progression « Étape 2 sur 3 » ;
- étape 1 : type de local en cartes radio ;
- étape 2 : surface en tranches ou champ numérique, fréquence en pastilles, puis l'estimation dans un encart `brand.blue-50` avec la mention `semantic.warning` « indicative, confirmée après visite » ;
- étape 3 : 4 champs avec labels visibles ;
- erreur sous le champ, en texte et avec icône, et `aria-describedby`.

**Bloc avis** : la note en grand (`price`), des étoiles avec un texte alternatif (« 4,8 sur 5, 37 avis Google »), 3 verbatims avec prénom, initiale et date.

| À faire | À ne pas faire |
|---|---|
| Un seul CTA primaire par section | « Devis », « Contact » et « Rappel » côte à côte au même poids |
| Le vert en pastilles, icônes et bordures | Du texte vert clair sur blanc (2,3:1) |
| L'estimation affichée avant de demander les coordonnées | Les coordonnées exigées dès l'étape 1 |
| Le téléphone en lien `tel:`, visible dans l'en-tête | Le numéro en image ou en pied de page seulement |
| De vraies photos compressées (WebP/AVIF) avec dimensions fixées | Des photos de banque d'images lourdes qui décalent la mise en page |
| Les avis datés, sourcés, avec un lien vers la fiche Google | Des avis sans date ni source, ou un widget qui charge 500 Ko de JavaScript |
| Un focus visible et un curseur avant/après utilisable au clavier | Un curseur uniquement au glisser |
