# Benchmark : site vitrine Rempart (SOC managé PME, entreprise fictive)

## Limites, à lire en premier

Mise à jour du 2026-11-12, faite avec un vrai navigateur (Chrome piloté par Playwright).

- **Ce qui a été vu** : les 18 références d'origine ont été ouvertes. 18 captures, dont une page de remplacement pour le PDF MonAideCyber, qui ne s'affiche plus. Une capture par référence, en 1440 × 900 px, au-dessus de la ligne de flottaison, dans [`captures/`](captures/). Les couleurs et les polices citées ont été relevées dans la page (`getComputedStyle`), pas devinées. Les chiffres cités sont ceux affichés sur la page le 2026-11-12.
- **Corrections** : plusieurs affirmations de la version précédente, écrites « d'après la description », étaient fausses. Elles sont corrigées dans les tableaux (n° 1, 4, 5, 6, 10, 17 surtout).
- **URL mortes ou redirigées** : le PDF MonAideCyber (n° 4) ne s'affiche plus, il est remplacé par la page du diagnostic en accès libre. La page Dattak n° 7 redirige vers `/fr/insurance`.
- **Galeries** : 8 références ajoutées (Dribbble, Awwwards, One Page Love). Behance, Land-book, Lapa Ninja, Pinterest et Godly n'ont rien donné : voir « Galeries : requêtes lancées ».
- **Pas vérifié** : le nombre de recommandations du diagnostic MonAideCyber (il faut accepter des CGU, ce qui n'a pas été fait) et le résultat de l'estimateur Coverall (il faut envoyer nom, e-mail et téléphone).
- **Bannières cookies** : refusées partout où un refus existait (« Tout refuser », « Refuser », « Continuer sans accepter »). Sur Advens mobile, le widget a été fermé en laissant tous les choix décochés.

---

## Hero et positionnement

| # | Référence | URL | Source | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 1 | Huntress : Why Huntress | https://www.huntress.com/why-huntress | Site réel (US) | [capture](captures/01-huntress.jpg) | Fond quasi noir `#050707`, titre en capitales Archivo Black 56 px, texte en Funnel Sans, photo de salle serveurs aux néons cyan et magenta. Bouton principal cyan `#00DBE5` à texte noir, angles droits. **Il n'y a pas de chiffres sous le titre** : « 285,000 businesses » n'apparaît que plus bas, dans un intertitre, et « déployé en moins de 20 minutes » dans un paragraphe. Le délai de 8 min annoncé dans la version précédente n'est pas sur la page. **À reprendre** : le bouton cyan à texte sombre (11,8:1). **À éviter** : la photo de datacenter néon et les capitales massives, à l'opposé du ton rassurant. |
| 2 | Stoïk : Cybersécurité | https://www.stoik.com/cybersecurite | Site réel (FR) | [capture](captures/02-stoik-cybersecurite.jpg) | Hero dans une grande carte bleu saturé `#1362DD` à coins arrondis, titre fin (Lazzer, graisse 400, 56 px) en `#F2F2F2` avec « 360° » en rose, maquette de tableau de bord à droite. Les preuves « 14 000+ PME et ETI européennes protégées et assurées » et « 24h/7j de surveillance par un SOC européen internalisé » sont plus bas, pas accolées à la promesse. Le premier bouton est « Devenir partenaire », avant « Se protéger ». **À reprendre** : la mention géographique du SOC (Stoïk dit « européen », Rempart pourra dire « en France »). **À éviter** : un CTA partenaire avant le CTA client. |
| 3 | Dattak : accueil | https://www.dattak.io/fr | Site réel (FR) | [capture](captures/03-dattak.jpg) | Hero sombre (dégradé noir vers marine, halo brique en haut à gauche), titre centré en Inter 79 px graisse 400. La baseline « Opérateur de gestion des risques technologiques » est passée dans une pastille au-dessus du titre, et le titre reste une catégorie : « Dattak réduit et assure les risques technologiques des entreprises ». Bouton terracotta `#C4684A` : texte blanc à 3,9:1, sous le seuil AA. **Contre-exemple** confirmé : le titre de Rempart doit nommer le résultat pour le dirigeant, pas la catégorie. |

## Quiz et diagnostic

| # | Référence | URL | Source | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 4 | MonAideCyber (ANSSI) : diagnostic en accès libre | PDF d'origine mort : https://monaidecyber.ssi.gouv.fr/fichiers/Plaquette_MonAideCyber.pdf redirige vers monaide.cyber.gouv.fr et affiche une page blanche. Page vue à la place : https://monaide.cyber.gouv.fr/diagnostic-libre-acces | Site public | [capture](captures/04-monaidecyber-diagnostic.jpg) | Charte de l'État (police Marianne), titre violet, illustration au trait d'une personne devant un écran. Aucun e-mail pour commencer, mais une case CGU obligatoire avant « Je commence le diagnostic ». Un lien propose un diagnostic accompagné. Les « 6 recommandations prioritaires » de la plaquette n'ont pas pu être vérifiées. **À reprendre** : l'illustration au trait et le démarrage sans e-mail. **À éviter** : une case à cocher avant la première question. Pour Rempart, le résultat reste : un niveau, puis 3 actions, sans e-mail. |
| 5 | Stoïk : Assurance | https://www.stoik.com/assurance | Site réel (FR) | [capture](captures/05-stoik-assurance.jpg) | Même hero bleu, « Le risque cyber. Entièrement couvert. » avec la 2e ligne en rose, une photo et des tuiles d'icônes. Les deux boutons visent les courtiers. Sous le hero, 3 chiffres en pastilles colorées : 2 Md€, 10 M€, 150 M€. **Correction** : aucun scan externe gratuit n'est proposé sur cette page, les scans sont « inclus dans chaque police ». Le principe « outil gratuit avant le commercial » n'est donc pas illustré ici. **À reprendre** : les chiffres en pastilles sous le hero. |
| 6 | Coverall : estimateur | https://www.coverall.com/commercial-cleaning-services/janitorial/ | Site réel (US, nettoyage), référence transversale | [capture](captures/06-coverall.jpg) | Hero photo d'équipe, titre en capitales Roboto Condensed 900, bouton vert « Get a free cleaning quote ». **Correction** : le bloc « Get an instant cleaning quote » est sous la ligne de flottaison et c'est un formulaire de 10 champs (7 obligatoires, dont nom, e-mail, téléphone et code postal) avant toute fourchette, plus un reCAPTCHA. Ce n'est pas « 2 champs puis un prix ». **À éviter** : l'estimateur qui exige l'identité avant le prix. **À reprendre** : la promesse écrite (« fourchette instantanée selon la surface et la fréquence »). Le simulateur de Rempart : 1 champ (postes), prix tout de suite, aucune coordonnée. |

## Timeline « En cas d'attaque »

| # | Référence | URL | Source | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 7 | Dattak : Assurance Cyber Proactive | https://www.dattak.io/fr/cyberattack (redirige vers https://www.dattak.io/fr/insurance) | Site réel (FR) | [capture](captures/07-dattak-cyberattack.jpg) | Hero sombre, « L'Assurance Cyber Proactive » en Inter 72 px. Le texte confirme le découpage « Avant l'incident », « Pendant l'incident », « Après l'incident », avec deux délais chiffrés : « scan et analyse en 5 minutes », « intervention en moyenne en moins de 2 minutes ». **À reprendre** : la timeline en 3 temps et un délai moyen chiffré dans la partie « pendant ». |
| 8 | Dattak : gestes des premières heures | https://www.dattak.io/fr/blog/dattak-blog-gestes-cyberattaque-reponse-incident | Site réel (FR), blog | [capture](captures/08-dattak-blog-gestes.jpg) | Article du 25 novembre 2025, puis une infographie « Premières actions en cas de cyberattaque » en illustration plate. Gestes confirmés : déconnecter les systèmes compromis, isoler les sauvegardes, couper internet si nécessaire. Erreurs citées : redémarrer trop tôt, payer une rançon sans accompagnement juridique, agir seul. Résumé de l'article : « Déconnecter, isoler, documenter ». **À reprendre** : ces 3 verbes pour le bloc « 3 réflexes en attendant notre appel ». **À éviter** : le cadenas et le point d'exclamation rouge de l'infographie. |
| 9 | Arctic Wolf : How it works | https://arcticwolf.com/how-it-works/ | Site réel (US) | [capture](captures/09-arcticwolf-how.jpg) | Hero marine `#00112C` avec rayons de lumière bleue, titre « Work For You » (forma-djr-display, 600), texte en Lato. Sous le hero, 5 chiffres en ligne, dont « <1 actionable event per day ». La page décrit le « Concierge Delivery Model » (alertes triées, conseils suivis). Un lien « Experienced a Breach? » est dans l'en-tête. **À reprendre** : montrer qui agit à chaque étape ; un chiffre qui parle au dirigeant (« moins d'une alerte utile par jour ») ; le lien d'urgence dans l'en-tête. |

## Tarifs

| # | Référence | URL | Source | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 10 | Huntress : Pricing | https://www.huntress.com/pricing | Site réel (US) | [capture](captures/10-huntress-pricing.jpg) | **Correction** : au-dessus de la ligne de flottaison, pas de prix. La moitié droite est un formulaire « Get pricing » (e-mail pro, entreprise, nombre de postes, activité, produit). Les prix publics sont plus bas : Managed EDR à 8,99 $ par poste et par mois, ITDR à 4,80 $ par identité, prix catalogue dégressif. La phrase « 24/7 SOC Management included at no additional cost » est bien là. **À reprendre** : le prix unitaire public et le « tout compris » explicite. **À éviter** : un formulaire « obtenir un prix » au-dessus de prix pourtant publics, qui fait croire qu'il faut donner son e-mail. |
| 11 | Arctic Wolf : Bundles | https://arcticwolf.com/solutions/bundles/ | Site réel (US) | [capture](captures/11-arcticwolf-bundles.jpg) | Hero en dégradé cyan vers marine, titre « Bundles ». Les 3 paliers Core, Plus et Total sont confirmés, avec des options de garantie financière chiffrées (à partir de 100 k$). Aucun prix affiché. **À reprendre** : 3 paliers et une ligne « garantie » ou « engagement de délai » par palier. **À éviter** : des paliers sans prix. |
| 12 | Stoïk : prix d'une cyber assurance | https://www.stoik.com/prix-assurance-cyber | Site réel (FR), blog | [capture](captures/12-stoik-prix.jpg) | Article de blog daté du 14 juin 2023, fond blanc, titre en bleu puis prune `#320A37`, photo de banque d'images. Le contenu donne des prix d'appel par secteur (de 115 à 172 € par mois) et les hypothèses de calcul (chiffre d'affaires, franchise, plafond). **À reprendre** : une FAQ prix sous la grille, avec les hypothèses écrites. **À éviter** : une page prix datée de 2023 et une photo de banque d'images. |

## Preuves et réassurance

| # | Référence | URL | Source | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 13 | Advens : qualification PDIS | https://www.advens.com/media/news-advens/qualification-pdis/ | Site réel (FR) | [capture](captures/13-advens-pdis.jpg) | Article du 30 septembre 2025. Hero bleu très clair `#E6F6FF`, titre Space Grotesk 700 en `#1F1F1F`, visuel du « Visa de sécurité » de l'ANSSI, lien vers la qualification dans le texte. C'est l'une des deux seules pages du panel avec un hero clair. Un bouton flottant « Assistance 24/7 CERT Advens » reste en bas à droite, mais son texte blanc sur `#0AB3FF` ne fait que 2,4:1. **À reprendre** : le bandeau de certifications sobre, avec le logo officiel et un lien vers le justificatif (placeholders sur la démo). **À éviter** : un bouton d'urgence sous le seuil de contraste. |
| 14 | Dattak : Témoignages | https://www.dattak.io/fr/temoignages | Site réel (FR) | [capture](captures/14-dattak-temoignages.jpg) | Hero sombre « Ils nous font confiance ». Chaque témoignage est une carte : vidéo à gauche, à droite une citation d'une phrase en italique, le nom, la fonction et l'entreprise. **À reprendre** : 3 témoignages courts sur la home (nom, fonction, taille d'entreprise), la vidéo en option, et la page complète en lien. |
| 15 | Arctic Wolf : Inside the SOC | https://arcticwolf.com/uk/inside-the-soc/ | Site réel (UK) | [capture](captures/15-arcticwolf-soc.jpg) | Photo réelle d'un analyste avec un casque, très assombrie, « SOC » en lettres géantes, boutons orange « Meet our teams » et « How our SOC works ». **À reprendre** : de vraies photos de l'équipe à la place des hackers à capuche. **À éviter** : l'assombrissement dramatique. Chez Rempart, des photos claires, en lumière du jour. |

## NIS2 et offres par maturité

| # | Référence | URL | Source | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 16 | Stoïk : NIS2 | https://www.stoik.com/nis2 | Site réel (FR) | [capture](captures/16-stoik-nis2.jpg) | Contenu vu. Hero bleu avec un titre-question, « Êtes-vous concerné par NIS2 ? », un chiffre (environ 160 000 entités européennes) et le bouton « Vérifier si je suis concerné ». Les intertitres sont en langage courant : « Réglons d'abord le point qui fâche. », « Une directive, pas un règlement. ». **À reprendre** : le titre-question avec un test en bouton, et ce ton d'intertitre pour la page longue « NIS2 pour les PME ». |
| 17 | Advens : offres mySOC | https://www.advens.com/mysoc/offres/ | Site réel (FR) | [capture](captures/17-advens-mysoc.jpg) | Bandeau noir, titre bleu `#006BFF` en Space Grotesk 56 px, sous-titre « Une trajectoire adaptée à votre contexte », logos de clients. **Correction** : il n'y a pas de paliers nommés par besoin. L'offre est une trajectoire en 3 phases (schéma en image), puis 3 valeurs (Efficient, Adaptatif, Collaboratif). **À reprendre** : l'idée de trajectoire (commencer petit, élargir). Les noms Essentiel, Pro et NIS2 restent une décision propre à Rempart. |
| 18 | Cybermalveillance.gouv.fr : infographie maturité TPE-PME 2025 | https://www.cybermalveillance.gouv.fr/medias/2025/10/250910_InfographieMaturiteCyberTPE-PME_SCREEN.pdf | Document public (PDF, 2 pages) | [capture](captures/18-cybermalveillance-infographie.jpg) | Ouvert dans la visionneuse PDF. Bleu marine et rouge-orangé, chiffres en jauges : 16 % des entreprises se déclarent victimes d'au moins un incident, 80 % ne sont pas préparées, 3 TPE-PME sur 4 investissent moins de 2 000 € par an. La source est en pied : enquête OpinionWay, 588 entreprises de moins de 250 salariés, juin et juillet 2025. **À reprendre** : 2 ou 3 chiffres officiels avec leur source écrite. **À éviter** : le cadenas rouge ouvert qui illustre le 16 %. |

---

## Galeries d'inspiration

Retenues pour Rempart : dirigeants non techniques, ton rassurant et pédagogique, direction B. Les numéros suivent ceux du bench. Les contre-exemples sont signalés.

| # | Référence | URL | Source | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 19 | Latch : Cybersecurity Landing Page (Dipa Inhouse) | https://dribbble.com/shots/27193953-Latch-Cybersecurity-Landing-Page | Dribbble | [capture](captures/19-dribbble-latch.jpg) | L'une des rares maquettes claires de la recherche : fond blanc bleuté, titre fin centré, bouton pastille bleu, beaucoup d'air. Plus bas, la photo d'une personne souriante. **À reprendre** : la densité et la clarté, proches de la direction B. **À éviter** : le bouclier-serrure en 3D isométrique, cousin du cadenas. |
| 20 | Ghost UI risk score widget (Evil Martians) | https://dribbble.com/shots/24816320-Ghost-UI-risk-score-widget | Dribbble | [capture](captures/20-dribbble-risk-score.jpg) | Une jauge en arc, un chiffre (2.9), un libellé (« Low ») et une légende (« Median app risk »). Le niveau ne passe jamais par la couleur seule. **À reprendre** pour le résultat du quiz, mais sur fond clair : jauge, niveau écrit, une phrase d'explication. |
| 21 | B2B SaaS Pricing Page UX (Katerina Bulkina) | https://dribbble.com/shots/27813140-B2B-SaaS-Pricing-Page-UX-for-Plans-Trials-Enterpris | Dribbble | [capture](captures/21-dribbble-pricing-seat.jpg) | Titre « Pay per seat. Talk to us when you need more control. », 12 $ par siège et par mois, le total annuel et le prix mensuel écrits sous le montant, et « See your estimate below before you start ». Deux cartes numérotées : libre-service et devis. **À reprendre** : la phrase de calcul sous le prix et l'estimation avant tout engagement, pour le simulateur. **À éviter** : le dégradé violet et le jaune fluo. |
| 22 | Cybersecurity Landing Page (FleexStudio) | https://dribbble.com/shots/26361362-Cybersecurity-Landing-Page | Dribbble | [capture](captures/22-dribbble-contre-exemple.jpg) | **Contre-exemple** : cadenas vert néon, main robotique, silhouette à capuche, fond noir. Il coche le premier interdit de la liste. Il représente bien la recherche : environ trois quarts des vignettes « cybersecurity landing page » sont sombres (noir, néon vert ou violet). |
| 23 | Enshore Security (Ricardo Dol) | https://www.awwwards.com/sites/enshore-security | Awwwards (nominé, décembre 2023) | [capture](captures/23-awwwards-enshore.jpg) | Prestataire néerlandais d'audit et de sécurité. Hero marine, photo de la Terre la nuit. Plus bas dans l'aperçu : 3 chiffres de volume (1 500+ audits internes, 400+ audits de certification, 30+ ISMS gérés) à côté d'un encart « Laissez-nous vous aider » avec 2 auditeurs nommés, en photo, avec leur qualification. Le site en ligne ne répond plus (nom de domaine introuvable). **À reprendre** : chiffres et visages nommés dans le même bloc. **À éviter** : la Terre vue de l'espace. |
| 24 | SAFE security | https://www.awwwards.com/sites/safe-security-1 | Awwwards (mention honorable) | [capture](captures/24-awwwards-safe.jpg) | Version primée : fond marine, « Predicting cyber breaches », un score « 3.14, Risk: Low » dans un nuage de points cyan, bouton cyan. Le site actuel a changé (fond noir et violet, autre message). **À reprendre** si la direction C est retenue : le score et son libellé dans le hero. **À noter** : une fiche Awwwards montre la version primée, pas forcément le site actuel. |
| 25 | Steadily (assurance de bailleurs) | https://onepagelove.com/steadily | One Page Love (publié le 16 juin 2022) | [capture](captures/25-onepagelove-steadily.jpg) | Fond crème, titre serif (Faustina) « Get fast, affordable landlord insurance », un seul champ (l'adresse) et un bouton « Get a quote », illustration au trait (main, téléphone avec un devis à 60 $ par mois, maison), logos presse puis avis 5 étoiles. **À reprendre** : c'est la direction B appliquée à un service de protection. Un champ dans le hero pour obtenir un prix, des illustrations au trait, aucune image de menace. |
| 26 | The State of Software Delivery in Healthcare (Thoughtbot) | https://onepagelove.com/the-state-of-software-delivery-in-healthcare | One Page Love | [capture](captures/26-onepagelove-thoughtbot.jpg) | Rapport en une page : grands titres serif (Redaction), sections blanc cassé, grands pourcentages et graphiques, méthode d'enquête écrite. **À reprendre** : la mise en scène des chiffres sourcés (n° 18) pour la section NIS2 et la page longue. Fond brun sombre du hero non retenu. |

### Galeries : requêtes lancées

| Plateforme | Requêtes | Résultat |
|---|---|---|
| Behance | « cybersecurity landing page » | Inaccessible : la page renvoie « HTTP ERROR 400 » au navigateur automatisé. |
| Dribbble | « cybersecurity landing page », « risk score quiz », « pricing per seat », « security quiz », « managed security services website » | 4 retenues (n° 19 à 22, dont 1 contre-exemple). « security quiz » ne renvoie que des applis de formation sombres. |
| Pinterest | « cybersecurity web design navy cyan » | Inaccessible sans compte : une fenêtre de connexion couvre les résultats et aucune URL d'épingle n'est exposée. Derrière, les vignettes sont presque toutes marine, avec boucliers et cadenas. |
| Awwwards | « cybersecurity », « security », « security saas » | 2 retenues (n° 23, 24). Beaucoup de sites primés ont changé ou ont disparu depuis. |
| Land-book | « security » | Inaccessible (protection anti-robots, challenge Cloudflare). |
| Lapa Ninja | « security », catégorie security | Inaccessible (protection anti-robots, « Sorry, you have been blocked »). |
| One Page Love | « security », « cyber », « insurance » | 2 retenues (n° 25, 26). « security » donne surtout des gabarits sombres (Retinax, œil en gros plan : contre-exemple). |
| Godly | page d'accueil, « Websites » | Rien de retenu : pas de recherche ni de catégorie « security » sans compte, godly.website redirige vers recent.design et les fiches renvoient vers l'accueil. |

---

## Mobile

Trois sites vus en 390 × 844 px :

| Site | Capture | Ce qu'on observe |
|---|---|---|
| Stoïk : Cybersécurité | [capture](captures/mobile-stoik.jpg) | Le hero bleu tient sur l'écran, les 2 boutons passent l'un sous l'autre en pleine largeur, « Devenir partenaire » en premier. Aucun numéro ni bouton d'urgence, aucun élément fixe. |
| Advens : offres mySOC | [capture](captures/mobile-advens.jpg) | Le seul site du panel avec un bouton d'urgence fixe sur mobile : la pastille « Assistance 24/7 » reste en bas à droite pendant le défilement. Mais son contraste est de 2,4:1 et la page n'a aucun lien `tel:` : le bouton ne lance pas d'appel. |
| Arctic Wolf : How it works | [capture](captures/mobile-arcticwolf.jpg) | Les 5 chiffres passent en grille de 2 colonnes. Le lien « Experienced a Breach? », visible dans l'en-tête sur desktop, disparaît dans le menu burger sur mobile. |

Ce que ces observations confirment pour Rempart :
- une barre d'urgence fixe en bas (« Urgence : nous appeler », rouge discret, 1 tap). Elle porte un vrai lien `tel:` et un contraste d'au moins 4,5:1 (blanc sur `#C8102E` : 5,9:1). Elle ne se cache jamais dans le menu ;
- un quiz en plein écran, une question par écran, une barre de progression, un bouton retour. Aucune page vue n'affiche de quiz directement (Stoïk renvoie vers un test NIS2 par un bouton) : c'est un point de différence ;
- une grille tarifaire en carrousel horizontal avec le palier « Pro » centré par défaut ;
- les chiffres clés en grille de 2 colonnes, comme Arctic Wolf.

---

## Synthèse du moodboard

**Ajustements après observation (2026-11-12)**
- Le panel sectoriel est sombre : Huntress (`#050707`), Arctic Wolf (`#00112C`) et Dattak (noir vers marine) ont un hero sombre, Stoïk un bleu saturé. Seuls Advens (article PDIS, `#E6F6FF`) et MonAideCyber ont un hero clair. Sur Dribbble, environ trois quarts des vignettes sont sombres. La direction B se démarque donc du secteur : la recommandation est maintenue, avec cette raison en plus.
- Aucun concurrent ne montre un prix sans demander de coordonnées en premier (Huntress cache ses prix sous un formulaire, Coverall exige 7 champs, Arctic Wolf n'affiche pas de prix). Le simulateur sans e-mail de Rempart devient un argument de différence, pas une simple reprise.
- La palette et les tokens ne changent pas : aucune observation ne le justifie. Les contrastes ont été recalculés et sont confirmés.

**Direction A : « Tour de contrôle »**
- Fond marine profond, données en cyan, une timeline et un compteur de délai.
- L'expertise se montre par la précision (horaires, délais, étapes).
- Le risque est d'être trop froid. On le compense par des photos d'équipe.
- C'est le registre par défaut du secteur (n° 1, 9, 15) : Rempart s'y fondrait.

**Direction B : « Le cabinet de confiance »** (recommandée)
- Fond blanc cassé dominant, marine pour la structure, cyan en touches.
- Un ton de médecin de famille : schémas simples, illustrations au trait, beaucoup d'air.
- C'est la plus cohérente avec « rassurant et pédagogique » et avec la cible de dirigeants non techniques.
- Références vues : Steadily (n° 25) pour le hero à un champ et les illustrations au trait, MonAideCyber (n° 4) pour l'illustration, Thoughtbot (n° 26) pour les chiffres sourcés.

**Direction C : « Le tableau de bord »**
- Des cartes façon interface (score de risque, statut « surveillé »), des micro-interactions.
- Le produit est montré comme il sera vécu, avec le score du quiz en écho.
- Le risque est de faire « éditeur SaaS » plutôt que service humain.
- Références vues : la jauge Evil Martians (n° 20) et le score SAFE (n° 24). Stoïk l'utilise déjà en hero (n° 2).

**Palette recommandée** (contrastes WCAG recalculés le 2026-11-12)

| Rôle | Hex | Usage |
|---|---|---|
| Marine | `#0B1F3A` | Titres, fonds sombres. Contraste de 15,2:1 sur blanc cassé |
| Blanc cassé | `#F7F5F0` | Fond principal |
| Texte | `#1E293B` | Corps de texte (13,4:1) |
| Texte secondaire | `#5B6B80` | Légendes (5,0:1) |
| Cyan accent | `#00B8D9` | Accent sur fond marine seulement (7,0:1). Jamais pour du texte sur fond clair |
| Cyan texte | `#006B85` | Liens et accent sur fond clair (5,6:1) |
| Rouge urgence | `#C8102E` | Bouton et numéro d'urgence uniquement. Blanc sur rouge : 5,9:1 |

Observé chez Huntress (n° 1) : un bouton cyan à texte sombre. L'équivalent Rempart (texte marine sur `#00B8D9`) fait 7,0:1. Il peut servir de CTA dans les sections sombres, sans nouveau token.

**Polices Google Fonts**
- **Manrope** (600 à 800) pour les titres, **Manrope** (400 et 500) pour le texte. Une seule famille, rapide à charger.
- Alternative : **Plus Jakarta Sans** pour les titres.
- Option : **JetBrains Mono** (500) pour les horodatages de la timeline (« T+05 min »).
- Observé : les références les plus rassurantes des galeries (n° 25, 26) titrent en serif. Le brief impose une grotesque, donc rien ne change. Une serif de titre reste une piste à tester en atelier.

**3 choses à ne pas faire**
1. Pas de hacker à capuche, de cadenas rouge, de code Matrix ni de compte à rebours anxiogène.
2. Pas de rouge hors urgence : sinon il ne signale plus rien.
3. Pas de quiz qui exige l'e-mail avant d'afficher le score.

---

## Design tokens (format design system)

Contrastes calculés selon la formule WCAG 2.1, recalculés le 2026-11-12 (valeurs inchangées). Le fond de référence est `bg.default` (`#F7F5F0`).

### Couleurs

| Token | Hex | Usage | Contraste |
|---|---|---|---|
| `brand.navy` | `#0B1F3A` | Titres, fonds sombres, bouton primaire | 15,2:1 sur bg |
| `brand.navy-hover` | `#132E54` | Survol du bouton primaire | 12,5:1 |
| `brand.cyan` | `#00B8D9` | Accent sur fond navy uniquement | 7,0:1 sur navy, **2,2:1 sur bg, donc jamais en texte clair** |
| `brand.cyan-text` | `#006B85` | Liens et accent sur fond clair | 5,6:1 |
| `semantic.urgent` | `#C8102E` | Bouton et numéro d'urgence **uniquement** | 5,4:1. Blanc sur rouge : 5,9:1 |
| `semantic.error` | `#B42318` | Erreurs de formulaire (teinte distincte de l'urgence) | 6,0:1 |
| `semantic.success` | `#15803D` | Confirmation, niveau de risque « faible » | 4,6:1 |
| `semantic.warning` | `#B45309` | Niveau de risque « moyen », avertissements | 4,6:1 |
| `neutral.900` | `#1E293B` | Corps de texte | 13,4:1 |
| `neutral.600` | `#5B6B80` | Texte secondaire | 5,0:1 |
| `neutral.400` | `#7A8699` | Bordures de champs (contraste non textuel ≥ 3:1) | 3,4:1 |
| `neutral.200` | `#E2E0D8` | Séparateurs décoratifs | décoratif |
| `bg.default` | `#F7F5F0` | Fond de page | — |
| `bg.surface` | `#FFFFFF` | Cartes, champs | — |
| `bg.inverse` | `#0B1F3A` | Sections sombres (timeline, footer) | — |

Le niveau de risque du quiz ne doit jamais être signalé par la couleur seule : chaque niveau porte aussi un libellé et une icône.

### Typographie (Manrope ; JetBrains Mono en option)

| Token | Taille (mobile / desktop) | Graisse | Interligne |
|---|---|---|---|
| `display` | 36 / 56 px | 800 | 1,1 |
| `h1` | 30 / 44 px | 800 | 1,15 |
| `h2` | 24 / 32 px | 700 | 1,2 |
| `h3` | 20 / 24 px | 700 | 1,3 |
| `body-lg` | 18 / 20 px | 400 | 1,6 |
| `body` | 16 / 17 px | 400 | 1,6 |
| `small` | 14 px | 500 | 1,5 |
| `mono` (timeline) | 14 / 15 px | 500 | 1,4 |

### Espacement, rayons, ombres, motion

| Catégorie | Tokens |
|---|---|
| Espacement (base 4) | `space.1`=4, `2`=8, `3`=12, `4`=16, `6`=24, `8`=32, `12`=48, `16`=64, `24`=96 px. Sections : 64 px en mobile, 96 px en desktop |
| Rayons | `radius.sm`=6 px (champs), `radius.md`=10 px (boutons), `radius.lg`=16 px (cartes), `radius.full` (pastilles) |
| Ombres | `shadow.sm` = 0 1px 2px rgba(11,31,58,.08) ; `shadow.md` = 0 4px 16px rgba(11,31,58,.10) ; `shadow.focus` = 0 0 0 3px #006B85 |
| Motion | `duration.fast`=120 ms (survol), `duration.base`=200 ms (ouverture, transitions du quiz), `duration.slow`=320 ms (révélation du score). `ease.out` = cubic-bezier(.2,.8,.2,1), `ease.in-out` = cubic-bezier(.4,0,.2,1). Respecter `prefers-reduced-motion` : animations remplacées par un fondu de 0 ms |

### Composants clés

**Bouton primaire** : fond `brand.navy`, texte blanc, `radius.md`, hauteur 48 px (44 px minimum).
- Survol : `brand.navy-hover`.
- Focus : `shadow.focus` visible.
- Actif : translateY(1px).
- Désactivé : opacité 0,5, `aria-disabled`, curseur not-allowed.
- Chargement : spinner et libellé « Envoi… ».

**Bouton secondaire** : fond transparent, bordure de 1,5 px `brand.navy`, texte navy. Mêmes états. Survol : fond `#0B1F3A0D`.

**Bouton urgence** : fond `semantic.urgent`, texte blanc, icône téléphone et numéro visible. Fixe en bas sur mobile, dans l'en-tête sur desktop.

**Carte d'offre** : fond `bg.surface`, `radius.lg`, `shadow.sm`, padding `space.6`. Elle contient une icône au trait, un titre `h3`, 3 puces et un lien. Au survol : `shadow.md`.

**Carte de tarif** : le palier mis en avant porte une bordure de 2 px `brand.cyan-text` et un badge « Le plus choisi ».

**Formulaire et quiz** :
- labels visibles au-dessus des champs, hauteur 48 px, bordure `neutral.400` ;
- erreur affichée sous le champ en `semantic.error`, avec icône et texte, et `aria-describedby` ;
- quiz : une question par écran, barre de progression « 2/5 », gros boutons-réponses en cartes, bouton Retour.

| À faire | À ne pas faire |
|---|---|
| Un seul bouton primaire par écran | Deux boutons primaires concurrents dans le hero |
| Le rouge réservé à l'urgence, et l'erreur dans une teinte distincte | Le rouge pour la décoration ou les badges promotionnels |
| Le cyan en accent sur fond navy | Du texte cyan clair sur blanc cassé (2,2:1) |
| Le score du quiz avec un libellé, une couleur et une icône | Le score signalé par la couleur seule |
| Des labels visibles et une erreur expliquée sous le champ | Les placeholders utilisés comme labels, ou « Champ invalide » |
| Un focus visible sur tous les éléments interactifs | `outline: none` sans remplacement |
| Les animations désactivées avec `prefers-reduced-motion` | Un compteur ou un radar animé en boucle |
