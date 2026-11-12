# Benchmark visuel : Liasse (fintech et SaaS de gestion, entreprise fictive)

## Limites, à lire en premier

Mise à jour du 2026-11-12, faite avec un vrai navigateur (Chrome piloté par Playwright). La version précédente avait été écrite sans réseau, à partir des seuls résultats de recherche.

- **Ce qui a été vu** : 14 des 20 références d'origine. 10 par leur URL d'origine (n° 1, 2, 3, 6, 7, 8, 9, 15, 16, 17), 4 par une page équivalente sur le même sujet, parce que l'URL d'origine est bloquée (n° 13, 14, 18, 20). Captures en 1440 × 900 px, au-dessus de la ligne de flottaison, dans [`captures/`](captures/), avec parfois une seconde capture ciblée. Les couleurs et les polices citées ont été relevées dans la page (`getComputedStyle`). Les chiffres cités sont ceux affichés le 2026-11-12.
- **Ce qui reste bloqué** :
  - Behance (n° 4 et 12) : erreur HTTP 400 pour un navigateur automatisé.
  - Abby (n° 5) : erreur 403 CloudFront, deux essais à une heure d'écart.
  - Godly (n° 10 et 11) : les deux fiches redirigent vers recent.design, sans la fiche. Le site de Revolut affiche un challenge Cloudflare, non contourné.
  - Lapa Ninja (n° 13) et Land-book (n° 14) : blocage Cloudflare.
  - Pinterest (n° 18, 19, 20) : mur de connexion par-dessus le visuel. Le titre et la description des épingles se lisent, pas l'image. Aucune capture de Pinterest (elle montrerait un formulaire de connexion).
- **Remplacements** : 6 références ajoutées (n° 21 à 26), toutes ouvertes et capturées. Elles remplacent les n° 4, 10, 11, 12 et 19, et complètent la section Tarifs.
- **Corrections importantes** :
  - Qonto (n° 2) n'affiche **aucun numéro d'immatriculation de plateforme agréée** sur les 3 pages ouvertes. Le seul numéro visible est celui d'établissement de paiement (ACPR, CIB 16958). Pennylane non plus, mais il montre le logo officiel « Plateforme agréée ».
  - Mercury (n° 1) n'a ni « beaucoup de blanc » ni « un seul bouton » : photo pleine page, champ e-mail puis deux boutons.
  - Les palettes Dribbble (n° 7, 8) sont extraites automatiquement de l'image, pas choisies par le designer. La n° 8 est grise, pas « chaude ».
  - Acctual (n° 13) ne réunit pas factures émises et reçues sur une page. Maze (n° 14) n'affiche plus aucun prix.
  - **DM Sans, servie par Google Fonts, n'a pas de chiffres tabulaires** : `font-variant-numeric: tabular-nums` ne change rien (test fait dans le navigateur). Outfit les a. Les tokens typo sont corrigés.
  - Indy (n° 16), concurrent direct sur les artisans, a déjà un hero crème `#FEF7EC`, une photo d'artisan et une carte « Facture électronique · Payée ». La synthèse en tient compte.
- **Mobile** : 3 sites capturés en 390 × 844 px (Indy, Pennylane, Mercury). Voir la section « Mobile (observé) ».
- **Bannières cookies** : refusées partout où un refus existait (« Reject all », « Continuer sans accepter », « Reject »). Sur Maze, préférences enregistrées sans rien cocher. Sur SaaS Landing Page et Hangar, le bandeau n'offre que « I agree » ou « Accept » : il a été masqué pour la capture, rien n'a été accepté.

| Source | Références d'origine | Vues le 2026-11-12 |
|---|---|---|
| Sites réels du secteur | 4 | 3 (Abby bloqué) |
| Behance | 2 | 0 (erreur 400) |
| Dribbble | 3 | 3 |
| Pinterest | 3 | 0 visuel (mur de connexion), 2 sources d'origine ouvertes |
| Awwwards | 1 | 1 (le site primé ne répond plus) |
| Land-book | 1 | 0 (Cloudflare), page d'origine ouverte |
| Lapa Ninja | 1 | 0 (Cloudflare), site d'origine ouvert |
| SaaS Landing Page | 2 | 2 |
| One Page Love | 1 | 1 |
| Godly | 2 | 0 (redirection) |
| **Ajouts** (Dribbble 3, One Page Love 2, site réel 1) | | 6 |

---

## Hero

| # | Référence | URL | Source | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 1 | Mercury | https://saaslandingpage.com/mercury/ et le site https://mercury.com/ (analyse complémentaire : https://swipefile.com/ai-powered-finance-orchestration-built-into-accounts) | SaaS Landing Page (fiche d'octobre 2026) et site réel (US) | [fiche](captures/01-mercury-slp.jpg), [site](captures/01-mercury-site.jpg) | **Correction** : la fiche classe le site « Dark ». Hero photo pleine page (un bureau posé dans une vallée brumeuse), titre centré « Radically different banking » en Arcadia Display 49 px, graisse 480, `#EDEDF3`. Sous le titre : un champ « Enter your email », le bouton « Open account » (`#5266EB`, texte blanc à 4,71:1, rayon 32 px) **et** un second bouton « Launch demo ». Une mention reste épinglée en bas du hero : « Mercury is a fintech company, not an FDIC-insured bank ». Les micro-animations n'ont pas été constatées. L'analyse Swipefile (juillet 2026) décrit une version antérieure, sur fond étoilé. **À reprendre** : le champ e-mail dans le hero ; la mention « Liasse n'est pas une banque » écrite près du CTA, comme Mercury, pour répondre à la contrainte réglementaire du brief. **À éviter** : la photo d'ambiance sans produit. |
| 2 | Qonto | https://qonto.com/fr?tp=1 et https://qonto.com/fr/accountants/for-your-clients | Site réel (France) | [accueil](captures/02-qonto.jpg), [experts-comptables](captures/02-qonto-experts-comptables.jpg) | Accueil : hero noir, rendu 3D d'une carte métal, titre QontoSans 700 de 68 px en 3 phrases (« Compte pro. Financement. Facturation électronique. »), « 4,7 sur 5 » Trustpilot. Bandeau : « 750 000 entreprises font déjà confiance à Qonto ». La page dit « Certifié Plateforme Agréée ». **Correction** : aucun numéro d'immatriculation PA sur l'accueil, la page experts-comptables ni la page `/accountants/e-invoicing`. Les numéros du pied de page sont ceux de l'ACPR (CIB 16958), de l'ORIAS et du RCS. Page experts-comptables : fond blanc, titre noir de 56 px, 4 coches, « Parler à un conseiller » (`#050505`, rayon 8 px), capture de l'app avec la mention « Mon comptable · Synchronisé ». Le texte explique l'invitation des clients « en un clic » et l'ouverture de compte « en moins de 2 minutes ». **Contre-exemple** : la même page annonce « 600 000 entreprises », contre 750 000 sur l'accueil. **À reprendre** : la structure de la page experts-comptables (bénéfices, invitation des clients, formats) pour la section 5. |
| 3 | Finpay, Fintech Landing Page (Dipa Inhouse) | https://dribbble.com/shots/24820686-Finpay-Fintech-Landing-Page | Dribbble | [vignette](captures/03-dribbble-finpay.jpg), [bloc courbe](captures/03-dribbble-finpay-bento.jpg) | Maquette claire, sarcelle et blanc. Hero « Get paid early, save automatically all your pay. » avec **un seul champ** (« Your business email ») et « Get Started ». **Correction** : les blocs de fonctionnalités ne suivent pas « facturation, intégrations, trésorerie ». Cette phrase n'est que l'accroche. Les blocs sont : virements gratuits, comptes multiples, sécurité, puis une grille avec « 3k+ », un retrait instantané et une carte « Summary $1,876,580 » avec une courbe sur 6 mois. Puis 3 étapes, 3 chiffres et 2 formules (2,99 £ et 6,99 £). **À reprendre** : le champ unique du hero et la carte courbe et montant, pour la direction C. |
| 4 | Fintt.te, Landing Page (Fintech) | https://www.behance.net/gallery/141980721/Finttte-Landing-Page-(Fintech) | Behance | Non capturé | **Non vérifié** : Behance renvoie une erreur 400. Remplacé par le n° 22 (Ledgerly), qui montre la composition titre et mockup sur un produit très proche de Liasse. |

## Échéancier de la réforme / pédagogie

| # | Référence | URL | Source | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 5 | Abby, facturation électronique | https://abby.fr/facturation-electronique | Site réel (France) | Non capturé | **Non vérifié** : erreur 403 (CloudFront) sur la page et sur l'accueil. Le calendrier, la gratuité et les notes citées restent à contrôler. Pour l'échéancier, la référence vue est le n° 6. |
| 6 | Pennylane, logiciel de facturation électronique | https://www.pennylane.com/fr/logiciel-facturation-electronique?so=1 | Site réel (France) | [hero](captures/06-pennylane.jpg), [échéancier](captures/06-pennylane-echeancier.jpg) | Entrée par cible en onglets (« Indépendants et TPE », « PME et ETI », « Cabinet expertise comptable »). Titre Manrope 600 de 42 px en `#003D3D`, « facturation électronique » en vert. Bouton `#00F872`, texte `#003D3D` (8,46:1). L'image du hero porte le logo officiel « Plateforme agréée · Facturation électronique · République française », mais aucun numéro. L'échéancier tient en 3 cartes : « 1er septembre 2026 » (réception), « 1er septembre 2027 » (émission des PME, TPE et micro-entreprises), « Dès aujourd'hui ». **Correction** : sur cette page, les dates sont cohérentes. Les incohérences visibles sont ailleurs : le titre de l'onglet dit encore « préparez-vous pour 2026 », et la page annonce « Plus d'un million d'entreprises » puis « +1 500 000 dirigeants, indépendants et directeurs financiers » juste en dessous. **À reprendre** : les 3 cartes datées, lisibles sans couleur. **À éviter** : « Évitez les amendes » dans la 3e carte, l'inverse du ton voulu. |

## Aperçu de l'application / mobile

| # | Référence | URL | Source | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 7 | Fintech mobile app, par Excel Belmiro | https://dribbble.com/shots/15812075-Fintech-mobile-app | Dribbble | [capture](captures/07-dribbble-excel.jpg) | 3 écrans de téléphone sur fond lavande : cartes bancaires, écran d'accueil rose-violet en dégradé avec un personnage 3D, courbe « $11,902 May Income ». La palette affichée compte 6 couleurs, extraites automatiquement de l'image : `#E8DFFB`, `#CAB7F8`, `#AA2DA8`, `#6538E5`, `#613939`, `#C4A9BD`. **À reprendre** : `#E8DFFB` reste une bonne base pour le violet clair (proche de `#ECE4FA`). **À éviter** : le dégradé rose-violet et le personnage 3D, trop « app grand public ». |
| 8 | Invoicing tool, iOS Mobile app (Vishal Reddy) | https://dribbble.com/shots/15711855-Invoicing-tool-iOS-Mobile-app | Dribbble | [capture](captures/08-dribbble-invoicing-ios.jpg) | **Correction** : le visuel n'est pas chaud. C'est un iPhone gris et blanc, avec un bouton vert « Send invoice ». La palette (`#E4E4E4`, `#C2B5B5`, `#0D0D0D`, `#4E3F35`, `#676767`, `#7E7D80`) est extraite de l'image : ce sont surtout des gris. L'intérêt est ailleurs. Le texte explique un flux de création en 2 temps (ce qui change à chaque facture, puis les réglages), et l'écran montre le choix de l'envoi : e-mail ou SMS. **À reprendre** : l'envoi par SMS, utile pour les clients particuliers des artisans. |
| 9 | Tara | https://onepagelove.com/tara | One Page Love (publié le 25 septembre 2026) | [capture](captures/09-onepagelove-tara.jpg) | Coffre crypto et carte de paiement. Police Herokid, couleurs vert, rose et blanc, style « 3D, Minimal, Scroll Effects ». Aperçu mobile : « Money on your side », un champ e-mail et « Join waitlist ». Plus bas, un téléphone et une carte en dégradé vert-rose. **À reprendre** : la mise en scène téléphone et carte, et l'inscription en un champ. **À noter** : produit crypto, à ne pas citer pour le ton. |
| 10 | Revolut | https://godly.website/website/revolut-254 | Godly | Non capturé | **Non vérifié** : redirection vers recent.design. Le site de Revolut Business affiche un challenge Cloudflare. Remplacé par le n° 24 (Depo). |
| 11 | Eco | https://godly.website/website/eco-935 | Godly | Non capturé | **Non vérifié** : redirection vers recent.design. Remplacé par le n° 25 (invoicemon), une démo qui se déroule au scroll. |

## Fonctionnalités

| # | Référence | URL | Source | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 12 | Invo, SaaS product for automatizing invoicing | https://www.behance.net/gallery/157230691/Invo-SaaS-product-for-automatizing-invoicing?locale=en_US | Behance | Non capturé | **Non vérifié** : erreur 400. Remplacé par le n° 23 (séquence de relances DueCourse). |
| 13 | Acctual | Fiche d'origine bloquée : https://www.lapa.ninja/post/acctual-2/ (Cloudflare). Site vu à la place : https://www.acctual.com/ | Site réel (US) | [capture](captures/13-acctual.jpg) | Fond `#F7FAFC`, titre visible « Get paid on time » en Open Runde 600 de 64 px, pastille « Used by 5,000+ businesses worldwide », bouton « Send my first invoice » (`#0D111B`). Les frais sont écrits sous le bouton (carte 2,7 %, virement 1 %, stablecoin 1 %). Puis une facture « From / To » posée comme un vrai papier, avec trombone, clavier et pince. Bandeau « Acctual is joining Altitude ». **Correction** : pas de présentation factures émises et factures reçues ; le site ne parle que d'émettre et d'encaisser. **À reprendre** : les conditions chiffrées sous le CTA ; la facture traitée comme un objet réel. |

## Tarifs

| # | Référence | URL | Source | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 14 | Maze, Pricing | Fiche d'origine bloquée : https://land-book.com/websites/37536-flexible-pricing-and-plans-maze (Cloudflare). Page vue à la place : https://maze.co/pricing/ | Site réel | [capture](captures/14-maze-pricing.jpg) | Titre « Pricing & Packages » en Phonic 300 de 90 px, fond gris chaud clair. **Correction** : la page n'a plus que 2 formules, « Free » et « Enterprise » (« Custom pricing »), et aucun prix. Ce n'est plus une référence de lisibilité. **À éviter** : une page tarifs sans prix. Pour la grille, voir les n° 15 et 21. |
| 15 | Bonsai | https://saaslandingpage.com/bonsai/ et https://www.hellobonsai.com/pricing | SaaS Landing Page (fiche d'octobre 2026) et site réel | [fiche](captures/15-bonsai-slp.jpg), [tarifs](captures/15-bonsai-pricing.jpg) | Fiche : Geist Sans, palette `#003C2F`, `#22AD01`, `#EE8146`. Bonsai (« by zoom ») vise maintenant les « service businesses ». Sous le hero, une barre de 13 onglets (formulaires, projets, temps, facturation, paiements, compta, CRM…). C'est beaucoup pour un artisan. Tarifs : 4 formules (9, 19, 29 et 49 $ par utilisateur et par mois, facturés à l'année), interrupteur « Monthly / Yearly - Up to 4 months free », badge noir « Most popular » sur Premium. **À reprendre** : le badge sobre et une phrase par formule. **À éviter** : 4 formules et 13 onglets ; le bouton en dégradé de la formule mise en avant. |
| 21 | Pennylane, tarifs de la page facturation électronique (ajout) | https://www.pennylane.com/fr/logiciel-facturation-electronique?so=1 | Site réel (France) | [capture](captures/21-pennylane-tarifs.jpg) | 3 cartes « À partir de » 7, 14 et 24 € « /mois HT », celle du milieu en fond sombre. Une ligne par formule, le même bouton « Essayer gratuitement » partout, et sous la grille : « 15 jours d'essai gratuit, sans engagement. ». **À reprendre** : la mention HT sous chaque prix, une phrase par formule, les conditions de l'essai sous la grille. **À éviter** : les prix en vert `#00BD57` sur blanc, à 2,5:1, sous le seuil de 3:1 même en 48 px. |

## Preuves et avis

| # | Référence | URL | Source | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 16 | Indy, page artisans | https://www.indy.fr/artisan/ | Site réel (France) | [capture](captures/16-indy-artisan.jpg) | **Le plus proche de la direction A, et c'est un concurrent.** Hero crème `#FEF7EC`, titre serif (Martina Plantijn 400, 56 px, `#171514`) « L'application tout-en-un des artisans », photo d'un plombier sous un évier, avec deux cartes flottantes : « Facture électronique · Payée » et « Recettes 39 787,09 € ». Pastille « + de 10 000 Artisans déjà clients ! », puis « +700 000 indépendants utilisent Indy au quotidien » et 3 notes (Trustpilot 4,8 et +16 000 avis, App Store 4,9, Play Store 4,8). Bouton rose `#FA5D89` à texte blanc : 3,0:1, sous le seuil AA. **Correction** : le chiffre de 350 000 n'apparaît ni ici ni sur l'accueil, qui n'affiche aucun nombre d'utilisateurs. L'incohérence visible est autre : « A partir de 12 € /mois » dans le hero, puis « Un socle gratuit avec tous les essentiels » plus bas. **À reprendre** : les notes avec leur nombre d'avis et leur source. **À éviter** : le CTA sous le seuil de contraste ; reprendre tel quel le hero crème, photo d'artisan et carte « Payée », que les artisans ont peut-être déjà vu chez Indy. |
| 17 | Invoice Builder by Tola | https://www.awwwards.com/sites/invoice-builder-by-tola | Awwwards (mention honorable, 19 janvier 2024) | [capture](captures/17-awwwards-tola.jpg) | Fiche vue : une tablette posée en biais, « Create beautiful invoices in seconds » sur bleu pâle, et un aperçu mobile avec « Share them as links or export as PDF » et « Select a template ». Le site primé (invoice.tolahq.com) ne répond plus (erreur Cloudflare 1000). L'aperçu en direct et les montants **n'ont pas pu être vérifiés**. Pour la mise en scène d'une facture, voir plutôt les n° 13 et 22. |

## Palette, typo et contre-exemples

| # | Référence | URL | Source | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 18 | Color Palette for Fintech Brand (Yapstone, par Hangar) | Épingle : https://co.pinterest.com/pin/1044694444796643488/ (mur de connexion). Source vue à la place : https://hangar.co/projects/yapstone | Pinterest, puis étude de cas du studio Hangar | [capture](captures/18-hangar-yapstone.jpg) | La description de l'épingle se lit : identité Yapstone par le studio Hangar, avec « Warm Black, Violet, Lilac, Electric Purple, Neutral Cream, Blue, Green, Yellow, Pink, Pastel ». **Correction** : ce n'est pas une palette de 5 couleurs. L'étude de cas montre un noir chaud, un lilas en fond, puis 5 couleurs vives (lilas, bleu, vert, jaune, rose) avec chacune sa version claire, et la police Graphik. **À reprendre** : le couple noir chaud et lilas, et le principe d'une teinte claire par couleur. **À éviter** : les 5 couleurs vives, trop pour Liasse. |
| 19 | Idées « Purple Website Design Inspiration » | https://www.pinterest.com/ideas/purple-website-design-inspiration/916159820380/ | Pinterest | Non capturé | **Non vérifié** : mur de connexion, aucun visuel lisible. Remplacé par le n° 26. |
| 20 | Fintech futuristic hero section design | Épingle : https://www.pinterest.com/pin/842454674093763176/ (mur de connexion). Source vue à la place : https://dribbble.com/shots/24273813-Fintech-futuristic-Website-design | Pinterest, puis Dribbble | [capture](captures/20-dribbble-fintech-futuristic.jpg) | **Contre-exemple** confirmé. « FinNova », « Fintech Made Easy. » en blanc sur noir violacé, halo violet en bas, bouton « Sign Up » violet électrique, chiffres « 4.9+ » (« Starts rating », avec la faute) et « 20k+ ». Au pied du hero : « Mobile payments », « Financial wellness », « Cryptocurrency ». |

## Références ajoutées

| # | Référence | URL | Source | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 22 | Ledgerly, Invoicing App Website & Product UI (Nazar Deynega) | https://dribbble.com/shots/27843787-Ledgerly-Invoicing-App-Website-Product-UI | Dribbble | [vignette](captures/22-dribbble-ledgerly.jpg), [section 90 jours](captures/22-dribbble-ledgerly-forecast.jpg) | Remplace le n° 4. Le concept le plus proche de Liasse : « invoicing and cash-flow app », pour freelances et petits studios, objectif essai gratuit. Corail `#FE1D07`, surfaces crème `#F6F5F0`. Vignette : un téléphone tenu en main, écran « Forecast » avec 30 j, 90 j et 6 mois, « Projected balance €51,300 », et une phrase : « Lowest point Dec 1: €35,200. You stay above your €20k safety line. » Section du site : « 90 days ahead, at a glance », courbe de solde, point bas signalé (« still safe »), 4 montants (« Cash in bank », « Outstanding », « Overdue », « Safe to spend ») et des statuts écrits (« Paid », « Pending », « Overdue »). **À reprendre** : la phrase qui traduit la courbe, le point bas signalé, les statuts écrits. **À éviter** : le corail pour « Overdue » (Liasse le garde pour « payé ») ; le tableau de bord complet en hero. |
| 23 | Automatic invoice reminder sequence, DueCourse (Paul Haydock) | https://dribbble.com/shots/6882240-Automatic-invoice-reminder-sequence-DueCourse | Dribbble | [capture](captures/23-dribbble-duecourse-relances.jpg) | Remplace le n° 12. 4 relances posées sur une ligne de temps (avant l'échéance, le jour même, après). Chaque relance a son délai (« 3 days before invoice is due ») et son objet (« Your invoice is due in 3 days »). Le texte parle de 4 e-mails automatiques. **À reprendre** : la relance montrée comme une frise de 3 ou 4 étapes, avec l'objet réel de chaque message. **À éviter** : le fond bois et le style daté. |
| 24 | Depo Budget App | https://onepagelove.com/depo-budget-app | One Page Love (publié le 13 août 2026) | [capture](captures/24-onepagelove-depo.jpg) | Remplace le n° 10. Hero « Face your number », un téléphone en premier plan, un seul montant (71 $, ce qu'on peut dépenser aujourd'hui), « No spreadsheet. » Polices Archivo et DM Sans. Puis 4 cartes numérotées avec un montant chacune : Income, Essentials, Savings, Today. **À reprendre** : un seul chiffre qui répond à une question ; les cartes numérotées avec montant, pour la trésorerie à 90 jours. **À éviter** : le style brutaliste bleu et jaune fluo. |
| 25 | invoicemon | https://onepagelove.com/invoicemon | One Page Love (publié le 17 juin 2026) | [capture](captures/25-onepagelove-invoicemon.jpg) | Remplace le n° 11. One Page Love le décrit comme une démo interactive qui se déroule au scroll. Couleurs « Beige, Earth Tones », police Inter. Site ouvert : titre Inter 600 « A complete invoicing workflow in your browser », un seul bouton « Create an invoice » (`#1A1816`, texte `#FDFCF8`), des étiquettes de fonctionnalités autour, puis l'éditeur de facture réel. **À reprendre** : la démo au scroll qui montre le vrai produit, une seule fois, pour la section 4. |
| 26 | Recherche Dribbble « purple fintech website » | https://dribbble.com/search/purple-fintech-website | Dribbble | [capture](captures/26-dribbble-recherche-violet.jpg) | Remplace le n° 19. Sur les 8 premières vignettes, 6 sont violet électrique, souvent sur fond sombre, avec de la 3D (ADN, guichet, téléphone flottant). Le violet profond et calme de Liasse (`#2E1A5C`) n'y figure pas. **À retenir** : le violet fintech courant est saturé et nocturne ; Liasse se distingue par un violet sombre sur crème. Même constat sur « fintech landing page » : la majorité des vignettes populaires sont sombres. |

---

## Mobile (observé)

Captures en 390 × 844 px, le 2026-11-12. Hauteurs mesurées dans la page.

| Site | Capture | Ce qu'on observe |
|---|---|---|
| Indy, page artisans | [capture](captures/mobile-indy-artisan.jpg) | Titre, 4 coches, puis 2 boutons pleine largeur de 48 px (« Démarrer », « Prendre rendez-vous »). La photo et la carte « Payée » n'arrivent qu'en bas de l'écran. Pas de capture d'app ni de champ e-mail au premier écran. |
| Pennylane, facturation électronique | [capture](captures/mobile-pennylane.jpg) | Onglets de cible tronqués en haut, titre centré, 3 coches, un bouton de 229 × 50 px. L'image du produit commence sous la ligne de flottaison. |
| Mercury | [capture](captures/mobile-mercury.jpg) | Champ e-mail pleine largeur, puis « Open account » et « Launch demo » côte à côte. Le champ fait 38 px de haut et les boutons 40 px, sous les 44 px. Le champ a `type="email"` et `autocomplete="email"`, mais pas de label visible (seulement un texte indicatif). La mention « not an FDIC-insured bank » reste visible en bas. |

**Ce que ça change** :
- Aucun des 3 sites ne montre l'app au premier écran mobile. La consigne du brief (« capture mobile en premier ») n'a donc pas de modèle direct : la placer juste sous le champ e-mail, en la laissant dépasser du premier écran pour inviter au défilement, plutôt qu'au-dessus du titre.
- Le schéma de Mercury (champ pleine largeur puis bouton) confirme le composant prévu. Mais il faut faire mieux sur 2 points mesurés : 48 px minimum pour le champ et le bouton, et un label visible.
- Un seul bouton sous le champ en mobile. Mercury en met deux, qui se partagent la largeur et deviennent trop petits.

---

## Synthèse du moodboard

**Ajustements du 2026-11-12, et pourquoi** : les références des directions ont été remplacées quand elles n'avaient pas pu être vues (n° 5, 11) ou quand la capture contredisait la description (n° 7, 8, 9). Deux observations changent le fond : Indy occupe déjà le registre « crème, artisan, carte Payée » (n° 16), et Ledgerly (n° 22) montre que la trésorerie à 90 jours se raconte très bien en une phrase. La direction A reste recommandée, avec un garde-fou.

### Direction A : « Carnet chaleureux » (recommandée)
- Fond crème, cartes blanc cassé, violet profond pour le texte et les boutons, corail pour un seul signal (facture payée, point de l'échéancier).
- **Garde-fou** : le crème seul ne distingue pas Liasse d'Indy (`#FEF7EC`, très proche de `#FBF6EE`). La différence doit venir du violet profond (absent chez Indy, rose `#FA5D89`), de vraies captures de l'app plutôt qu'une photo d'artisan avec cartes flottantes, et de la trésorerie à 90 jours, qu'Indy ne montre pas.
- Captures mobiles en grand, légèrement inclinées, avec ombres douces. Les montants s'animent au passage (refs 3, 22, 24).
- Registre : rassurant et humain, adapté à des artisans.

### Direction B : « Calendrier clair »
- L'échéancier devient la colonne vertébrale du site : on scrolle dans le temps (aujourd'hui, réception, émission 2027), et chaque étape révèle une fonctionnalité (refs 6, 23, 25).
- Typo DM Sans grasse, frise violette, jalons en corail.
- Registre : pédagogique, fort pour le SEO réforme. Risque : se démoder après 2027.

### Direction C : « Tableau de bord doux »
- Hero centré sur la courbe de trésorerie à 90 jours (refs 3, 22), avec des widgets arrondis et des chiffres tabulaires grands formats. Une phrase sous la courbe dit ce qu'elle signifie (« Point bas le 1er décembre : vous restez au-dessus de votre seuil »).
- Plus de violet clair en surfaces, moins de crème.
- Registre : pilotage, plus adapté aux TPE de services qu'aux artisans du bâtiment.

### Palette recommandée

Inchangée : aucune observation ne justifie de changer une couleur. Les contrastes « à vérifier » ont été calculés (WCAG 2.1).

| Rôle | Hex | Contraste mesuré |
|---|---|---|
| Crème (fond) | `#FBF6EE` | |
| Crème profond (surfaces) | `#F3EADB` | |
| Violet profond (marque, texte) | `#2E1A5C` | 13,76:1 sur crème ; blanc sur violet 14,80:1 |
| Violet clair (surfaces d'accent) | `#ECE4FA` | violet profond dessus : 12,02:1 |
| Corail (accent) | `#FF6F59` | 2,54:1 sur crème : jamais pour du texte (confirmé) |
| Corail foncé (texte d'accent) | `#B8412E` | 5,09:1 sur crème, 5,48:1 sur blanc, 4,59:1 sur `#F3EADB` : AA validé |
| Encre neutre | `#1F1A2B` | 15,73:1 sur crème |

### Polices (Google Fonts)

**Correction du 2026-11-12** : test fait dans le navigateur avec les polices servies par Google Fonts. Avec DM Sans (version statique et version variable), « 111111 » et « 000000 » gardent des largeurs différentes même avec `font-variant-numeric: tabular-nums` : DM Sans n'a pas de chiffres tabulaires sur Google Fonts. Outfit 600 les a (largeurs égales avec `tabular-nums`, différentes sans). DM Mono est à chasse fixe.

- **DM Sans** pour les titres (700) et le texte (400).
- **Montants** : **Outfit 600** avec `font-variant-numeric: tabular-nums`. Elle reste dans la famille des grotesques arrondies du brief. DM Mono en solution de repli, pour les tableaux uniquement.
- **Alternative titres** : Outfit (600 et 700), ce qui ferait d'Outfit la police unique du site.

### 3 « à ne pas faire »
1. Pas de dégradé violet-noir futuriste ni de glassmorphisme (refs 20, 26) : c'est le code crypto et néobanque, pas celui de l'artisan.
2. Pas de corail pour le texte sur fond crème (2,54:1), ni pour les alertes de réforme : le corail signale une bonne nouvelle (« payé »), jamais une menace. Pennylane écrit « Évitez les amendes » (ref 6) : Liasse ne le fera pas.
3. Pas de tableau de bord de DAF en hero (graphiques denses, jargon) : une seule courbe, trois montants, une phrase.

---

## Design tokens (proposition)

### Couleurs

| Token | Hex | Usage |
|---|---|---|
| `color.brand.primary` | `#2E1A5C` | Boutons primaires, titres |
| `color.brand.primary-hover` | `#432A80` | Survol (texte blanc : 11,16:1) |
| `color.brand.primary-soft` | `#ECE4FA` | Surfaces d'accent, badges |
| `color.brand.accent` | `#FF6F59` | Signal « payé », jalon actif, pastilles. Pas de texte sur crème |
| `color.brand.accent-text` | `#B8412E` | Texte d'accent si nécessaire (5,09:1 sur crème) |
| `color.success.text` | `#17704A` | Validation, « Facture payée » en texte (5,35:1 sur `success.bg`) |
| `color.success.bg` | `#E5F4EC` | Fond des messages de succès |
| `color.error.text` | `#B42318` | Erreurs de formulaire (5,75:1 sur `error.bg`) |
| `color.error.bg` | `#FDECEA` | Fond des messages d'erreur |
| `color.warning.text` | `#9A5B00` | Échéance proche, avertissements (4,94:1 sur `warning.bg`) |
| `color.warning.bg` | `#FFF3DC` | Fond des avertissements |
| `color.neutral.0` | `#FFFFFF` | Champs |
| `color.neutral.50` | `#FBF6EE` | Fond de page (crème) |
| `color.neutral.100` | `#F3EADB` | Surfaces, cartes |
| `color.neutral.200` | `#E3D8C6` | Bordures décoratives uniquement (1,31:1 sur crème) |
| `color.neutral.500` | `#7A7186` | Texte désactivé et bordure des champs (4,31:1 sur crème, 4,63:1 sur blanc) |
| `color.neutral.700` | `#544B63` | Texte secondaire (7,61:1 sur crème) |
| `color.neutral.900` | `#1F1A2B` | Texte principal |

Contrastes calculés le 2026-11-12 (formule WCAG 2.1). `neutral.500` reste sous 4,5:1 sur crème : réservé au texte désactivé, jamais à un texte utile. La bordure d'un champ doit atteindre 3:1 (critère 1.4.11) : `neutral.200` ne suffit pas, d'où `neutral.500` pour les champs.

### Typographie
`font.sans` = DM Sans, `font.display` (optionnel) = Outfit, `font.numeric` = **Outfit 600 avec `tabular-nums`** (DM Sans n'a pas de chiffres tabulaires sur Google Fonts, voir plus haut), repli DM Mono.

| Token | Taille desktop / mobile | Graisse | Interligne | Usage |
|---|---|---|---|---|
| `type.display` | 60 / 38 px | 700 | 1.08 | Titre du hero |
| `type.h2` | 38 / 28 px | 700 | 1.15 | Titres de section |
| `type.h3` | 22 / 20 px | 600 | 1.3 | Cartes |
| `type.body-lg` | 20 / 18 px | 400 | 1.5 | Sous-titre |
| `type.body` | 17 / 16 px | 400 | 1.6 | Texte courant |
| `type.small` | 14 px | 500 | 1.45 | Mentions, conditions de l'essai |
| `type.amount-xl` | 48 / 36 px | 600 | 1.0 | Montants héros (trésorerie), en `font.numeric` |
| `type.amount` | 18 / 16 px | 600 | 1.2 | Montants dans les mockups et tableaux, en `font.numeric` |

### Espacement (base 4 px)
`space.1` = 4, `space.2` = 8, `space.3` = 12, `space.4` = 16, `space.5` = 20, `space.6` = 24, `space.8` = 32, `space.12` = 48, `space.16` = 64, `space.24` = 96, `space.30` = 120 px.
Sections : 120 px en desktop, 64 px en mobile. Gouttière latérale de 16 px en mobile. Conteneur de 1160 px.

### Rayons
`radius.sm` = 8 px (champs, pastilles), `radius.md` = 14 px (boutons, cartes), `radius.lg` = 24 px (mockups, blocs mis en avant), `radius.full` = 999 px (badges, bouton du champ e-mail en mobile).
Rayons généreux, cohérents avec une grotesque arrondie.

### Ombres
`shadow.sm` = `0 1px 3px rgba(46,26,92,.08)` ; `shadow.md` = `0 10px 30px rgba(46,26,92,.10)` (cartes mises en avant) ; `shadow.device` = `0 30px 60px -20px rgba(46,26,92,.25)` (mockups) ; `shadow.focus` = `0 0 0 3px rgba(46,26,92,.4)`.

### Motion

| Token | Valeur | Usage |
|---|---|---|
| `motion.duration.fast` | 120 ms | Survol, focus |
| `motion.duration.base` | 220 ms | Accordéons (FAQ), sélecteur de profil |
| `motion.duration.amount` | 600 ms | Montant qui s'incrémente (une seule fois, à l'entrée dans l'écran) |
| `motion.duration.draw` | 900 ms | Tracé de la courbe de trésorerie |
| `motion.ease.standard` | `cubic-bezier(.2,0,0,1)` | Défaut |
| `motion.ease.out-soft` | `cubic-bezier(.16,1,.3,1)` | Montants, courbe |

Avec `prefers-reduced-motion: reduce`, les montants s'affichent directement à leur valeur finale et la courbe est statique.

### Composants clés

**Bouton primaire** : fond `brand.primary`, texte blanc, `radius.md`, hauteur 52 px (48 px minimum en mobile).
États : repos ; survol (`brand.primary-hover`) ; focus (`shadow.focus`) ; actif (légèrement assombri) ; désactivé (`neutral.200` et `neutral.500`) ; chargement (« Création du compte… », bouton bloqué).

**Bouton secondaire** : fond transparent, bordure 1,5 px `brand.primary`, texte `brand.primary`. Survol : fond `brand.primary-soft`.

**Champ e-mail et bouton (hero)** : en desktop, champ et bouton sur une ligne. En mobile, champ pleine largeur puis **un seul** bouton pleine largeur, 48 px de haut minimum pour les deux (Mercury, mesuré à 38 et 40 px, est trop petit). Label visible (« Votre e-mail professionnel »), pas seulement un texte indicatif. `type="email"`, `autocomplete="email"`, `inputmode="email"`. Bordure du champ en `neutral.500`. Sous le bouton : les conditions de l'essai, puis « Liasse n'est pas une banque » si la connexion bancaire est citée au-dessus (modèle : Mercury, n° 1).

**Carte** (fonctionnalité, formule, avis) : fond `neutral.0` ou `neutral.100`, `radius.md`, padding `space.6`. La formule recommandée a une bordure de 2 px `brand.primary` et un badge `brand.primary-soft`. Chaque prix porte « HT » juste dessous (modèle : n° 21).

**Formulaire** : erreur sous le champ (`error.text`, icône, `aria-describedby`, `aria-invalid`). Succès dans un bloc `success.bg` qui remplace le formulaire et prend le focus.

| À faire | À ne pas faire |
|---|---|
| Un seul champ (e-mail) pour l'inscription | Nom, téléphone et SIRET dès l'inscription |
| Conditions de l'essai écrites sous le bouton | Conditions cachées dans les CGU |
| Montants en chiffres tabulaires (Outfit), animés une fois | Compteurs qui tournent en boucle |
| Corail pour les bonnes nouvelles (payé, jalon atteint) | Corail ou rouge pour faire peur avec la réforme |
| Cibles tactiles d'au moins 44 px, focus visible | `outline: none` ou liens de 12 px en pied de page |
| Captures d'application réelles et à jour | Mockups génériques sans lien avec le produit |
| Échéancier lisible sans la couleur (texte et icônes) | Frise uniquement codée par couleur |
| Un même chiffre d'utilisateurs partout, daté | Deux chiffres sur la même page (Qonto, Pennylane) |
| Numéro d'immatriculation PA affiché à côté de la mention | « Plateforme agréée » sans numéro (Qonto, Pennylane) |
