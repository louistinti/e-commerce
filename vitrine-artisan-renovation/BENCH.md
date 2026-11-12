# Benchmark visuel : Arotz Rénovation (artisan RGE, Pays basque)

Ce bench suit le brief bloc par bloc : chaque inspiration est rattachée à un bloc de l'arborescence ou à une exigence précise du brief, le reste est rangé à côté avec sa raison.

## Limites, à lire en premier

- **Références ouvertes et capturées le 2026-11-12**, dans un navigateur Chrome piloté (viewport 1440×900, au-dessus de la ligne de flottaison, et 390×844 pour le mobile). Les couleurs et les polices citées ont été relevées dans la page (styles calculés), pas devinées. Pour les shots Dribbble, qui sont des images, seules les couleurs visibles sont décrites. Les contrastes sont calculés selon la formule WCAG 2.1.
- **14 références sur 20 vues et capturées.** Les 2 liens Pinterest (n° 15 et 16) s'ouvrent, mais une fenêtre de connexion recouvre la page : seul le texte a été lu, aucune capture. Les 3 liens Behance (n° 4, 19 et 20) renvoient une **erreur HTTP 400** au navigateur automatisé. Lapa Ninja (n° 18) affiche **« Sorry, you have been blocked »** (Cloudflare). Aucune protection n'a été contournée. Ces références gardent leur texte, marqué **non vérifié**.
- **Remplacées par des pages ouvertes** : n° 18 par le vrai site de Quilt, n° 19 par l'accueil d'Effy. Le n° 20 (Manatee) n'a pas de remplaçant : la seule trace trouvée est une adresse de préproduction, pas un site public.
- **6 références ajoutées** (n° 21 à 26) : un shot de PAC en français, la fiche d'un artisan du 64 sur l'annuaire Effy, 2 pages officielles France Rénov', un vrai site d'entreprise de rénovation avec curseur avant/après, et un shot avant/après en même cadrage.
- **Corrections du premier passage** (les faits sont repris dans les tableaux) : le bandeau France Rénov' est obligatoire depuis le 1er octobre 2026 (n° 23, voir « Points à remonter au client ») ; Final Touch Carpentry (n° 2) a 2 boutons fantômes de même poids et son site renvoie vers une autre activité ; le shot n° 3 n'a ni icônes de services ni curseur ; le shot n° 6 est un seul écran de résultat ; le shot n° 8 n'est pas un avant/après de chantier ; le lien du vrai site du n° 9 est mort ; PRB (n° 14) montre des rendus contemporains ; One Page Love compte 2 exemples de menuisiers et 9 de construction ; le tag « heat-pumps » (n° 17) n'est pas dominé par le bleu.
- Aucun formulaire n'a été rempli ni envoyé. Le parcours Effy (n° 5) n'a pas été avancé au-delà du premier écran, car chaque réponse part vers leur serveur. Sur les captures, les photos de clients (n° 10) et les signatures et avatars de designers (Dribbble, Awwwards) ont été masqués.
- **Refonte du 2026-11-12** :
  - tri des 26 références : **11 inspirations** et **15 à côté**. Les captures sont rangées dans [`captures/inspis/`](captures/inspis/) et [`captures/a-cote/`](captures/a-cote/), sans renommage : le préfixe reste le numéro de la référence, et les numéros ne changent pas ;
  - le bench est réorganisé selon l'arborescence du brief (section 6), puis le mobile, les directions, les tokens et la liste des références à côté ;
  - **aucune nouvelle référence**. Deux blocs n'ont pas d'inspiration (déroulé en 5 étapes, zone et contact). La recherche de complément n'a rien donné d'exploitable : Dribbble affiche maintenant une vérification anti-robots (« Let's confirm you are human »), non contournée ; les sections « How it works » et « Timeline » de One Page Love ne montrent que des produits numériques ; sur Awwwards, le site de Bam Rénovation déclenche un téléchargement au lieu d'une page et n'a pas été ouvert. Détail dans « Galeries : requêtes lancées » ;
  - **tokens corrigés** pour suivre le brief (textes d'au moins 17 px, boutons de 48 px) et WCAG 2.2 AA : `type.small` passe de 15 à 17 px, `type.label` de 16 à 17 px, la poignée du curseur de 44 à 48 px, les bordures de champs de `neutral.300` (1,4:1) à `neutral.500` (3,7:1), et le bois ne sert plus aux icônes porteuses de sens (2,7:1, sous le seuil de 3:1). La direction B reçoit un garde-fou sur le drapeau basque.

**Répartition** : 26 références. Sites réels du secteur 9 (dont 2 officiels et les 2 remplaçants) · Dribbble 9 · One Page Love 2 · Awwwards 2 · Behance 2 (inaccessibles) · Pinterest 2 (mur de connexion). Les n° 18 (Lapa Ninja, bloqué) et 19 (Behance, inaccessible) sont comptés avec le site réel qui les remplace.

## Points à remonter au client

- **Bandeau France Rénov' obligatoire.** Le brief classe la mention France Rénov' dans les publicités « à confirmer par un juriste ». Or la loi Cazenave l'impose depuis le **1er octobre 2026** sur tout support de promotion de travaux de rénovation énergétique, avec un bandeau officiel, et prévoit une amende jusqu'à 75 000 € pour une société (page officielle, n° 23). Le bench prévoit le composant ; le brief n'est pas modifié. Au client de faire valider l'emplacement par un juriste et de récupérer le kit officiel dans l'espace professionnels de France Rénov'.
- **Qualibat.** Le brief cite « RGE et Qualibat avec numéros » dans les messages clés (section 5), mais seulement le RGE dans la présentation (section 1). Comme le brief interdit d'afficher une qualification non détenue, le client doit confirmer la liste exacte (organisme, numéro, domaine, validité) avant les maquettes.

---

## Couverture du brief

| Exigence du brief | Inspirations | Manque |
|---|---|---|
| 1. Hero : équipe sur un chantier, CTA « Visite gratuite », numéro cliquable, bandeau de réassurance | 1, 25 | Aucun hero vu avec un bandeau de réassurance chiffré **et numéroté** (Aira aligne des logos sans numéro). Le numéro de téléphone en gros à côté du CTA n'a été vu nulle part. |
| 2. Les travaux : 4 travaux, photo réelle, « ce que ça change » | 18, 10 | Aucune grille de services vue avec photo réelle et bénéfice concret : le seul exemple (n° 3) utilise la banque d'images. À dessiner. |
| 3. Estimation des aides : questions, fourchette indicative, barème daté, renvoi France Rénov' | 5, 1, 6, 23 | Aucun exemple de tranches de revenus Anah par taille de foyer. Le moment où Effy demande les coordonnées n'est pas vérifié. |
| 4. Réalisations avant/après : curseur, commune, travaux, DPE avant → après, gain estimé, avis | 25, 26, 7, 10, 11 | Aucune carte vue qui réunit curseur et badges DPE : Hellio met la classe dans le titre, NSH n'a pas de donnée énergétique. |
| 5. Déroulé en 5 étapes | aucune | Le seul exemple de procédé en étapes (Farbenhaus, n° 13) est hors ligne et connu par le texte de sa fiche. La recherche de complément n'a rien donné. À dessiner, en s'appuyant sur la piste C. |
| 6. Labels et assurances : numéros, liens de vérification, attestation décennale | 24 | Aucune carte label avec numéro vue en production. L'attestation décennale téléchargeable n'a été vue nulle part. |
| 7. Avis clients : note, nombre, 3 à 6 avis récents, lien vers tous les avis | 18, 5 | Aucune intégration d'avis Google vue. Le seul carrousel d'avis observé en détail est filtré (Aira, n° 1). |
| 8. Zone d'intervention et contact : carte, communes en texte, formulaire court, horaires, adresse | aucune | Ni carte avec communes en texte, ni formulaire court vus. Seul détail : les horaires collés au téléphone, chez Wambreck (n° 21, à côté). |
| Pied de page : mentions, bandeau réglementaire | 23 | Mentions légales et déclaration d'accessibilité non étudiées. |
| Mobile : barre fixe « Appeler » et « Visite gratuite » | aucune | Aucun des 3 sites vus en mobile n'a de barre fixe. NSH (n° 25) montre seulement des CTA pleine largeur. |
| Mobile : estimateur plein écran, une question par écran | 5 | Néant. |
| Marque : palette chaux, rouge basque, vert sapin, bois | aucune | Aucune référence vue avec cette palette. Le rouge est courant chez les marques de PAC (n° 17, à côté) : il reste réservé aux CTA. |
| Marque : Fraunces pour les titres | 18, 25 | Néant : Quilt (serif pour les titres) et NSH (seconde ligne en serif italique) confirment le choix. |
| Marque : photos réelles de chantiers, d'équipe, de mains | 1, 18, 25, 26 | Le shooting reste à faire, avec avant et après du même point de vue (n° 26). |
| Accessibilité : curseur avant/après au clavier | 25 | Néant. |
| Accessibilité : boutons de 48 px, textes de 17 px | 5 | Contre-exemple : l'icône téléphone de 31 px d'Aira en mobile (n° 1). |
| Preuve « Des artisans d'ici, pas des démarcheurs » | 1, 10 | Aucun engagement « on ne vous appelle jamais sans demande » vu. L'adresse de l'atelier n'est mise en avant nulle part. |
| Preuve « Certifiés et assurés, vérifiez par vous-même » | 24 | Voir le bloc 6. |
| Preuve « Des résultats mesurés » | 11, 7, 10 | Voir le bloc 4. |
| Preuve « Un seul interlocuteur » | 10 | Aucun portrait de chef de chantier référent vu : Aira nomme seulement le technicien par son prénom. |
| Preuve « Avis sans sélection trompeuse » | aucune | Aucune référence ne prouve l'absence de filtre. Aira annonce même « Showing our 4 & 5 star reviews » (n° 1). |
| Réglementaire : renvoi et bandeau France Rénov' | 23, 24 | Le kit officiel n'a pas été ouvert. |

---

## Inspirations, bloc par bloc

### 1. Hero

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 1 | Aira : Heat pump installation (site réel, UK), https://www.airahome.com/en-gb/heat-pump-installation-2 | [hero](captures/inspis/01-aira-installation.jpg) | Texte alternatif confirmé : deux installateurs bras croisés devant la camionnette jaune Aira, une pastille ronde « Which? Trusted Trader » posée sur la photo. Fond blanc, H1 en airaText 400, 54 px, `#222226`, CTA « Get a quote » `#222226` sur orange `#FFAF51` (8,7:1). Le téléphone est en texte dans l'en-tête. Version Arotz : l'équipe et la pastille RGE **avec son numéro** dans la même image. | « Photo réelle de chantier avec l'équipe » et bandeau de réassurance « RGE (n°) » |
| 25 | NSH Renovierung (Vechta), https://nsh-renovierung.de/ | [hero](captures/inspis/25-nsh-renovierung-site-reel.jpg) | H1 en Inter 800, 77 px, puis une seconde ligne en serif italique (« Neues Lebensgefühl. »), pastille « Bauunternehmen & Generalunternehmer in Vechta », un seul bouton bleu « Kostenlose Beratung » (blanc sur `#0B4EEE`, 6,3:1). | Un seul CTA « Visite gratuite », l'ancrage local dès le hero, Fraunces italique pour la seconde ligne |

À éviter : 2 boutons fantômes de même poids (n° 2, à côté) et des chiffres qui se contredisent (« 80+ » projets et « +23 » clients dans le hero de NSH, « über 150 » clients plus bas). Deux détails pris à des références à côté : des chiffres avec leur définition à côté (« <24 Hrs » d'intervention, FTCC, n° 2), pour « X chantiers au Pays basque » ; « Je calcule mes aides » en second bouton du hero (Wambreck, n° 21), pour mener vers l'estimateur.

### 2. Les travaux

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 18 | Quilt (site réel, remplace la fiche Lapa Ninja), https://www.quilt.com/ | [site réel](captures/inspis/18-quilt-site-reel.jpg) | L'unité intérieure à façade bois photographiée dans un vrai salon, une main qui pose un vase devant. La PAC se montre posée chez quelqu'un, pas en rendu produit. | « Une photo réelle » par type de travaux ; le frein « bruit d'une PAC » de Maite et Jean-Pierre se traite aussi par l'image d'une installation discrète |
| 10 | Aira : Roger & Sue's installation (site réel, UK), https://www.airahome.com/en-gb/case-studies/roger-sue-aira-heat-pump-installation | [capture](captures/inspis/10-aira-roger-sue.jpg) | Une FAQ qui répond au bruit de la PAC, sur la page du chantier. | « Ce que ça change » pour la pompe à chaleur, et le frein « bruit » du persona 1 |

À éviter : des cartes de services illustrées par la banque d'images (n° 3, à côté).

### 3. Estimation des aides

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 5 | Effy : Estimez votre prime énergie (site réel), https://www.effy.fr/parcours/1/accueil | [desktop](captures/inspis/05-effy-parcours.jpg), [mobile](captures/inspis/mobile-effy-parcours.jpg) | L'URL redirige vers `/parcours/1/travaux-aides/logement-type`. Une question, 2 grandes cartes à pictogramme et bouton radio (maison, appartement), barre de progression bleue `#4754FF` en haut, pastille « En 2 minutes ! ». Sur mobile : « 1/4 Votre logement », cartes de 312×64 px. | « Estimateur en plein écran, une question par écran » ; « tranches de revenus » en choix, jamais en champ libre |
| 1 | Aira : Heat pump installation | [questions](captures/inspis/01-aira-installation-questions.jpg) | « Answer 4 quick questions » avec 5 cartes à pictogramme (type de maison), directement dans la page. | Entrée de l'estimateur depuis le one-page, avec le nombre de questions annoncé |
| 6 | Mobile Energy Savings Calculator (Dribbble), https://dribbble.com/shots/787436-Mobile-Energy-Savings-Calculator | [capture](captures/inspis/06-dribbble-mobile-energy-calculator.jpg) | Un seul écran de résultat (400×300 px) : « 38 % Saved per year* » en très grand, la note « *based on US national… » collée dessous. Version Arotz : la fourchette d'aides en grand, « indicatif, barème du JJ/MM/AAAA, sous réserve d'éligibilité » juste dessous. | « Fourchette indicative MaPrimeRénov' + CEE », « barème daté, mention d'éligibilité » ; aucun montant présenté comme garanti (critères de réussite) |
| 23 | Publicité pour la rénovation énergétique : obligation de faire référence à France Rénov' (site officiel), https://france-renov.gouv.fr/actualites/publicite-pour-la-renovation-energetique-obligation-desormais-de-faire-reference-au | [capture](captures/inspis/23-france-renov-bandeau-publicite.jpg) | Le bandeau officiel : Marianne, logo France Rénov' et « Avant de vous engager, le service public vous informe gratuitement… ». À placer près du résultat. | « Renvoi vers France Rénov' » et obligation légale (voir « Points à remonter au client ») |

À éviter : le code « plateforme nationale » d'Effy (mascotte, jaune vif, mensualité, n° 19, à côté). **Non vérifié** : le moment où Effy demande les coordonnées. Chez Arotz, le résultat s'affiche avant toute demande de contact.

### 4. Réalisations avant/après

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 25 | NSH Renovierung (Dribbble + site réel), https://dribbble.com/shots/27865951-NSH-Renovierung-Renovation-Company-Website-Vechta et https://nsh-renovierung.de/ | [shot](captures/inspis/25-dribbble-nsh-renovierung.jpg), [références](captures/inspis/25-nsh-renovierung-references.jpg) | Références filtrables (Alle, Wohnung, Haus, Bad, Boden, Büro). Chaque carte a un curseur avec les étiquettes « Vorher » et « Nachher » toujours visibles, de vraies photos et un titre « travaux + commune ». Le curseur a `role="slider"`, un `aria-label` et se pilote au clavier (5 % par appui sur une flèche). Les sous-traitances sont signalées par un astérisque. | « Curseur avant/après », « commune, travaux » ; accessibilité : « curseur utilisable au clavier » ; ton honnête (l'astérisque) |
| 26 | Before & After renovation (Dribbble), https://dribbble.com/shots/14540322-Before-After-renovation | [capture](captures/inspis/26-dribbble-before-after-renovation.jpg) | L'avant (briques à nu, plafond abîmé) se fond en diagonale dans l'après, **avec exactement le même cadrage**. À noter dans le brief du shooting. | Un curseur qui prouve vraiment le résultat ; photos de vrais chantiers |
| 7 | Remodelmate Before/After (Dribbble), https://dribbble.com/shots/13476909-Remodelmate-Before-After | [capture](captures/inspis/07-dribbble-remodelmate-before-after.jpg) | Sous la photo, « Budget $5000 », « Time 3 weeks » et le nom de l'artisan ; une bulle de témoignage posée sur l'image. Version Arotz : classe DPE avant → après, commune, travaux, durée, extrait d'avis. | « Extrait d'avis » sur la carte ; délais attendus par Laura et Iban et par Philippe |
| 10 | Aira : Roger & Sue's installation | [capture](captures/inspis/10-aira-roger-sue.jpg) | Un fil d'Ariane qui donne la ville, « Property details » (type de maison, niveaux, chambres), « The installation at a glance » (lieu, matériel posé, aide obtenue), le technicien nommé par son prénom. Le seul chiffre de résultat est dans la citation du client. | « Commune, travaux » ; bloc « le chantier en bref » pour la page « Voir le chantier complet » |
| 11 | Hellio : Rénovation globale, 76 % d'économies à Orléans (site réel), https://www.hellio.com/actualites/communiques/renovation-energetique-orleans-globale | [capture](captures/inspis/11-hellio-orleans.jpg) | Title « Évolution de la lettre F à B au DPE : 76 % d'économies d'énergie », 156 m², chantier d'un mois, travaux listés, artisans locaux nommés. Le gain est au futur : c'est une estimation. | « Classe DPE avant → après » et « gain estimé (audit) » ; persona 3 (« cas de passage de classe ») |

À éviter : un avant/après qui n'en est pas un (n° 8, à côté) et une maison miniature dans une main (n° 9, à côté). Sur la carte Arotz, écrire « gain estimé par l'audit », jamais un gain présenté comme mesuré s'il ne l'est pas.

### 5. Déroulé en 5 étapes

Aucune inspiration. Le seul procédé en étapes trouvé est celui de Farbenhaus (8 étapes avec une infographie en poteaux de bois), connu seulement par le texte de sa fiche One Page Love : le site est hors ligne (n° 13, à côté). Le numéro de chantier en légende de PRB (n° 14, à côté) et le bloc « le chantier en bref » d'Aira (n° 10) nourrissent la piste C. À dessiner sans modèle : 5 étapes numérotées, l'étape 2 nomme Mon Accompagnateur Rénov' pour la rénovation d'ampleur, l'étape 3 dit « on monte les dossiers avec vous ».

### 6. Labels et assurances

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 24 | Annuaire des professionnels RGE (site officiel), https://france-renov.gouv.fr/annuaires-professionnels/artisan-rge-architecte | [capture](captures/inspis/24-france-renov-annuaire-rge.jpg) | Deux onglets, « Rechercher par type de prestation » et « Rechercher un professionnel », et le rappel « pour bénéficier de MaPrimeRénov', il est obligatoire de confier ses travaux à un professionnel RGE ». Le lien « Vérifier notre certification RGE » pointe ici, avec la consigne « tapez Arotz Rénovation » si aucun lien direct n'existe (non vérifié : aucune recherche lancée). | « Liens de vérification » ; « rappeler que le RGE est requis pour MaPrimeRénov' et les CEE » ; chaque label vérifiable en un clic |

À éviter : le mur de logos sans numéro d'Aira (n° 1), les logos de fournisseurs présentés comme une caution chez NSH (n° 25). La fiche Effy d'un artisan du 64 (n° 22, à côté) montre ce que le site doit dépasser : aucun numéro RGE, aucun visage.

### 7. Avis clients

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 18 | Quilt | [site réel](captures/inspis/18-quilt-site-reel.jpg) | Les avis sont titrés par type de maison (« Crisp and cozy bungalow »). Version Arotz : « Maison de 1975, Anglet ». | « Des avis de gens du coin » (persona 1) |
| 5 | Effy : parcours | [desktop](captures/inspis/05-effy-parcours.jpg) | Trustpilot 4,4 sur 9 005 avis, la note et le nombre affichés ensemble. | « Note et nombre d'avis Google » |

À éviter : « Showing our 4 & 5 star reviews » (Aira, n° 1), contraire à « sans sélection trompeuse ».

### 8. Zone d'intervention et contact

Aucune inspiration : ni carte avec les communes en texte, ni formulaire court n'ont été vus. Un seul détail, pris à une référence à côté : les horaires écrits à côté du téléphone (« Du lundi au vendredi, 8h à 19h », Wambreck, n° 21). Les messages du formulaire (succès, erreur, hors zone) sont déjà rédigés dans le brief.

### Pied de page

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 23 | France Rénov' : obligation de faire référence à France Rénov' | [capture](captures/inspis/23-france-renov-bandeau-publicite.jpg) | Le bandeau officiel, tel que fourni dans le kit, sans le redessiner. Amende jusqu'à 15 000 € (personne physique) et 75 000 € (personne morale). | Renvoi vers France Rénov' (0 808 800 700) ; obligation légale à remonter au client |

---

## Mobile (390×844)

| # | Site | Capture | Ce qu'on observe | Exigence du brief |
|---|---|---|---|---|
| 1 | Aira, installation | [capture](captures/inspis/mobile-aira-installation.jpg) | Le téléphone n'est qu'une icône de 31×31 px dans l'en-tête. L'en-tête se masque quand on fait défiler. Pas de barre fixe en bas. Le CTA orange « Get a quote » ne fait pas toute la largeur. | Contre-exemple pour « boutons de 48 px » et « téléphone trouvé en moins de 3 secondes » |
| 5 | Effy, parcours | [capture](captures/inspis/mobile-effy-parcours.jpg) | L'estimateur occupe tout l'écran : « 1/4 Votre logement », barre de progression, 2 cartes de 312×64 px. Le bouton téléphone jaune fait 54×48 px, en haut à droite, sans `aria-label` ni texte relevé. | « Estimateur en plein écran, une question par écran » |
| 25 | NSH Renovierung | [capture](captures/inspis/mobile-nsh-renovierung.jpg) | Un en-tête flottant avec le logo et un menu burger. Les 2 CTA font toute la largeur. Le numéro de téléphone n'apparaît qu'en bas de page, à environ 12 500 px du haut. Pas de barre fixe. | CTA pleine largeur ; contre-exemple pour le téléphone |

**À retenir** : aucun des 3 n'a de barre fixe avec « Appeler » et « Visite gratuite ». Le téléphone est soit trop petit (Aira), soit introuvable sans défiler (NSH). La barre fixe du brief est un vrai différenciant pour les seniors (critère : téléphone trouvé en moins de 3 secondes). Recommandations :
- une barre fixe en bas, 2 boutons égaux d'au moins 48 px : « Appeler l'atelier » (vert sapin plein) et « Visite gratuite » (rouge basque), libellés du brief ;
- l'estimateur en plein écran, l'étape nommée (« 1/4 Votre logement ») et une barre de progression, comme Effy ;
- des cartes de choix pleine largeur d'au moins 64 px de haut ;
- l'en-tête ne disparaît pas au défilement tant que la barre fixe n'est pas visible.

---

## Directions

Le brief demande un moodboard en **3 pistes** (section 10). Les 3 directions sont compatibles avec la marque, le ton et les interdits du brief ; la B reçoit un garde-fou.

**A. « Atelier » (recommandée)**
Fond blanc chaux, titres Fraunces en vert sapin, rouge basque réservé aux CTA, photos réelles chaudes (bois, laine, mains).
Les avant/après sont la colonne vertébrale de la page, et les labels numérotés apparaissent comme des tampons.
Inspirations : l'équipe et le label dans la photo (n° 1), la PAC posée dans un vrai intérieur et la serif chaleureuse (n° 18), la carte avant/après en production (n° 25), le même cadrage avant/après (n° 26).
Sensation : un artisan fier de son travail, local et vérifiable.

**B. « Etxe » (maison basque)**
Grands aplats rouge profond et vert sapin, comme les colombages, avec un motif discret inspiré des linteaux sculptés.
Inspiration : un bandeau en aplat qui porte une preuve, comme le bandeau pétrole de Quilt avec sa citation (n° 18).
**Garde-fou** : le brief interdit de reproduire tel quel le drapeau basque. Jamais de croix ni de sautoir, jamais rouge, vert et blanc assemblés comme sur l'ikurriña. Risque de folklore, contraire au ton « honnête, artisanal » : à garder pour le pied de page et les séparateurs. Le rouge en aplat rappellerait aussi les marques de PAC (n° 17, à côté).

**C. « Carnet de chantier »**
Mise en page de journal de bord : dates, étapes numérotées, photos en planche contact, notes manuscrites légères.
Excellent pour le déroulé en 5 étapes, le bloc qui n'a pas d'inspiration, et pour la transparence.
Inspirations : le bloc « le chantier en bref » (n° 10), le coût, la durée et l'artisan sous la photo (n° 7). Détail pris à une référence à côté : le numéro de chantier en légende (PRB, n° 14).
Moins direct pour la conversion : il faut la barre mobile fixe.

## Palette recommandée (direction A)

Les couleurs suivent la palette du brief (blanc chaux, rouge basque profond, vert sapin, bois). Contrastes recalculés le 2026-11-12 (WCAG 2.1), tous confirmés. Une correction d'usage : le bois ne porte plus d'icône qui a un sens.

| Rôle | Hex | Usage |
|---|---|---|
| Blanc chaux | `#F6F1E7` | Fond principal |
| Chaux claire | `#FBF8F2` | Cartes, estimateur |
| Rouge basque profond | `#9E1B22` | CTA, accents, numéros d'étapes. Blanc sur rouge : 8,0:1. Rouge sur chaux : 7,1:1 |
| Vert sapin | `#1F4A37` | Titres, barre mobile, fonds sombres, icônes porteuses de sens. Sur chaux : 8,9:1 |
| Bois | `#B98A5A` | Filets et pastilles **décoratifs** uniquement (2,7:1 sur chaux, sous le seuil de 3:1 des éléments graphiques porteurs de sens, jamais en texte) |
| Bois foncé | `#7A5534` | Texte décoratif et icônes sur fond clair si besoin (5,9:1) |
| Encre | `#1E1A17` | Texte courant (15,4:1) |

Les couleurs DPE (étiquette A à G) servent **uniquement** aux badges de classe énergie, jamais à la décoration.

## Polices (Google Fonts)

- **Fraunces** (variable, axes optique et « soft ») : titres, graisses 600 à 700, réglage « soft » modéré pour un rendu chaleureux. Exigée par le brief.
- **Source Sans 3** : texte courant, très lisible pour les seniors (la « sans lisible » du brief). Alternative : **Public Sans**.
- **Fraunces italique** : citations d'avis clients, et éventuellement la seconde ligne du H1, comme le fait NSH (n° 25).
- Relevé chez les autres : airaText, police maison (Aira), buenos-aires (Effy), Lexend (Hellio), Barlow Condensed (FTCC), Inter et une serif système en italique (NSH), « Quilt Serif » et « Quilt Sans » (Quilt). Quilt et NSH montrent qu'une serif chaleureuse fonctionne dans le secteur.

## 3 « à ne pas faire »

1. **Pas de codes de démarchage** : pas de compte à rebours, de « PAC à 1 € », de pop-up « on vous rappelle », de bandeau défilant « -10 % » (n° 21) ni de prime en très gros caractères (n° 17). Le brief interdit « travaux gratuits » et « 1 € ».
2. **Pas de banque d'images ni d'allégation verte** : pas de famille souriante sur canapé, de maison miniature dans une main (n° 9), de salon mis en scène (n° 19), de PAC en rendu 3D. Pas de « écologique » (n° 21).
3. **Pas de logos sans preuve** : ni RGE ou Qualibat sans numéro et sans lien de vérification (n° 1), ni logos de fournisseurs présentés comme une caution (n° 25), ni avis filtrés « 4 et 5 étoiles » (n° 1).

---

## Design tokens (direction A, « Atelier »)

### Couleurs

| Token | Hex | Usage |
|---|---|---|
| `color.brand.primary` | `#9E1B22` | Rouge basque : bouton primaire, numéros d'étapes |
| `color.brand.primary-hover` | `#821519` | Survol du primaire |
| `color.brand.secondary` | `#1F4A37` | Vert sapin : titres, barre mobile, bouton secondaire, icônes porteuses de sens |
| `color.brand.secondary-hover` | `#173A2B` | Survol |
| `color.brand.wood` | `#B98A5A` | Filets et pastilles décoratifs uniquement (**corrigé** : plus d'icônes porteuses de sens) |
| `color.brand.lime` | `#F6F1E7` | Blanc chaux, fond principal |
| `color.brand.lime-light` | `#FBF8F2` | Cartes, estimateur |
| `color.semantic.success` | `#2E6B3F` | Demande envoyée, éligible |
| `color.semantic.error` | `#B3261E` | Erreur de champ : toujours avec une icône, pour ne pas se confondre avec le rouge de marque |
| `color.semantic.warning` | `#A15C00` | Hors zone, barème à confirmer |
| `color.semantic.info` | `#2D5C7A` | Mentions sur les aides, infobulles |
| `color.neutral.900` | `#1E1A17` | Texte courant |
| `color.neutral.700` | `#4A433D` | Texte secondaire, légendes |
| `color.neutral.500` | `#857A70` | Bordures de champs (**corrigé**), gros textes, éléments non textuels |
| `color.neutral.300` | `#D8CFC3` | Séparateurs décoratifs uniquement (**corrigé** : plus de bordures de champs) |
| `color.neutral.100` | `#EFE8DC` | Fonds alternés |
| `color.neutral.0` | `#FFFFFF` | Champs |
| `color.dpe.a` … `color.dpe.g` | reprendre l'étiquette officielle | Badges DPE uniquement |

Contrastes calculés (WCAG 2.1), sur `#F6F1E7` sauf mention :
- blanc sur `#9E1B22` : 8,0:1 ; blanc sur `#821519` : 10,1:1 ;
- `#1E1A17` : 15,4:1 ; `#1F4A37` : 8,9:1 ; `#4A433D` : 8,6:1 ;
- `#2E6B3F` : 5,7:1 ; `#2D5C7A` : 6,4:1 ; `#A15C00` : 4,6:1 (juste au-dessus du seuil) ; `#B3261E` sur blanc : 6,5:1, sur chaux : 5,8:1 ;
- **`#857A70` : 3,7:1** (4,2:1 sur blanc), insuffisant pour un texte de moins de 24 px. Les légendes passent en `neutral.700`. Il suffit pour une bordure de champ (seuil de 3:1, WCAG 1.4.11) ;
- **`#D8CFC3` : 1,4:1**, trop faible pour délimiter un champ blanc sur fond chaux (blanc sur chaux : 1,1:1). D'où la correction des bordures ;
- `#B98A5A` : 2,7:1, jamais en texte ni en icône porteuse de sens.

### Typographie (base 17 px pour le public senior)

Le brief demande des textes d'au moins 17 px. **Corrigé** : `type.small` passe de 15 à 17 px et `type.label` de 16 à 17 px.

| Token | Police | Taille (desktop / mobile) | Graisse | Interligne |
|---|---|---|---|---|
| `type.display` | Fraunces | 72 / 40 px | 700 | 1.05 |
| `type.h1` | Fraunces | 52 / 34 px | 650 | 1.1 |
| `type.h2` | Fraunces | 38 / 28 px | 600 | 1.15 |
| `type.h3` | Fraunces | 24 / 21 px | 600 | 1.25 |
| `type.quote` (avis) | Fraunces italique | 22 / 19 px | 400 | 1.45 |
| `type.body-lg` | Source Sans 3 | 20 / 19 px | 400 | 1.6 |
| `type.body` | Source Sans 3 | 18 / 17 px | 400 | 1.65 |
| `type.small` | Source Sans 3 | 17 px | 500 | 1.5 |
| `type.label` (champs, badges) | Source Sans 3 | 17 px | 600 | 1.3 |

`type.small` et `type.body` mobile ont la même taille : la hiérarchie passe par la graisse (500) et la couleur (`neutral.700`).

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
  - **Dans la barre mobile** : fond `brand.secondary` plein, texte chaux, au moins 48 px de haut (l'icône de 31 px d'Aira est trop petite, n° 1).
  - Les horaires d'appel sont écrits à côté du numéro sur desktop (détail vu chez Wambreck, n° 21).
- **Carte réalisation** (modèle NSH, n° 25) : curseur avant/après avec `role="slider"`, `aria-label` (« Comparer avant et après, maison de 1975 à Anglet »), flèches clavier par pas de 5 %, poignée de **48 px** (**corrigé**, 44 px auparavant : le brief demande 48 px).
  - Étiquettes « Avant » et « Après » toujours visibles dans les coins.
  - Photos avant et après du même point de vue (n° 26).
  - Puis badges DPE avant → après, commune, travaux, durée, extrait d'avis en `type.quote` (n° 7), et le bloc « le chantier en bref » d'Aira (n° 10).
  - Filtres par travaux au-dessus de la grille (isolation, PAC, menuiseries, rénovation globale).
- **Carte label** : logo, nom de la qualification, numéro, domaine, date de validité, lien « Vérifier notre certification RGE » vers l'annuaire France Rénov' (n° 24). Assureur décennale, zone couverte et attestation téléchargeable à côté.
- **Bandeau France Rénov'** (obligatoire depuis le 1er octobre 2026, n° 23) : le bandeau officiel tel que fourni dans le kit, sans le redessiner, en pied de page et près du résultat de l'estimateur. Emplacement à valider par un juriste.
- **Formulaire / estimateur** :
  - une question par écran sur mobile, avec une barre de progression et l'étape nommée (« 1/4 Votre logement », comme Effy, n° 5) ;
  - libellés visibles et aide en `type.small` (17 px) ;
  - champs blancs bordés de `neutral.500` (3,7:1) ;
  - tranches de revenus en boutons radio (jamais un champ libre) ;
  - résultat annoncé par `aria-live`, en très grand, la mention collée dessous (n° 6) ;
  - mention « indicatif, barème du JJ/MM/AAAA, sous réserve d'éligibilité » collée au montant.

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

---

## À côté

Références gardées avec leur raison. Quand un détail utile en a été tiré, il est cité dans le bloc concerné.

| # | Référence | Capture | Pourquoi à côté |
|---|---|---|---|
| 2 | Final Touch Carpentry, Awwwards (nominé, 21/07/2021), https://www.awwwards.com/sites/final-touch-carpentry | [fiche](captures/a-cote/02-awwwards-final-touch-carpentry.jpg), [site actuel](captures/a-cote/02-ftcc-site-reel.jpg) | Contre-exemple pour le hero : hero bleu nuit, accroche manuscrite dorée et **2 boutons fantômes de même poids** (« Request a quote », « Call us now »), alors que le brief veut un CTA « Visite gratuite » dominant. Le lien « Visit Site » mène aujourd'hui à FTCC Group, réparation de sinistres pour assureurs (H1 Barlow Condensed 700, 78 px, or `#B8965F` sur `#17222A`), hors secteur. Détail repris au hero : des chiffres avec leur définition (« 10+ » ans, « 3000+ » sinistres, « <24 Hrs », « <5% » de reprises). |
| 3 | Home Renovation Service : Website Landing Page, Dribbble, https://dribbble.com/shots/21920571-Home-Renovation-Service-Website-Landing-Page | [capture](captures/a-cote/03-dribbble-home-renovation-service.jpg) | Enfreint « pas de banque d'images » : 3 cartes photo de services (bricoleur à la scie, plombier souriant). L'avant/après se réduit à une photo coupée en deux. Fond blanc et crème, accent orange, pastille « 12+ years ». |
| 4 | Squarespace Construction Home Renovation Website, Behance (07/2026), https://www.behance.net/gallery/252421797/SQUARESPACE-CONSTRAUCTION-HOME-RENOVATION-WEBSITE | aucune | **Non vérifié** : erreur HTTP 400 de Behance. D'après la description, un site de rénovation centré sur les chantiers terminés. |
| 8 | Before and After Website Transition (Christian Reindl), Dribbble, https://dribbble.com/shots/7180177-Before-and-After-Website-Transition | [capture](captures/a-cote/08-dribbble-before-after-transition.jpg) | Hors sujet pour le bloc 4 : pas un avant/après de chantier, mais « Zeitreise durchs Wiley », l'histoire d'un bâtiment (photo noir et blanc, motifs géométriques rouges). |
| 9 | Renovations website (One-Shot Marketing), Dribbble, https://dribbble.com/shots/20485061-Renovations-website | [capture](captures/a-cote/09-dribbble-renovations-website.jpg) | Enfreint « pas de banque d'images » : une main qui tient une maison miniature, une cuisine blanche de catalogue. Lien mort : le site annoncé (khokharrenovation.com) ne répond plus. |
| 12 | Carpenter Website Examples, One Page Love, https://onepagelove.com/tag/carpenter | [capture](captures/a-cote/12-onepagelove-carpenter.jpg) | Contexte seulement : 2 exemples. L'Atelier de la Menuisière est hors ligne depuis décembre 2011, il ne reste qu'une capture (outils roses sur fond blanc). Aucun élément ne sert un bloc du brief. |
| 13 | Construction Website Examples, One Page Love, https://onepagelove.com/tag/construction | [capture](captures/a-cote/13-onepagelove-construction.jpg) | Galerie vieillie : 9 exemples (Rockmaster, Tegra, PIQ-Mecobat, Strömma Projekt, Kvadrat, Farbenhaus, Pandolfo Costruzioni, Tvoříme domovy), dont 3 hors ligne. Le seul détail utile (Farbenhaus, procédé en 8 étapes en poteaux de bois) est **non vérifié** : site hors ligne, connu par le texte de la fiche. Cité au bloc 5. |
| 14 | PRB Architects, Awwwards SOTD (20/03/2021), https://www.awwwards.com/sites/prb-architects | [capture](captures/a-cote/14-awwwards-prb-architects.jpg) | Enfreint « uniquement de vrais chantiers » : rendus 3D de bâtiments contemporains, grande flèche noire. Note 7,43/10, palette `#000`, `#DF6C4F`, `#fff`. Le lien pointe vers une archive. Détail repris dans la piste C : le numéro de projet en légende (« PRB 21-319 »). |
| 15 | Renovation Inspiration (Architectural Digest), Pinterest, https://www.pinterest.com/archdigest/renovation-inspiration/ | aucune | **Non vérifié** : mur de connexion. Lu sans compte : 687 épingles, surtout des articles de décoration, pas des photos de chantier. |
| 16 | Artisan Renovations (artisandns), Pinterest, https://www.pinterest.com/artisandns/ | aucune | **Non vérifié** visuellement : mur de connexion. Entreprise de la région de Toronto, tableaux par pièce vieux de 7 ans. L'idée des réalisations filtrables est vue en production chez NSH (n° 25). |
| 17 | Tag « heat-pumps », Dribbble, https://dribbble.com/tags/heat-pumps | [capture](captures/a-cote/17-dribbble-tag-heat-pumps.jpg) | Contre-exemple pour « photos réelles » et « pas de travaux gratuits » : rendus produit (Alpha Innotec, Calorex), maison illustrée (Orange Energia), prime de « 2000 zł » en gros (Immergas). Le rouge y est courant : le rouge basque reste réservé aux CTA. |
| 19 | EFFY : Branding, Behance, remplacé par https://www.effy.fr/ | [accueil Effy](captures/a-cote/19-effy-accueil.jpg) | Behance **non vérifié** (erreur HTTP 400). L'accueil Effy est le code « plateforme nationale » dont Arotz doit se distinguer : salon mis en scène (contraire à « pas de banque d'images »), mascotte, jaune vif (CTA `#161637` sur `#FFF164`, 15:1), « Votre pompe à chaleur dès 49€/mois », aucun visage d'artisan (contraire au ton « artisanal, local »). |
| 20 | Manatee Energy Website, Behance (10/2025), https://www.behance.net/gallery/236008203/Manatee-Energy-Website | aucune | **Non vérifié** : erreur HTTP 400, pas de remplaçant public. La transparence promise (étapes, aide, matériel posé) est visible chez Aira (n° 1 et 10). |
| 21 | Landing Page heat pumps, Wambreck, Dribbble (projet fictif), https://dribbble.com/shots/24770469-Landing-Page-heat-pumps | [capture](captures/a-cote/21-dribbble-wambreck-pac.jpg) | Enfreint 2 interdits du brief : H1 « … nos pompes à chaleur écologiques » (allégation environnementale) et bandeau jaune défilant « -10% sur toute la gamme » (code du démarchage). Deux détails repris : les horaires à côté du téléphone (bloc 8) et « Je calcule mes aides » en second bouton (bloc 1). |
| 22 | Fiche « Renovation 64 & Co », annuaire Effy, https://www.effy.fr/artisans/pro/2807-renovation-64-co | [capture](captures/a-cote/22-effy-fiche-artisan-64.jpg) | Contexte sectoriel : ce que voit un particulier du 64 aujourd'hui. Sigle « R6 », « Partenaire Effy », 5,0 sur 1 avis, SIRET, formulaire de devis Effy en jaune, pas de photo, aucun numéro RGE dans la partie lue. C'est la situation que décrit le brief (« les plateformes captent les demandes locales ») et que le site doit dépasser. |

---

## Galeries : requêtes lancées

| Date | Galerie | Requête ou page | Résultat |
|---|---|---|---|
| 2026-11-12 | Dribbble | Shots cités (n° 3, 6, 7, 8, 9, 21, 25, 26) et tag `heat-pumps` (n° 17) | Ouverts et capturés. |
| 2026-11-12 | One Page Love | Tags `carpenter` et `construction` (n° 12, 13) | Ouverts : 2 et 9 exemples, en partie hors ligne. |
| 2026-11-12 | Awwwards | Fiches Final Touch Carpentry et PRB Architects (n° 2, 14) | Ouvertes et capturées. |
| 2026-11-12 | Behance | n° 4, 19, 20 | Erreur HTTP 400, non vérifiées. |
| 2026-11-12 | Lapa Ninja | n° 18 | Bloqué par Cloudflare, remplacé par le site réel. |
| 2026-11-12 | Pinterest | n° 15, 16 | Mur de connexion, texte seul. |
| 2026-11-12 | Land-book, Godly | non retestés | Sur ce projet, Land-book bloque par Cloudflare et Godly redirige vers recent.design. |
| 2026-11-12 (refonte) | Dribbble | Recherche « renovation process steps » | Landing pages génériques de rénovation et de toiture (Norra Haus, RENOVUM, Mercer Co…) ; aucune section de déroulé visible sur les vignettes. Aucune retenue. |
| 2026-11-12 (refonte) | Dribbble | Recherche « how it works steps timeline » | Vérification anti-robots (« Let's confirm you are human »). Arrêt, rien contourné. |
| 2026-11-12 (refonte) | One Page Love | Sections `how-it-works` (198 exemples) et `timeline` (109) | Premiers exemples : produits numériques et portfolios (Clips, Flashform, Statements, Petrillo…). Rien pour un artisan. |
| 2026-11-12 (refonte) | Awwwards | Recherche « renovation » | 4 fiches : NYC Renovation (2025), Bam Rénovation (2024, Studio Waaz, maçonnerie), RS.D Agencements & Rénovation (2020), Total Renovation Contractors (2017). Le site de Bam Rénovation déclenche un téléchargement au lieu d'une page : pas ouvert. Les 3 autres n'ont pas été ouverts. |
