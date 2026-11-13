# Benchmark visuel : Liasse (fintech et SaaS de gestion, entreprise fictive)

Ce bench suit le brief bloc par bloc : chaque référence retenue sert un bloc de l'arborescence ou une contrainte du [brief client](BRIEF-CLIENT.md).

## Limites, à lire en premier

**Passe du 2026-11-13** : Liasse est fictive et personne ne validera rien. Les anciens points ouverts deviennent des décisions (section **Arbitrages**, en fin de document). Le brief ne contient plus aucun chiffre propre à Liasse : plus de taille d'équipe, d'utilisateurs, de cibles de KPI, de budget, de note d'avis ni de durée promise (« 2 minutes »). Le bloc d'avis est retiré du one-page. Les chiffres observés sur les pages du bench restent, avec leur URL. Le brief ne demande aucune photo d'équipe : rien à chercher en banque d'images.

**Refonte du 2026-11-12 (cette version)** :
- Les 26 références d'origine ont été triées : **12 inspirations** et **14 à côté**. Avec les 2 ajouts, le bench compte **14 inspirations**. Rien n'a été supprimé : chaque référence à côté garde sa ligne et sa raison, en fin de document.
- Les captures sont rangées dans [`captures/inspis/`](captures/inspis/) et [`captures/a-cote/`](captures/a-cote/), sans renommage. Le préfixe reste le numéro de la référence. Les numéros n'ont pas changé.
- Le bench est réorganisé selon les 8 blocs du one-page du brief (section 6), dans le même ordre.
- **2 références ajoutées**, ouvertes et capturées le 2026-11-12 : n° 27 (Billow) pour le sélecteur de profil de l'échéancier et la FAQ, n° 28 (Statements) pour le comparatif des tarifs. Une recherche pour le bloc Sécurité n'a rien donné : sur Dribbble, les fiches affichent maintenant un challenge anti-robots (« Let's confirm you are human »), non contourné.
- **Valeurs corrigées** (voir « Palette, polices, design tokens ») : `shadow.focus` passait à 2,37:1 sur crème, sous le seuil de 3:1 ; le corail en pastille porteuse de sens est à 2,54:1, sous 3:1 pour un élément graphique ; `color.brand.accent-text` sur `primary-soft` est à 4,45:1, sous 4,5:1.
- **Directions** : la direction B « Calendrier clair » est retirée (elle fait de la réforme la colonne du site, alors que le brief demande de gagner sur la trésorerie, les relances et le ton artisan). La direction C garde le crème en fond de page.

**Vérification du 2026-11-12 (version précédente, toujours valable)**, faite avec un vrai navigateur (Chrome piloté par Playwright) :
- **Ce qui a été vu** : 14 des 20 références d'origine. 10 par leur URL d'origine (n° 1, 2, 3, 6, 7, 8, 9, 15, 16, 17), 4 par une page équivalente sur le même sujet, parce que l'URL d'origine est bloquée (n° 13, 14, 18, 20). Captures en 1440 × 900 px, au-dessus de la ligne de flottaison, parfois avec une seconde capture ciblée. Les couleurs et les polices citées ont été relevées dans la page (`getComputedStyle`). Les chiffres cités sont ceux affichés le 2026-11-12.
- **Ce qui reste bloqué** : Behance (n° 4 et 12, erreur HTTP 400) ; Abby (n° 5, erreur 403 CloudFront, deux essais à une heure d'écart) ; Godly (n° 10 et 11, redirection vers recent.design ; le site de Revolut affiche un challenge Cloudflare, non contourné) ; Lapa Ninja (n° 13) et Land-book (n° 14), Cloudflare ; Pinterest (n° 18, 19, 20), mur de connexion, aucune capture.
- **Remplacements** : n° 21 à 26, tous ouverts et capturés. Ils remplacent les n° 4, 10, 11, 12 et 19, et complètent les tarifs.
- **Corrections importantes** :
  - Qonto (n° 2) n'affiche **aucun numéro d'immatriculation de plateforme agréée** sur les 3 pages ouvertes. Le seul numéro visible est celui d'établissement de paiement (ACPR, CIB 16958). Pennylane non plus, mais il montre le logo officiel « Plateforme agréée ».
  - Mercury (n° 1) n'a ni « beaucoup de blanc » ni « un seul bouton » : photo pleine page, champ e-mail puis deux boutons.
  - Les palettes Dribbble (n° 7, 8) sont extraites automatiquement de l'image, pas choisies par le designer. La n° 8 est grise, pas « chaude ».
  - Acctual (n° 13) ne réunit pas factures émises et reçues sur une page. Maze (n° 14) n'affiche plus aucun prix.
  - **DM Sans, servie par Google Fonts, n'a pas de chiffres tabulaires** : `font-variant-numeric: tabular-nums` ne change rien (test fait dans le navigateur). Outfit les a.
  - Indy (n° 16), concurrent direct sur les artisans, a déjà un hero crème `#FEF7EC`, une photo d'artisan et une carte « Facture électronique · Payée ».
- **Mobile** : 3 sites capturés en 390 × 844 px (Indy, Pennylane, Mercury).
- **Bannières cookies** : refusées partout où un refus existait. Sur Maze, préférences enregistrées sans rien cocher. Sur SaaS Landing Page et Hangar, le bandeau n'offre que « I agree » ou « Accept » : il a été masqué pour la capture, rien n'a été accepté. Billow et Statements (ajouts) n'affichaient pas de bandeau.
- Les ajouts n° 27 et 28 n'ont pas eu de relevé `getComputedStyle` des couleurs : seuls le texte, la structure et les polices annoncées par One Page Love sont cités.

---

## Couverture du brief

| Exigence du brief | Inspirations | Manque |
|---|---|---|
| 1. Hero : titre, champ e-mail, « Essai gratuit 30 jours », capture mobile en premier sur téléphone | 1, 3, 13, 27 | Aucune référence ne montre l'app au premier écran mobile (voir « Mobile »). |
| 2. Échéancier de la réforme : frise 2026-2027, sélecteur « Je suis », « Ce que vous devez faire » | 6, 27, 23 | Aucune référence ne réunit frise et sélecteur de profil. Abby (n° 5), qui le faisait peut-être, n'a pas pu être vu. |
| 3. Fonctionnalités : facture, relance, trésorerie, export comptable (4 cartes) | 8, 23, 22, 28, 3 | Pas de grille de 4 cartes sur ces 4 sujets précis : chaque carte a son modèle, la grille vient du n° 3. |
| 4. Aperçu de l'application : captures mobile et desktop, micro-animations sur les montants | 22, 24, 25, 27 | Aucune micro-animation de montant constatée (non vue chez Mercury, captures fixes ailleurs). À prototyper. |
| 5. Pour les experts-comptables : bénéfices, export, invitation des clients, contact partenaire | 2, 28, 6 | Pas de bande de logos : le brief n'en veut pas (compatibilité fictive), les formats d'export suffisent. |
| 6. Sécurité : plateforme agréée, hébergement, chiffrement, données bancaires | 1, 2, 6 | Aucune référence ne nomme l'hébergeur, la région, le chiffrement ni l'agrégateur bancaire. Le seul exemple vu est vague (n° 27, à éviter). |
| 7. Tarifs : 2 formules HT et TTC, prix de démonstration calés sur une grille publique, comparatif par catégories sans nom de concurrent | 21, 28 | Aucune grille ne montre HT et TTC côte à côte : le n° 21 n'affiche que le HT. |
| 8. FAQ et inscription : FAQ de 8 à 10 questions, champ e-mail répété | 27 | Le bloc d'avis est retiré du brief (voir Arbitrages). Les n° 16 et 2 restent comme repères de ce que font les concurrents. |
| Mobile : capture d'app en premier, inscription en un champ et un tap, cibles de 44 px | 16, 1, 6 | Voir bloc 1. Mercury (n° 1) est sous 44 px. |
| Marque : crème, violet profond, accent corail | 22, 16, 25 | Aucun violet profond sur crème observé (la n° 26, à côté, montre que le violet fintech courant est électrique et sombre). |
| Marque : grotesque arrondie (DM Sans ou Outfit), chiffres tabulaires | 24 | Les chiffres tabulaires viennent d'un test navigateur, pas d'une référence (voir « Polices »). |
| Accessibilité : AA, corail jamais en texte sur crème, frise lisible sans couleur | 6, 22 | Plusieurs contre-exemples mesurés (n° 16, 21, 1) cités dans les blocs. |
| Preuve « Une facture conforme depuis votre téléphone, sans repasser au bureau » | 8, 27 | Pas de boucle mobile du parcours observée. Le n° 27 se contredit sur la durée : une raison de plus pour ne promettre aucune durée. |
| Preuve « Prêt pour l'émission de septembre 2027 » | 6 | Aucun numéro d'immatriculation PA affiché nulle part (n° 2 et 6). |
| Preuve « Les relances partent toutes seules » | 23 | La séquence de relances du n° 23 suffit : le brief n'affiche aucun délai moyen de paiement, Liasse n'en a pas. |
| Preuve « Votre trésorerie à 90 jours, en un coup d'œil » | 22, 24, 3 | Animation des montants non observée. |
| Preuve « Votre expert-comptable branché directement » | 2, 28 | Formats d'export écrits en clair (n° 28). Pas de logos de logiciels tiers : une compatibilité affichée par une entreprise fictive serait fausse. |
| Preuve « Vos données sont protégées » | 1, 2 | Région d'hébergement et statut du prestataire de connexion bancaire jamais écrits. |

---

## Inspirations, bloc par bloc

### 1. Hero

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 1 | [Mercury](https://mercury.com/), via [SaaS Landing Page](https://saaslandingpage.com/mercury/) (fiche d'octobre 2026, site US) | [site](captures/inspis/01-mercury-site.jpg), [fiche](captures/inspis/01-mercury-slp.jpg) | Sous le titre, un champ « Enter your email » puis le bouton « Open account » (`#5266EB`, texte blanc à 4,71:1, rayon 32 px). La mention « Mercury is a fintech company, not an FDIC-insured bank » reste épinglée en bas du hero. À éviter : la photo d'ambiance pleine page sans produit, et le second bouton « Launch demo ». | Champ e-mail du hero ; « Ne pas laisser entendre que Liasse est une banque » |
| 3 | [Finpay, Fintech Landing Page](https://dribbble.com/shots/24820686-Finpay-Fintech-Landing-Page) (Dipa Inhouse, Dribbble) | [vignette](captures/inspis/03-dribbble-finpay.jpg) | Maquette claire, un seul champ (« Your business email ») et « Get Started » sous le titre. | Inscription en un champ et un tap |
| 13 | [Acctual](https://www.acctual.com/) (fiche Lapa Ninja bloquée) | [capture](captures/inspis/13-acctual.jpg) | Les conditions chiffrées écrites juste sous le bouton « Send my first invoice » (carte 2,7 %, virement 1 %, stablecoin 1 %). Fond `#F7FAFC`, titre Open Runde 600 de 64 px. | Conditions de l'essai écrites à côté du bouton |
| 27 | [Billow](https://www.billow.so/), via [One Page Love](https://onepagelove.com/billow) (ajout) | [hero](captures/inspis/27-billow.jpg) | « 14-day free trial · Cancel anytime. » en une ligne sous « Start your trial », répété à l'identique au CTA de fin de page. Juste sous le hero, le produit à manipuler (« Go on, play with it ;-) »). À éviter : le halo bleu en dégradé. | « Sans carte bancaire. Sans engagement. » sous le bouton ; CTA répété en pied de page |

Détail d'une référence à côté : l'aperçu mobile de Tara (n° 9) met le champ et « Join waitlist » sur une seule ligne. Même principe que les n° 1 et 3.

### 2. Échéancier de la réforme

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 6 | [Pennylane, logiciel de facturation électronique](https://www.pennylane.com/fr/logiciel-facturation-electronique?so=1) (France) | [échéancier](captures/inspis/06-pennylane-echeancier.jpg), [hero](captures/inspis/06-pennylane.jpg) | 3 cartes dont la date est le titre : « 1er septembre 2026 » (réception), « 1er septembre 2027 » (émission des PME, TPE et micro-entreprises), « Dès aujourd'hui ». Lisible sans couleur. En haut de page, une entrée par cible en onglets (« Indépendants et TPE », « PME et ETI », « Cabinet expertise comptable »). À éviter : « Évitez les amendes » dans la 3e carte ; l'onglet du navigateur qui dit encore « préparez-vous pour 2026 ». | Frise 2026-2027 lisible sans couleur ; contenu réforme daté ; ton sans peur |
| 27 | [Billow](https://www.billow.so/) (ajout) | [profils](captures/inspis/27-billow-profils.jpg) | 5 pastilles de profil (« Freelancers », « Studios », « Agencies », « Creators », « Consultants ») au-dessus d'un seul bloc. Un clic sur « Studios » remplace le titre du bloc par « Small team, big clarity. », sans changer de page. | Sélecteur « Je suis : artisan, commerçant, profession libérale, société » qui affiche « Ce que vous devez faire » |
| 23 | [Automatic invoice reminder sequence, DueCourse](https://dribbble.com/shots/6882240-Automatic-invoice-reminder-sequence-DueCourse) (Paul Haydock, Dribbble) | [capture](captures/inspis/23-dribbble-duecourse-relances.jpg) | Une ligne de temps qui place des étapes avant, le jour même et après une date pivot, chacune avec un libellé écrit. | Mise en page de la frise : aujourd'hui, septembre 2026, septembre 2027 sur un même axe |

### 3. Fonctionnalités (4 cartes)

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 8 | [Invoicing tool, iOS Mobile app](https://dribbble.com/shots/15711855-Invoicing-tool-iOS-Mobile-app) (Vishal Reddy, Dribbble) | [capture](captures/inspis/08-dribbble-invoicing-ios.jpg) | Choix de l'envoi en bas d'écran : « Email » ou « Text Message », puis « Send invoice ». Le texte décrit un flux en 2 temps (ce qui change à chaque facture, puis les réglages). Palette grise extraite automatiquement : rien à reprendre côté couleur. | Carte « facture » ; envoi par SMS aux clients particuliers (Mehdi) |
| 23 | DueCourse (voir bloc 2) | [capture](captures/inspis/23-dribbble-duecourse-relances.jpg) | 4 relances sur une ligne de temps, chacune avec son délai (« 3 days before invoice is due ») et son objet réel (« Your invoice is due in 3 days »). À éviter : le fond bois et le style daté. | Carte « relance » ; message « Payé plus vite » |
| 22 | [Ledgerly, Invoicing App Website & Product UI](https://dribbble.com/shots/27843787-Ledgerly-Invoicing-App-Website-Product-UI) (Nazar Deynega, Dribbble) | [vignette](captures/inspis/22-dribbble-ledgerly.jpg) | Écran « Forecast » avec 30 j, 90 j et 6 mois, « Projected balance €51,300 », et une phrase qui traduit la courbe : « Lowest point Dec 1: €35,200. You stay above your €20k safety line. » | Carte « trésorerie » |
| 28 | [Statements](https://statements.now/), via [One Page Love](https://onepagelove.com/statements) (ajout) | [comparatif](captures/inspis/28-statements-comparatif.jpg) | Carte « Export » : « Download a clean CSV that is ready for Excel, Xero, and downstream tools ». Le format et les logiciels de destination sont écrits dans la carte. | Carte « export comptable » |
| 3 | Finpay (voir bloc 1) | [bloc courbe](captures/inspis/03-dribbble-finpay-bento.jpg) | Une grille de blocs de tailles différentes, dont une carte « Summary $1,876,580 » avec une courbe sur 6 mois. | Grille des 4 cartes, la trésorerie en plus grand |

### 4. Aperçu de l'application

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 22 | Ledgerly (voir bloc 3) | [section 90 jours](captures/inspis/22-dribbble-ledgerly-forecast.jpg), [vignette](captures/inspis/22-dribbble-ledgerly.jpg) | Le concept le plus proche de Liasse (« invoicing and cash-flow app », objectif essai gratuit). Section « 90 days ahead, at a glance » : courbe de solde, point bas signalé (« still safe »), 4 montants (« Cash in bank », « Outstanding », « Overdue », « Safe to spend »), statuts écrits (« Paid », « Pending », « Overdue »). Corail `#FE1D07`, surfaces crème `#F6F5F0`. Vignette : un téléphone tenu en main. À éviter : le corail pour « Overdue » (Liasse le garde pour « payé ») ; le tableau de bord complet en hero. | Captures mobile et desktop ; aperçu de la courbe à 90 jours ; statuts lisibles sans couleur |
| 24 | [Depo Budget App](https://onepagelove.com/depo-budget-app) (One Page Love, 13 août 2026) | [capture](captures/inspis/24-onepagelove-depo.jpg) | Un téléphone au premier plan, un seul montant (71 $, ce qu'on peut dépenser aujourd'hui), « No spreadsheet. », puis 4 cartes numérotées avec un montant chacune. À éviter : le style brutaliste bleu et jaune fluo. | Montants mis en scène, support des micro-animations |
| 25 | [invoicemon](https://onepagelove.com/invoicemon) (One Page Love, 17 juin 2026) | [capture](captures/inspis/25-onepagelove-invoicemon.jpg) | Démo qui se déroule au scroll et montre l'éditeur de facture réel. Un seul bouton « Create an invoice » (`#1A1816`, texte `#FDFCF8`). Couleurs « Beige, Earth Tones », police Inter. | CTA « Voir l'application en 30 secondes » ; captures réelles et à jour |
| 27 | Billow (voir bloc 1) | [hero](captures/inspis/27-billow.jpg) | Sous le hero, un tableau de bord à manipuler : « Open Invoices », une ligne « 3d Overdue » avec un bouton « Reminder », une ligne « Awaiting Payment ». | Aperçu desktop ; la relance visible dans l'app |

### 5. Pour les experts-comptables

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 2 | [Qonto, page experts-comptables](https://qonto.com/fr/accountants/for-your-clients) et [accueil](https://qonto.com/fr?tp=1) (France) | [experts-comptables](captures/inspis/02-qonto-experts-comptables.jpg), [accueil](captures/inspis/02-qonto.jpg) | Fond blanc, titre noir de 56 px, 4 coches, bouton « Parler à un conseiller » (`#050505`, rayon 8 px), capture de l'app avec « Mon comptable · Synchronisé ». Le texte explique l'invitation des clients « en un clic ». À éviter : « 600 000 entreprises » sur cette page contre « 750 000 » sur l'accueil. | Bénéfices, invitation des clients, contact partenaire (« Devenir cabinet partenaire ») |
| 28 | Statements (voir bloc 3) | [comparatif](captures/inspis/28-statements-comparatif.jpg) | Les logiciels de destination nommés en toutes lettres (« Excel, Xero ») dans l'étape d'export. | Formats d'export |
| 6 | Pennylane (voir bloc 2) | [hero](captures/inspis/06-pennylane.jpg) | Un onglet « Cabinet expertise comptable » dès le haut de la page. | Accès direct à la section depuis le haut de page |

### 6. Sécurité

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 1 | Mercury (voir bloc 1) | [site](captures/inspis/01-mercury-site.jpg) | « Mercury is a fintech company, not an FDIC-insured bank », épinglé en bas du hero et encore visible en mobile. | « Ne pas laisser entendre que Liasse est une banque » |
| 2 | Qonto, accueil (voir bloc 5) | [accueil](captures/inspis/02-qonto.jpg) | Pied de page avec les numéros réglementaires écrits : ACPR (CIB 16958), ORIAS, RCS. À éviter : « Certifié Plateforme Agréée » sans numéro d'immatriculation PA (aucun sur les 3 pages ouvertes). | Statut réglementaire du prestataire écrit en clair |
| 6 | Pennylane (voir bloc 2) | [hero](captures/inspis/06-pennylane.jpg) | Le logo officiel « Plateforme agréée · Facturation électronique · République française » dans l'image du hero. À éviter : pas de numéro à côté. | Mention « plateforme agréée ». Liasse l'écrit dans le texte, sans ce logo officiel ni numéro (voir Arbitrages) |

À éviter : à « Is my data secure? », Billow (n° 27) répond seulement « Billow uses encryption and secure cloud infrastructure ». Le brief demande la région d'hébergement, le chiffrement et le statut du prestataire bancaire écrits en clair.

### 7. Tarifs

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 21 | [Pennylane, tarifs de la page facturation électronique](https://www.pennylane.com/fr/logiciel-facturation-electronique?so=1) (France) | [capture](captures/inspis/21-pennylane-tarifs.jpg) | 3 cartes « À partir de » 7, 14 et 24 € « /mois HT », celle du milieu en fond sombre. Une ligne par formule, le même bouton « Essayer gratuitement » partout, et sous la grille : « 15 jours d'essai gratuit, sans engagement. ». À éviter : les prix en vert `#00BD57` sur blanc, à 2,5:1. | 2 formules ; HT lisible ; conditions de l'essai écrites ; grille publique sur laquelle sont calés les prix de démonstration de Liasse (7 et 14 € HT, rouverte le 2026-11-13) |
| 28 | Statements (voir bloc 3) | [comparatif](captures/inspis/28-statements-comparatif.jpg) | Tableau « How it compares » : colonnes « statements », « AI », « Others », « Manual », 7 lignes de critères, la colonne du produit encadrée. Les autres sont des catégories, jamais des marques. À éviter : des cellules à icône seule (coche ou croix) sans texte accessible, constaté dans le code de la page ; le fond sombre. | Comparatif « Liasse et les autres » factuel, sans nommer de concurrent |

Détail d'une référence à côté : chez Bonsai (n° 15), le badge noir « Most popular » sur la formule mise en avant reste sobre.

### 8. FAQ et inscription

Le bloc d'avis est retiré du brief : une entreprise fictive n'a ni note ni verbatims. Les n° 16 et 2 restent comme repères de ce que font les concurrents, pas comme modèles à reproduire.

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 16 | [Indy, page artisans](https://www.indy.fr/artisan/) (France, concurrent direct) | [capture](captures/inspis/16-indy-artisan.jpg) | 3 notes avec leur source et leur volume : Trustpilot 4,8 et +16 000 avis, App Store 4,9, Play Store 4,8. Pastille « + de 10 000 Artisans déjà clients ! ». À éviter : le bouton rose `#FA5D89` à texte blanc (3,0:1) ; « A partir de 12 € /mois » dans le hero puis « Un socle gratuit avec tous les essentiels » plus bas. | Repère concurrent : notes sourcées (pas d'avis chez Liasse) |
| 27 | Billow (voir bloc 1) | [FAQ](captures/inspis/27-billow-faq.jpg) | FAQ en accordéon de 8 questions, dont « How does the 14-day trial work? » et « Is my data secure? ». Le CTA de fin de page reprend celui du hero avec ses conditions. À éviter : 3 durées pour la même promesse (« in under 5 minutes », « in under 2 minutes », « in under a minute ») ; une FAQ qui parle encore d'« upcoming launch » et de liste d'attente alors que l'essai est ouvert. | FAQ de 8 à 10 questions ; inscription répétée ; dates et chiffres cohérents d'une section à l'autre |
| 2 | Qonto, accueil (voir bloc 5) | [accueil](captures/inspis/02-qonto.jpg) | « 4,7 sur 5 » Trustpilot près du hero, avec la source nommée. | Repère concurrent (pas d'avis chez Liasse) |

---

## Mobile

Captures en 390 × 844 px, le 2026-11-12. Hauteurs mesurées dans la page. Exigences du brief concernées : capture mobile en premier (bloc 1), inscription en un champ et un tap (critères de réussite), part des inscriptions faites sur mobile (indicateur suivi), cibles tactiles de 44 px (accessibilité), LCP mobile sous 2,5 s.

| # | Site | Capture | Ce qu'on observe | Exigence du brief |
|---|---|---|---|---|
| 16 | Indy, page artisans | [capture](captures/inspis/mobile-indy-artisan.jpg) | Titre, 4 coches, puis 2 boutons pleine largeur de 48 px (« Démarrer », « Prendre rendez-vous »). La photo et la carte « Payée » n'arrivent qu'en bas de l'écran. Pas de capture d'app ni de champ e-mail au premier écran. | Cibles de 44 px : respecté |
| 6 | Pennylane, facturation électronique | [capture](captures/inspis/mobile-pennylane.jpg) | Onglets de cible tronqués en haut, titre centré, 3 coches, un bouton de 229 × 50 px. L'image du produit commence sous la ligne de flottaison. | Sélecteur de profil : des onglets tronqués ne marchent pas en 390 px |
| 1 | Mercury | [capture](captures/inspis/mobile-mercury.jpg) | Champ e-mail pleine largeur, puis « Open account » et « Launch demo » côte à côte. Le champ fait 38 px de haut et les boutons 40 px. Le champ a `type="email"` et `autocomplete="email"`, mais pas de label visible. La mention « not an FDIC-insured bank » reste visible en bas. | Inscription en un champ : bon schéma, mais sous 44 px et sans label |

**Ce que ça change** :
- Aucun des 3 sites ne montre l'app au premier écran mobile. La consigne du brief (« capture mobile en premier ») n'a pas de modèle direct : la placer juste sous le champ e-mail, en la laissant dépasser du premier écran pour inviter au défilement.
- Le schéma de Mercury (champ pleine largeur puis bouton) confirme le composant prévu, avec 48 px minimum pour le champ et le bouton, et un label visible.
- Un seul bouton sous le champ en mobile. Mercury en met deux, qui se partagent la largeur et deviennent trop petits.
- Le sélecteur « Je suis » doit passer à la ligne ou devenir une liste en mobile : les onglets de Pennylane sont coupés à 390 px. Les pastilles de Billow (n° 27) n'ont pas été vues en mobile.

---

## Directions

Le brief ne fixe pas de nombre de pistes. 2 pistes sont gardées, toutes deux sur la palette crème, violet profond et corail, en vouvoiement, sans peur ni amendes.

**Retirée : direction B « Calendrier clair »** (l'échéancier comme colonne vertébrale du site). Le brief demande de gagner sur la trésorerie, les relances et le ton artisan, pas sur la conformité, et veut un hero qui reste vrai après les échéances. L'échéancier reste le bloc 2 dans les deux pistes.

### Direction A : « Carnet chaleureux » (recommandée)
- Fond crème, cartes blanc cassé, violet profond pour le texte et les boutons, corail pour un seul signal (facture payée, jalon atteint), toujours doublé d'un texte.
- **Garde-fou** : le crème seul ne distingue pas Liasse d'Indy (`#FEF7EC`, très proche de `#FBF6EE`, n° 16). La différence vient du violet profond (absent chez Indy, rose `#FA5D89`), de maquettes de l'app Liasse plutôt qu'une photo d'artisan avec cartes flottantes, et de la trésorerie à 90 jours, qu'Indy ne montre pas.
- Hero : champ e-mail et conditions de l'essai sous le bouton (n° 1, 3, 13, 27), puis la capture mobile qui dépasse du premier écran.
- Captures mobiles en grand, légèrement inclinées, ombres douces. Les montants s'animent une fois au passage (n° 22, 24). Démo au scroll pour l'aperçu (n° 25).
- Échéancier en 3 cartes datées (n° 6) avec le sélecteur de profil en pastilles (n° 27).
- Inspirations : 1, 3, 6, 13, 16, 22, 24, 25, 27.

### Direction C : « Tableau de bord doux »
- Hero sur l'alternative C du brief (« Votre compte dans 90 jours, dès aujourd'hui »), pour les campagnes trésorerie. La courbe à 90 jours vit dans la capture mobile du hero, pas dans un tableau de bord plein écran (n° 22, 3). Une phrase sous la courbe dit ce qu'elle signifie (« Point bas le 1er décembre : vous restez au-dessus de votre seuil »).
- Widgets arrondis et grands montants en chiffres tabulaires (n° 24).
- **Correction** : la version précédente disait « moins de crème ». Le crème reste le fond de page, comme le veut la marque ; le violet clair ne sert qu'aux surfaces des cartes.
- Registre : pilotage, adapté à Nathalie et aux TPE de services. Moins direct pour les artisans du bâtiment, cœur de cible.
- Inspirations : 3, 22, 24, 21, 28.

### 3 « à ne pas faire »
1. Pas de dégradé violet-noir futuriste ni de glassmorphisme (n° 20, 26, à côté) : c'est le code crypto et néobanque, pas celui de l'artisan.
2. Pas de corail pour le texte sur fond crème (2,54:1), ni pour les alertes de réforme : le corail signale une bonne nouvelle (« payé »), jamais une menace. Pennylane écrit « Évitez les amendes » (n° 6) : Liasse ne le fera pas.
3. Pas de tableau de bord de DAF en hero (graphiques denses, jargon) : une seule courbe, trois montants, une phrase.

---

## Palette, polices, design tokens, composants

Toutes les valeurs ont été revérifiées le 2026-11-12 contre la marque (crème, violet profond, corail ; DM Sans ou Outfit ; chiffres tabulaires) et contre l'accessibilité du brief (WCAG 2.1 AA). Contrastes calculés avec la formule WCAG 2.1.

### Palette recommandée

Inchangée : aucune observation ne justifie de changer une couleur. Deux références à côté confirment des choix sans rien ajouter : le lilas `#E8DFFB` de la n° 7 (palette extraite automatiquement) est proche du violet clair `#ECE4FA` ; la n° 18 (Yapstone) donne à chaque couleur sa teinte claire, principe repris pour les fonds de messages.

| Rôle | Hex | Contraste mesuré |
|---|---|---|
| Crème (fond) | `#FBF6EE` | |
| Crème profond (surfaces) | `#F3EADB` | |
| Violet profond (marque, texte) | `#2E1A5C` | 13,76:1 sur crème ; blanc sur violet 14,80:1 |
| Violet clair (surfaces d'accent) | `#ECE4FA` | violet profond dessus : 12,02:1 |
| Corail (accent) | `#FF6F59` | 2,54:1 sur crème, 2,74:1 sur blanc, 2,30:1 sur `#F3EADB` : jamais pour du texte, et sous 3:1 pour un élément graphique (voir correction). 5,41:1 sur violet profond |
| Corail foncé (texte d'accent) | `#B8412E` | 5,09:1 sur crème, 5,48:1 sur blanc, 4,59:1 sur `#F3EADB` : AA validé. 4,45:1 sur `#ECE4FA` : pas de texte courant sur violet clair |
| Encre neutre | `#1F1A2B` | 15,73:1 sur crème |

**Correction du 2026-11-12 (refonte)** : le corail était prévu pour les pastilles et le jalon actif. Une pastille qui porte un sens doit atteindre 3:1 (critère 1.4.11) : le corail n'y arrive sur aucun fond clair. Une pastille corail est donc toujours accompagnée d'un texte ou d'une icône (« Payée »), ou entourée d'un contour `#B8412E`. Sur violet profond, le corail passe (5,41:1).

### Polices (Google Fonts)

Test fait dans le navigateur le 2026-11-12 avec les polices servies par Google Fonts. Avec DM Sans (version statique et version variable), « 111111 » et « 000000 » gardent des largeurs différentes même avec `font-variant-numeric: tabular-nums` : DM Sans n'a pas de chiffres tabulaires sur Google Fonts. Outfit 600 les a. DM Mono est à chasse fixe. La n° 24 (Depo) utilise DM Sans en texte courant.

- **DM Sans** pour les titres (700) et le texte (400).
- **Montants** : **Outfit 600** avec `font-variant-numeric: tabular-nums`. Elle reste dans les deux polices citées par le brief. DM Mono en repli, pour les tableaux uniquement.
- **Alternative** : Outfit seule (600 et 700 en titres), ce qui règle la question des chiffres avec une seule police.

### Couleurs

| Token | Hex | Usage |
|---|---|---|
| `color.brand.primary` | `#2E1A5C` | Boutons primaires, titres |
| `color.brand.primary-hover` | `#432A80` | Survol (texte blanc : 11,16:1) |
| `color.brand.primary-soft` | `#ECE4FA` | Surfaces d'accent, badges |
| `color.brand.accent` | `#FF6F59` | Signal « payé », jalon atteint, pastilles, toujours avec un texte ou une icône. Pas de texte sur fond clair |
| `color.brand.accent-text` | `#B8412E` | Texte d'accent si nécessaire (5,09:1 sur crème). Pas sur `primary-soft` (4,45:1) |
| `color.success.text` | `#17704A` | Validation, « Facture payée » en texte (5,35:1 sur `success.bg`) |
| `color.success.bg` | `#E5F4EC` | Fond des messages de succès |
| `color.error.text` | `#B42318` | Erreurs de formulaire (5,75:1 sur `error.bg`) |
| `color.error.bg` | `#FDECEA` | Fond des messages d'erreur |
| `color.warning.text` | `#9A5B00` | Échéance de facture proche, avertissements (4,94:1 sur `warning.bg`). Jamais pour la réforme |
| `color.warning.bg` | `#FFF3DC` | Fond des avertissements |
| `color.neutral.0` | `#FFFFFF` | Champs |
| `color.neutral.50` | `#FBF6EE` | Fond de page (crème) |
| `color.neutral.100` | `#F3EADB` | Surfaces, cartes |
| `color.neutral.200` | `#E3D8C6` | Bordures décoratives uniquement (1,31:1 sur crème) |
| `color.neutral.500` | `#7A7186` | Texte désactivé et bordure des champs (4,31:1 sur crème, 4,63:1 sur blanc, 3,88:1 sur `#F3EADB`) |
| `color.neutral.700` | `#544B63` | Texte secondaire (7,61:1 sur crème, 6,87:1 sur `#F3EADB`) |
| `color.neutral.900` | `#1F1A2B` | Texte principal |

`neutral.500` reste sous 4,5:1 sur crème : réservé au texte désactivé, jamais à un texte utile. La bordure d'un champ doit atteindre 3:1 (critère 1.4.11) : `neutral.200` ne suffit pas, d'où `neutral.500` pour les champs.

### Typographie
`font.sans` = DM Sans, `font.display` (optionnel) = Outfit, `font.numeric` = **Outfit 600 avec `tabular-nums`**, repli DM Mono.

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
`shadow.sm` = `0 1px 3px rgba(46,26,92,.08)` ; `shadow.md` = `0 10px 30px rgba(46,26,92,.10)` (cartes mises en avant) ; `shadow.device` = `0 30px 60px -20px rgba(46,26,92,.25)` (mockups) ; `shadow.focus` = `0 0 0 2px #FBF6EE, 0 0 0 4px #2E1A5C`.

**Correction du 2026-11-12 (refonte)** : `shadow.focus` valait `0 0 0 3px rgba(46,26,92,.4)`. Sur crème, ce violet à 40 % donne `#A99EB4`, à 2,37:1 (2,41:1 sur blanc) : sous 3:1, l'anneau de focus ne se voit pas assez. Le nouvel anneau est opaque (13,76:1 sur crème), avec un liseré crème de 2 px pour rester visible sur un bouton violet.

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

**Champ e-mail et bouton (hero)** : en desktop, champ et bouton sur une ligne. En mobile, champ pleine largeur puis **un seul** bouton pleine largeur, 48 px de haut minimum pour les deux (Mercury, mesuré à 38 et 40 px, est trop petit). Label visible (« Votre e-mail professionnel »), pas seulement un texte indicatif. `type="email"`, `autocomplete="email"`, `inputmode="email"`. Bordure du champ en `neutral.500`. Sous le bouton : les conditions de l'essai en une ligne (modèles : n° 13, 27), puis « Liasse n'est pas une banque » si la connexion bancaire est citée au-dessus (modèle : n° 1). Le même bloc revient en pied de page.

**Sélecteur de profil (échéancier)** : 4 pastilles « Artisan », « Commerçant », « Profession libérale », « Société », en boutons radio accessibles, 44 px de haut minimum, qui passent à la ligne en mobile (les onglets de Pennylane sont coupés à 390 px). Le profil choisi est écrit, pas seulement coloré. Modèle : n° 27.

**Carte** (fonctionnalité, formule, avis) : fond `neutral.0` ou `neutral.100`, `radius.md`, padding `space.6`. La formule recommandée a une bordure de 2 px `brand.primary` et un badge `brand.primary-soft`. Chaque prix porte « HT » et le montant TTC juste dessous (modèle pour le HT : n° 21).

**Tableau comparatif** : colonnes « Liasse » puis des catégories (« Logiciel gratuit », « Tableur », « Papier », par exemple), jamais des noms de concurrents (modèle : n° 28). Chaque cellule a un texte (« Oui », « Non », « En option »), visible ou lu par les lecteurs d'écran, en plus de l'icône.

**Formulaire** : erreur sous le champ (`error.text`, icône, `aria-describedby`, `aria-invalid`). Succès dans un bloc `success.bg` qui remplace le formulaire et prend le focus.

| À faire | À ne pas faire |
|---|---|
| Un seul champ (e-mail) pour l'inscription | Nom, téléphone et SIRET dès l'inscription |
| Conditions de l'essai écrites sous le bouton | Conditions cachées dans les CGU |
| Montants en chiffres tabulaires (Outfit), animés une fois | Compteurs qui tournent en boucle |
| Corail pour les bonnes nouvelles (payé, jalon atteint), avec un texte | Corail ou rouge pour faire peur avec la réforme |
| Cibles tactiles d'au moins 44 px, focus visible | `outline: none` ou liens de 12 px en pied de page |
| Maquettes de l'app Liasse, produites pour la démo et cohérentes d'un écran à l'autre | Mockups génériques sans lien avec le produit |
| Échéancier lisible sans la couleur (texte et icônes) | Frise uniquement codée par couleur |
| Un même chiffre partout, daté | Deux chiffres pour la même chose (Qonto, Pennylane, Billow) |
| « Plateforme agréée » expliqué, avec un lien vers la liste officielle, sans numéro inventé | « Plateforme agréée » sans numéro (Qonto, Pennylane) |
| Région d'hébergement et chiffrement écrits en clair | « Infrastructure cloud sécurisée » sans nom (Billow) |

---

## À côté

| # | Référence | Capture | Pourquoi à côté |
|---|---|---|---|
| 4 | [Fintt.te, Landing Page (Fintech)](https://www.behance.net/gallery/141980721/Finttte-Landing-Page-(Fintech)) (Behance) | Non capturé | Non vérifié : Behance renvoie une erreur 400 à un navigateur automatisé. Remplacé par le n° 22. |
| 5 | [Abby, facturation électronique](https://abby.fr/facturation-electronique) (France) | Non capturé | Non vérifié : erreur 403 CloudFront sur la page et sur l'accueil. Le calendrier, la gratuité et les notes ne sont donc pas cités ici ; l'étude de cas s'appuie sur la presse pour Abby. Pour l'échéancier, voir le n° 6. |
| 7 | [Fintech mobile app](https://dribbble.com/shots/15812075-Fintech-mobile-app) (Excel Belmiro, Dribbble) | [capture](captures/a-cote/07-dribbble-excel.jpg) | Hors marque et hors ton : dégradé rose-violet, personnage 3D, registre d'app grand public, loin de « simple, chaleureux, rassurant » et de la palette crème, violet profond, corail. La palette (`#E8DFFB`, `#CAB7F8`, `#AA2DA8`, `#6538E5`, `#613939`, `#C4A9BD`) est extraite automatiquement. Le lilas `#E8DFFB` est cité dans « Palette ». |
| 9 | [Tara](https://onepagelove.com/tara) (One Page Love, 25 septembre 2026) | [capture](captures/a-cote/09-onepagelove-tara.jpg) | Hors marque et hors ton : coffre crypto, rendus 3D, dégradés vert-rose, police Herokid. Le seul détail utile (champ et « Join waitlist » sur une ligne) est cité au bloc 1 et mieux couvert par les n° 1 et 3. |
| 10 | [Revolut](https://godly.website/website/revolut-254) (Godly) | Non capturé | Non vérifié : redirection vers recent.design ; le site de Revolut Business affiche un challenge Cloudflare, non contourné. Remplacé par le n° 24. |
| 11 | [Eco](https://godly.website/website/eco-935) (Godly) | Non capturé | Non vérifié : redirection vers recent.design. Remplacé par le n° 25. |
| 12 | [Invo, SaaS product for automatizing invoicing](https://www.behance.net/gallery/157230691/Invo-SaaS-product-for-automatizing-invoicing?locale=en_US) (Behance) | Non capturé | Non vérifié : erreur 400. Remplacé par le n° 23. |
| 14 | [Maze, Pricing](https://maze.co/pricing/) (fiche [Land-book](https://land-book.com/websites/37536-flexible-pricing-and-plans-maze) bloquée par Cloudflare) | [capture](captures/a-cote/14-maze-pricing.jpg) | Contre-exemple pour le bloc 7 : 2 formules, « Free » et « Enterprise » (« Custom pricing »), et aucun prix. Le brief demande 2 formules avec prix HT et TTC lisibles. Titre « Pricing & Packages » en Phonic 300 de 90 px. |
| 15 | [Bonsai](https://www.hellobonsai.com/pricing), via [SaaS Landing Page](https://saaslandingpage.com/bonsai/) | [tarifs](captures/a-cote/15-bonsai-pricing.jpg), [fiche](captures/a-cote/15-bonsai-slp.jpg) | Contraire au bloc 7 : 4 formules (9, 19, 29 et 49 $ par utilisateur et par mois) au lieu de 2, sans mention HT ni TTC, bouton en dégradé sur la formule mise en avant. Sous le hero, 13 onglets de fonctionnalités, beaucoup pour un artisan. Palette `#003C2F`, `#22AD01`, `#EE8146`, Geist Sans, hors marque. Le badge « Most popular » est cité au bloc 7. |
| 17 | [Invoice Builder by Tola](https://www.awwwards.com/sites/invoice-builder-by-tola) (Awwwards, mention honorable, 19 janvier 2024) | [capture](captures/a-cote/17-awwwards-tola.jpg) | URL morte : le site primé (invoice.tolahq.com) renvoie une erreur Cloudflare 1000. Seule la fiche a été vue (tablette en biais, « Create beautiful invoices in seconds »). L'aperçu en direct et les montants n'ont pas pu être vérifiés. |
| 18 | [Yapstone, par Hangar](https://hangar.co/projects/yapstone) (épingle [Pinterest](https://co.pinterest.com/pin/1044694444796643488/) derrière un mur de connexion) | [capture](captures/a-cote/18-hangar-yapstone.jpg) | Contexte seulement : identité d'une fintech de paiement, noir chaud, lilas et 5 couleurs vives (lilas, bleu, vert, jaune, rose) avec chacune sa version claire, police Graphik. Hors palette du brief (crème, violet profond, corail). Le principe d'une teinte claire par couleur est cité dans « Palette ». |
| 19 | [Idées « Purple Website Design Inspiration »](https://www.pinterest.com/ideas/purple-website-design-inspiration/916159820380/) (Pinterest) | Non capturé | Non vérifié : mur de connexion, aucun visuel lisible. Remplacé par le n° 26. |
| 20 | [Fintech futuristic Website design](https://dribbble.com/shots/24273813-Fintech-futuristic-Website-design) (épingle [Pinterest](https://www.pinterest.com/pin/842454674093763176/) derrière un mur de connexion) | [capture](captures/a-cote/20-dribbble-fintech-futuristic.jpg) | Contre-exemple : « FinNova », blanc sur noir violacé, halo violet, bouton violet électrique, « Cryptocurrency » au pied du hero, « Starts rating » avec la faute. Contraire à la palette crème et au ton rassurant du brief. |
| 26 | [Recherche Dribbble « purple fintech website »](https://dribbble.com/search/purple-fintech-website) | [capture](captures/a-cote/26-dribbble-recherche-violet.jpg) | Contexte sectoriel : sur les 8 premières vignettes, 6 sont violet électrique, souvent sur fond sombre, avec de la 3D. Le violet profond et calme du brief (`#2E1A5C`) n'y figure pas. Rien à reprendre, mais cela confirme que Liasse se distingue par un violet sombre sur crème. |

---

## Galeries : requêtes lancées

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
| **Ajouts du 2026-11-12** (Dribbble 3, One Page Love 2, site réel 1) | | 6 (n° 21 à 26) |
| **Ajouts de la refonte** (One Page Love 2) | | 2 (n° 27, 28) |

| Date | Galerie | Requête ou page | Résultat |
|---|---|---|---|
| 2026-11-12 | Dribbble | `purple fintech website` | 6 vignettes violet électrique sur 8 : n° 26 (à côté) |
| 2026-11-12 | Dribbble | `fintech landing page` | Majorité de vignettes sombres, aucune retenue |
| 2026-11-12 (refonte) | One Page Love | recherche `security` | Redirigée vers l'accueil, aucun résultat |
| 2026-11-12 (refonte) | Dribbble | `fintech security section` | Liste lisible (« Fintech Website Trust & Credibility », « Fintech SaaS UI, AI, Payments & Security Feature Section »), mais les 2 fiches ouvertes affichent « Let's confirm you are human ». Non contourné, aucune retenue |
| 2026-11-12 (refonte) | One Page Love | genre `finance` | 8 sites finance. Retenus : Billow (n° 27), Statements (n° 28). Écartés : Uglycash (néo-brutaliste, crypto, rose électrique), Vault AI (fond noir, « Futuristic »), The Useless Fund (expérimental) ; Tara, Depo et invoicemon déjà au bench |

---

## Arbitrages

- **DM Sans et chiffres tabulaires** : on garde DM Sans pour les titres et le texte, et on passe les montants en Outfit 600 avec `tabular-nums`, parce que DM Sans servie par Google Fonts n'a pas de chiffres tabulaires (test du 2026-11-12) et qu'Outfit reste dans les deux polices de la marque.
- **Le corail comme signal** : on n'utilise jamais le corail seul pour dire « payé » ou marquer le jalon actif. Il est sous 3:1 sur tous les fonds clairs (2,54:1 sur crème), donc un texte ou une icône l'accompagne toujours, ou un contour `#B8412E`.
- **Le crème déjà pris par Indy** : on garde la palette crème, violet profond et corail. On se distingue d'Indy (`#FEF7EC`, carte « Payée ») par le violet profond, des maquettes de l'app Liasse au lieu d'une photo d'artisan, et la trésorerie à 90 jours.
- **Aucun chiffre propre à Liasse** : on retire du brief l'équipe, les utilisateurs, la levée, les cibles de KPI, le budget et la promesse « 2 minutes », parce qu'ils seraient inventés. Les indicateurs restent, sans cible.
- **Prix et essai** : on cale les 2 formules sur les deux premières formules publiques de Pennylane (7 et 14 € HT par mois) et l'essai sur celui de Qonto (30 jours), sources vues le 2026-11-13, et le site les marque « prix de démonstration ». Une démo sans prix ne permet pas de tester la grille HT et TTC.
- **Avis** : on retire le bloc d'avis. Une entreprise fictive n'a ni note ni verbatims, et des avis inventés seraient de faux avis.
- **Plateforme agréée** : on écrit « plateforme agréée » dans le texte, sans numéro et sans le logo officiel, avec un lien vers la liste d'impots.gouv.fr. Liasse n'a pas d'immatriculation, et un faux numéro tromperait le visiteur.
- **Prestataires réels** : on ne nomme ni hébergeur, ni agrégateur bancaire, ni logiciel comptable compatible. On écrit la région d'hébergement, le chiffrement, le statut réglementaire du prestataire et les formats d'export, parce qu'une entreprise fictive n'a aucun contrat à afficher.
