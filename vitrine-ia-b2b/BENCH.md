# Benchmark visuel : Ordo (IA B2B, entreprise fictive)

Ce bench suit le brief client bloc par bloc : chaque référence retenue sert une exigence précise de [`BRIEF-CLIENT.md`](BRIEF-CLIENT.md), les autres sont rangées à côté avec leur raison.

## Limites, à lire en premier

Vérification du 2026-11-12, faite avec un vrai navigateur (Chrome piloté par Playwright).

- **Ce qui a été vu** : 14 des 20 références d'origine ont été ouvertes et capturées, dont 11 sur leur lien d'origine. Pour 3 autres, le lien d'origine était bloqué et une page équivalente a été ouverte à la place : le site réel de Fin (n° 6) et de Factory (n° 11), le shot Dribbble d'Archon (n° 4). 6 références ont été ajoutées (n° 21 à 26). Captures en 1440 × 900 px, au-dessus de la ligne de flottaison, plus 2 captures complémentaires (site actuel de Well au n° 7, page de Ramp au n° 12) et 4 captures mobiles en 390 × 844 px. Les couleurs et les polices citées ont été relevées dans la page (`getComputedStyle`), pas devinées. Les chiffres cités sont ceux affichés le 2026-11-12.
- **Ce qui reste bloqué** : Behance (n° 9, 16, 18) renvoie « HTTP ERROR 400 » au navigateur automatisé. Land-book (n° 5, 14) et Lapa Ninja (n° 6, 11) bloquent par Cloudflare. Pinterest (n° 4, 19) affiche un mur de connexion. Ces références sont marquées « non vérifié » et rangées à côté.
- **Corrections de la vérification** : Well (n° 7) a changé de produit et passe sur fond noir. Bubble Flow (n° 10) ne montre aucune frise en 3 étapes. La page de Ramp (n° 1) parle de « Ramp's agent » au singulier, pas de quatre agents. L'exemple de Fin (n° 6) est un changement d'adresse, pas un remboursement. 11sight (n° 17) est un téléphone 3D sur fond noir, et le site ne répond plus. Quid AI (n° 15) est la référence la plus proche d'Ordo.
- **Refonte du 2026-11-12** :
  - Chaque référence est triée : **13 inspirations** (n° 1, 2, 6, 8, 11, 12, 15, 20, 21, 22, 23, 25, 26) et **13 références à côté** (n° 3, 4, 5, 7, 9, 10, 13, 14, 16, 17, 18, 19, 24). Rien n'est supprimé, les numéros ne changent pas.
  - Les captures sont rangées dans [`captures/inspis/`](captures/inspis/) et [`captures/a-cote/`](captures/a-cote/). Les captures mobiles suivent le tri de leur référence (Ramp, Fin et Pennylane sont des inspirations).
  - Le bench est réorganisé selon l'arborescence du brief (9 blocs), avec un tableau de couverture.
  - La direction C « Éditorial » est retirée (voir **Directions**). Le brief ne fixe pas de nombre de pistes : 2 sont gardées.
  - **Tokens corrigés** pour suivre le brief : l'anneau de focus (2,2:1, sous le seuil de 3:1), les usages du vert (réservés à l'état « traité », plus au succès du formulaire), la police du texte courant (Inter n'est pas cité par le brief), et un token de bordure de champ ajouté (le bench demandait au moins 3:1 sans donner de valeur). Détails dans **Palette, polices, design tokens, composants**.
  - **Recherche complémentaire** pour les blocs Tarifs et FAQ : One Page Love (sections Pricing, Pricing Table, Pricing Slider, Contact Form, FAQ Accordion) vu, rien retenu. Dribbble demande une vérification « Let's confirm you are human » sur la recherche : non contournée. Aucune référence ajoutée.
- **Passe du 2026-11-13** : le brief n'a plus de chiffre inventé (titre chiffré, nombre de clients, cibles des indicateurs, budget). Le bench suit : les anciens points pour le client sont devenus des décisions (**Arbitrages**). Photos d'équipe cherchées en banque d'images : Unsplash répond « Access Denied », Pexels affiche une vérification anti-robots Cloudflare, non contournée. Le brief passe donc à un bloc « Qui sommes-nous » sans photo.
- **Bannières cookies** : refusées partout où un refus existait (« Reject all », « Opt out of all »). Sur SaaS Landing Page, la seule option était « I agree » : la bannière a été masquée, pas acceptée. Sur Pennylane, la fenêtre de choix du pays a été fermée en choisissant « France ».
- **Données personnelles** : les avatars des designers sur Dribbble et One Page Love sont floutés. Les noms restent quand ils créditent un studio ou un auteur.

| Source | Références | Vues le 2026-11-12 |
|---|---|---|
| Sites réels du secteur | 2 (n° 1, 2) + 1 ajouté (n° 25) | 3 sur 3 |
| Behance | 3 (n° 9, 16, 18) | 0 : erreur 400. Remplacées par les n° 21, 25 et 24 |
| Dribbble | 2 (n° 3, 10) + 4 ajoutés (n° 21 à 24) + 1 équivalent (n° 4) | 7 sur 7 |
| Pinterest | 2 (n° 4, 19) | 0 : mur de connexion. Le n° 4 est vu sur Dribbble |
| Awwwards | 3 (n° 7, 17, 20) | 3 sur 3 |
| Land-book | 2 (n° 5, 14) | 0 : Cloudflare. Le n° 14 est remplacé par le n° 26 |
| Lapa Ninja | 2 (n° 6, 11) | 0 : Cloudflare. Les sites réels de Fin et Factory sont vus à la place |
| SaaS Landing Page | 2 (n° 12, 13) | 2 sur 2 |
| One Page Love | 2 (n° 8, 15) + 1 ajouté (n° 26) | 3 sur 3 |
| Godly | 0 | Non relancé (redirige vers recent.design sur ce projet) |

---

## Couverture du brief

| Exigence du brief | Inspirations | Manque |
|---|---|---|
| 1. Hero (titre sans chiffre, CTA démo, lien tarifs, logos des outils connectés) | 1, 15, 21, 22, 23, 2 | Rien pour le titre : aucun titre de hero relevé ne contient de chiffre, ce qui va dans le sens du titre retenu. Logos d'outils sous le hero : vus seulement dans le visuel de Quid AI. |
| 2. Démo produit (boucle de 20 s sur une facture, version verticale) | 6, 1, 8, 2, 11, 23 | Aucun écart montré en entier (Ramp affiche seulement l'état « Checking for discrepancies… »). Contrôle pause et `prefers-reduced-motion` non vérifiés dans le panel. |
| 3. Comment ça marche (3 étapes) | 21, 23, 15 | Aucune frise en exactement 3 étapes : 5 onglets chez Agemandi, 4 pastilles chez FiscalPro. |
| 4. Intégrations (Pennylane, Sage, Qonto, connecteurs en cours marqués) | 12, 15 | Aucun délai de mise en route affiché à côté des logos. |
| 5. Preuves et témoignages (3 engagements sans chiffre, 2 ou 3 témoignages sans photo) | 26, 20, 1, 15 | Aucun bloc d'engagements sans chiffre vu : les exemples du panel sont chiffrés. Le témoignage de Quid AI est décrit, pas capturé. |
| 6. Sécurité et données (RGPD, France, pas d'entraînement, chiffrement, droits, `/securite`) | 15, 25, 21 | Aucun DPA téléchargeable ni liste de sous-traitants vus. Aucune page `/securite` ouverte. |
| 7. Tarifs (3 paliers publics par volume de factures, prix d'entrée HT) | aucune | Quid AI n'a pas de tarifs. Numira (n° 22) montre le titre « Simple Pricing That Fits Any Team », paliers illisibles. One Page Love : exemples d'agences, d'apps ou sur fond sombre. |
| 8. Qui sommes-nous et on recrute (bloc court sans photo, 3 à 5 postes, lien carrières) | aucune | Aucune section emploi dans le panel. Pas de galerie dédiée sur One Page Love, non cherché ailleurs. Photos d'équipe : Unsplash et Pexels bloqués le 2026-11-13, donc pas de photo. |
| 9. FAQ et formulaire de démo (8 questions, 4 champs) | 25 (rôle du cabinet, pour Sophie) | Aucun formulaire à 4 champs ni FAQ en capture. La FAQ de Quid AI est décrite, pas capturée. One Page Love « Contact Form » et « FAQ Accordion » : rien retenu. |
| Mobile (démo verticale, barre fixe, logos en défilement) | 1, 6, 25 (captures mobiles) | Barre fixe en bas et logos en défilement horizontal : vus nulle part. |
| Marque : palette (presque blanc, bleu nuit, vert réservé à « traité ») | 20, 25, 11 | Aucun site ne réserve son vert à un seul état : Pennylane et Catalyze le mettent sur les boutons ou les liens. |
| Marque : typo (Inter Tight ou Geist, mono pour les chiffres) | 11, 2 | Aucun exemple de chiffres héros en mono (n° 26 le confirme). |
| Marque : une seule animation forte | 1 | Ramp a une animation dans le hero. Le reste de la page n'a pas été audité sous cet angle. |
| Accessibilité (contrastes, vert jamais en texte, focus) | 1, 25 (boutons à 16:1 et 8,5:1) | Contre-exemples nombreux (n° 2, 11, 15, 20). Navigation clavier non testée dans le panel. |
| Règle des chiffres : aucun chiffre de résultat, une source à côté de tout chiffre public | 1 | Ramp rattache chaque chiffre à un renvoi numéroté : c'est la forme reprise pour les rares chiffres publics (date de la réforme, prix d'entrée calé sur Yooz). |
| Preuve « rapprochée avec sa commande » | 1, 15 | Aucun écart facture et commande montré côte à côte. |
| Preuve « Vous validez, Ordo exécute » (validation, journal) | 15, 6, 2 | Journal horodaté vu seulement chez Well (n° 7, à côté). |
| Preuve « branché sur Pennylane, Sage et Qonto » | 12, 15 | Étapes de mise en route : vues nulle part. |
| Preuve « données en France, pas d'entraînement » | 15, 25 | Hébergeur et région nommés : vus nulle part. |
| Preuve « un prix lisible » | aucune | Voir le bloc Tarifs. |
| Mention IA (AI Act) | aucune | Pas observée sous cet angle dans le panel. |

---

## Inspirations, bloc par bloc

### 1. Hero

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 1 | Ramp, page Accounts Payable (https://ramp.com/accounts-payable) | [capture](captures/inspis/01-ramp-ap.jpg) | Fond blanc, titre « A month of AP done in minutes. » en Lausanne 64 px, graisse 400, encre `#0C0A08`. À droite, une animation « Routing to approvals. » fait défiler de vraies lignes de factures (fournisseur, montant, date, numéro). Chiffres : « 2.4x faster », « 85,000+ businesses », chacun avec un renvoi numéroté (1, 2, 3). À éviter : le bouton jaune-vert `#E4F222`. | De vraies lignes de factures dès le hero. Le renvoi sous chaque chiffre sert la règle des allégations : tout chiffre public affiché porte sa source. |
| 15 | Quid AI (https://onepagelove.com/quid-ai, copie https://onepagelove.com/preserved/2025-09-23-quid-ai.html) | [capture](captures/inspis/15-onepagelove-quid-ai.jpg) | Titre « AI agents for your AP/AR workflows » en Space Grotesk 60 px, graisse 500, encre `#190806`. Une facture au centre, avec les champs extraits en étiquettes (centre de coût, numéro, compte général), les sources à gauche (Office, Slack, Gmail, Stripe), les logiciels comptables à droite (DATEV, LexOffice, NetSuite, Sage). À éviter : le bouton `#F94B38` à texte blanc (3,45:1). | Comprendre Ordo en moins de 5 secondes : la facture entre sources et outils dit lecture, rapprochement, écriture. |
| 21 | Accounts Payable Automation SaaS Website, Agemandi (https://dribbble.com/shots/27640668-Accounts-Payable-Automation-SaaS-Website) | [capture](captures/inspis/21-dribbble-ap-automation.jpg) | Hero « AI-powered Accounts Payable. » au-dessus d'une liste de factures fournisseurs avec statuts. La description dit ouvrir « with a product dashboard rather than an abstract promise about AI ». À éviter : la photo de banque d'images et le bleu-violet `#354AEA`. | Montrer le produit plutôt qu'une promesse, pour Claire qui veut voir le vrai traitement. |
| 22 | Landing Page for Invoice Management platform, Nadia Kapyrina pour Numira (https://dribbble.com/shots/27166316-Landing-Page-for-Invoice-Management-platform) | [capture](captures/inspis/22-dribbble-numira.jpg) | Palette publiée `#F2F6F7`, `#010F14`, `#B1D9D0`, `#263B4A`. Au centre, un tableau de factures (fournisseur, montant, date, pièce, statut). La description vise un « calm tone ». | Le tableau de factures comme visuel principal (direction A), ton sobre du brief. |
| 23 | Remittance Reconciliation Software Website Design, Crevio pour FiscalPro (https://dribbble.com/shots/27821027-Remittance-Reconciliation-Software-Website-Design) | [capture](captures/inspis/23-dribbble-fiscalpro.jpg) | Titre « Reconcile PDF Remittance Advice in Xero. Instantly. » : l'outil comptable est nommé dans le titre. À éviter : le fond photo de fleurs floues. | Sous-titre du brief qui nomme Pennylane, Sage ou Qonto. |
| 2 | Dust (https://dust.tt) | [capture](captures/inspis/02-dust.jpg) | Sous le hero, « Trusted by teams at 3,000+ global organizations ». Bouton principal « Request a demo » et lien secondaire « Try for free → ». À éviter : le bouton bleu en dégradé (texte blanc à 3,2:1 au mieux). | Le couple CTA principal plus lien secondaire (« Voir les tarifs »). La ligne de preuve sous le hero devient chez Ordo la rangée des outils connectés, pas un nombre de clients. |

### 2. Démo produit

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 6 | Fin (https://fin.ai/, fiche Lapa Ninja d'origine non vérifiée) | [capture](captures/inspis/06-fin.jpg) | Démo en conversation : le client signale un déménagement, Fin demande un justificatif, le PDF « UtilityBill.pdf » arrive, Fin confirme la nouvelle adresse. Chiffre : « 76% resolution rate, across 12,000+ businesses ». À éviter : le tube 3D orange et la serif fine du titre (« Serrif », 72 px). | Une tâche terminée à partir d'une pièce jointe. Pour Ordo : facture reçue, « rapprochée avec la commande », pastille « Traité ». |
| 1 | Ramp, version mobile | [démo facture](captures/inspis/mobile-ramp-facture.jpg) | Une facture se remplit ligne par ligne (« Draft Invoice #CI-14884 », catégorie, département, lieu), avec les états « Auto coding… » puis « Checking for discrepancies… ». | Démo verticale sur mobile, et l'état de recherche d'écart qui annonce le rapprochement. |
| 8 | invoicemon (https://onepagelove.com/invoicemon, site https://invoicemon.com/) | [capture](captures/inspis/08-onepagelove-invoicemon.jpg) | Sous le titre « A complete invoicing workflow in your browser » (Inter 36 px, graisse 600, encre `#1A1816`), l'éditeur de facture est rendu en HTML dans la page : lignes, quantités, totaux. Ce n'est pas un agent IA. | Démo en HTML/CSS plutôt qu'en vidéo : texte lisible par Google (SEO) et poids léger (< 1,5 Mo sur mobile). Une démo jouable reste une piste de phase 2. |
| 2 | Dust | [capture](captures/inspis/02-dust.jpg) | Des bulles d'agents nommés par tâche (@LeadQual, @Incident, @TicketRouter), chacune avec son résultat (« API gateway p99 latency > 2s »). À éviter : la scène 3D isométrique. | Le journal des actions de la preuve « Vous validez, Ordo exécute » : une bulle « Lecture », « Rapprochement » ou « Relance » avec son résultat. |
| 11 | Factory (https://factory.com/, fiche Lapa Ninja d'origine non vérifiée) | [capture](captures/inspis/11-factory.jpg) | Plus bas, l'interface liste des sessions avec une pastille d'état. Les statuts et les commandes sont en Geist Mono. À éviter : la mono gris clair `#8A8380` en texte (3,5:1). | Statuts et numéros de facture en mono, comme le demande le brief pour les chiffres. |
| 23 | FiscalPro | [capture](captures/inspis/23-dribbble-fiscalpro.jpg) | Statuts « Paid » en vert, « Pending » en orange dans le tableau de bord. | Deux états lisibles dans la démo : « Traité » (vert, avec le mot) et « Écart » (alerte). |

Détail repris d'une référence à côté : le journal horodaté de Well (« 10:40 Hexa Cloud invoice fetched and filed », n° 7) montre une forme possible du journal des actions.

### 3. Comment ça marche

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 21 | Agemandi | [capture](captures/inspis/21-dribbble-ap-automation.jpg) | Frise à onglets numérotés : 01 Capture, 02 Extract & store, 03 Recognise, 04 Auto-match, 05 Approve & pay, avec un panneau marine par étape. | Les 3 étapes du brief (connecter vos outils, Ordo traite, vous validez), un panneau par étape. |
| 23 | FiscalPro | [capture](captures/inspis/23-dribbble-fiscalpro.jpg) | 4 pastilles d'étape au-dessus du tableau de bord : Upload a file, Review, Reconcile, Completion. | Une version compacte des étapes, réutilisable dans la démo. |
| 15 | Quid AI | [capture](captures/inspis/15-onepagelove-quid-ai.jpg) | Plus bas sur la page, un chat : « approve all invoices under €500 from this vendor ». | L'étape « vous validez » et les règles que le client définit lui-même (brief, section 1 : un fournisseur récurrent sous un certain montant). |

### 4. Intégrations

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 12 | 15 Outstanding Integration Page Examples, page intégrations de Ramp (https://saaslandingpage.com/articles/15-outstanding-integration-page-examples/) | [article](captures/inspis/12-saaslp-integrations.jpg) ; [Ramp](captures/inspis/12b-saaslp-ramp-integrations.jpg) | Ramp : « Explore Integrations », recherche, filtres par catégorie (Accounting, Expense Automation, HR and payroll, Procurement…), « 123 Integrations », grille logo, nom et catégorie. L'article cite aussi Resend : apps disponibles, à venir et sur mesure. | 3 logos en grand (Pennylane, Sage, Qonto), puis un groupe « bientôt disponible » : les « connecteurs en cours, marqués comme tels » du brief. |
| 15 | Quid AI | [capture](captures/inspis/15-onepagelove-quid-ai.jpg) | Logiciels comptables à droite de la facture (DATEV, LexOffice, NetSuite, Sage). | Les connecteurs dans le visuel principal, puis repris dans la section. CTA « Vérifier la compatibilité de mon outil » juste dessous. |

Détail repris d'une référence à côté : Dayos (n° 13) pose son agent sur les logos de Workday et ServiceNow, comme une couche au-dessus des outils existants.

### 5. Preuves et témoignages

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 26 | Metrics Section Examples (https://onepagelove.com/section/metrics) | [capture](captures/inspis/26-onepagelove-metrics.jpg) | Kelvin : 4 chiffres sur une ligne, sous un filet, libellés en petites capitales. The Queue : 3 pourcentages, chacun avec une ligne d'explication. Aucun exemple n'utilise la mono. | La mise en page des 3 engagements : un libellé court en grand, un filet, une ligne d'explication, sans chiffre. |
| 20 | Catalyze AI, Halo Lab (https://www.awwwards.com/sites/catalyze-ai-saas-website, site https://catalyzeai.webflow.io/) | [capture](captures/inspis/20-awwwards-catalyze.jpg) | 3 chiffres sous le hero (400mm+, $3Tn, $77Bn). À éviter : les liens en vert sur fond clair (1,9:1). | Une rangée de 3 éléments sobre, sans compteur animé. |
| 1 | Ramp | [capture](captures/inspis/01-ramp-ap.jpg) | Plus bas : « Up to 7x fewer clicks to process a bill vs Bill.com », « Up to 95% », OCR « 99% accuracy », chacun avec un renvoi numéroté. | La forme du renvoi vers la source, pour les rares chiffres publics affichés (brief : allégations). |
| 15 | Quid AI | [capture](captures/inspis/15-onepagelove-quid-ai.jpg) | Logos clients sous le hero, puis un témoignage de CFO (vu sur la copie, hors capture). | Témoignage fictif d'un profil proche de Claire (DAF), sans photo. |

Détail d'une référence à côté, non repris : Archon (n° 4) utilise une grande phrase chiffrée comme intertitre (« 20% of the U.S. software market »). Ordo n'a pas de chiffre à mettre à cette place.

### 6. Sécurité et données

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 15 | Quid AI | [capture](captures/inspis/15-onepagelove-quid-ai.jpg) | Bloc sécurité en 3 points : RGPD, « Your data will not be used to train AI models available publicly », chiffrement (hors capture). | La phrase « pas d'entraînement sur vos données » attendue par Karim, dans un bloc court. |
| 25 | Pennylane (https://www.pennylane.com/fr) | [capture](captures/inspis/25-pennylane.jpg) | Preuves en ligne courte : ISO/IEC 27001, « Made in France », bloc « Plateforme Agréée immatriculée » pour la facture électronique. | Hébergement en France et conformité, affichés comme des preuves sobres. |
| 21 | Agemandi | [capture](captures/inspis/21-dribbble-ap-automation.jpg) | Bloc auditabilité : « 10 years » de conservation des pièces. | La piste d'audit attendue par Claire, à côté des droits d'accès. |

### 7. Tarifs

Aucune inspiration. Voir **Couverture du brief**. À produire sans modèle : 3 paliers par volume de factures par mois, ce qui est inclus, et le libellé de CTA par palier donné par le brief.

Repère de prix, sans modèle visuel : Yooz affiche « À partir de 99 € » pour l'abonnement mensuel de sa version entreprise (https://www.getyooz.com/fr/tarifs, vu le 2026-11-13, page non capturée). Le palier Essentiel d'Ordo reprend ce prix d'entrée comme prix de démo. Voir **Arbitrages**.

### 8. Qui sommes-nous et on recrute

Aucune inspiration. À produire sans modèle : le bloc « Qui sommes-nous » court, sans photo (texte dans le brief, section 6), puis 3 à 5 postes et le lien vers la page carrières.

Photos d'équipe : recherche tentée le 2026-11-13. Unsplash (https://unsplash.com/s/photos/startup-team-office) répond « Access Denied ». Pexels (https://www.pexels.com/search/small%20team%20office/) affiche une vérification anti-robots Cloudflare, non contournée. Aucune photo retenue, on ne cherche pas plus loin.

### 9. FAQ et formulaire de démo

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 25 | Pennylane | [capture](captures/inspis/25-pennylane.jpg) | Onglets d'audience au-dessus de l'en-tête : « Indépendants et TPE », « PME et ETI », « Cabinet expertise comptable ». | Une mention claire du rôle de l'expert-comptable pour Sophie, et son contact partenaire (FAQ et pied de page). |

### Transverse : marque et accessibilité

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 20 | Catalyze AI | [capture](captures/inspis/20-awwwards-catalyze.jpg) | Fond `#F8F9FB`, encre `#07133B`, vert `#1AD079`, titre en Hellix 58 px, graisse 600. Presque la palette d'Ordo, primée en 2023. | Preuve que fond clair, encre marine et vert vif tiennent ensemble. Risque de ressemblance : voir **Arbitrages**. |
| 25 | Pennylane | [capture](captures/inspis/25-pennylane.jpg) | Encre sarcelle `#003D3D`, titre en Manrope 52 px, graisse 600. Bouton vert `#00F872` à texte `#003D3D` (8,5:1). | Un vert vif dosé sur fond clair, avec un texte foncé dessus. Ce vert et l'accent d'Ordo sont à 1,22:1 l'un de l'autre. |
| 11 | Factory | [capture](captures/inspis/11-factory.jpg) | Fond `#F9F9F9`, titre en capitales Geist 60 px, graisse 500. Sous-titre, boutons et commande `curl` en Geist Mono. | Le couple Geist et Geist Mono autorisé par le brief, sur fond presque blanc. |
| 2 | Dust | [capture](captures/inspis/02-dust.jpg) | Titre en Geist 69 px, graisse 550, encre `#191715`, texte `#57534D`. | Geist en grand corps pour les titres. |
| 1 | Ramp | [capture](captures/inspis/01-ramp-ap.jpg) | Bouton à texte noir sur fond clair : 16:1. | Bouton principal très contrasté : le bouton encre d'Ordo (17,4:1) suit cette logique. |

---

## Mobile

Trois sites vus en 390 × 844 px. Le brief demande : CTA « Réserver une démo » en barre fixe, démo verticale, poids de la démo < 1,5 Mo, LCP mobile sous 2,5 s (seuil « bon » des Core Web Vitals de Google).

| Site | Capture | Ce qu'on observe | Exigence du brief |
|---|---|---|---|
| Ramp (n° 1) | [hero](captures/inspis/mobile-ramp.jpg) ; [démo facture](captures/inspis/mobile-ramp-facture.jpg) | Titre centré, champ e-mail et bouton jaune en pleine largeur, puis l'animation de factures empilée dessous, dans une carte grise. Plus bas, une facture se remplit ligne par ligne, avec « Auto coding… » puis « Checking for discrepancies… ». Seul l'en-tête est fixe. | Démo verticale : confirmée. Une facture tient en largeur mobile avec 3 colonnes courtes par ligne. |
| Fin (n° 6) | [capture](captures/inspis/mobile-fin.jpg) | Le bouton noir « Contact sales » reste dans l'en-tête fixe, en haut. La démo en conversation passe sous les boutons, au format vertical. Aucun élément fixe en bas. | CTA toujours accessible : ici en haut, pas en bas. |
| Pennylane (n° 25) | [capture](captures/inspis/mobile-pennylane.jpg) | Les onglets d'audience défilent horizontalement en haut. L'en-tête reste collé en haut, sans bouton. La capture d'écran de bureau n'est pas recadrée pour le mobile. | À éviter : visuel desktop réduit. Prévoir un visuel recadré pour la démo verticale. |

Ce que ces observations changent pour Ordo :
- **Démo verticale** : le modèle est la facture de Ramp qui se remplit, puis l'état « Traité ».
- **CTA fixe** : aucun des 3 sites n'a de barre fixe en bas. La barre « Réserver une démo » est gardée (voir **Arbitrages**). Elle se masque quand le formulaire est à l'écran.
- **Défilement horizontal** : vu chez Pennylane pour les onglets d'audience, pas pour les logos. Les logos d'intégration en défilement horizontal sont gardés : avec 5 logos (3 disponibles, 2 « bientôt »), une rangée défilante évite de les réduire.

---

## Directions

Le brief ne fixe pas de nombre de pistes (2 allers-retours prévus en S3 et S4). Deux directions compatibles avec la marque sont gardées. Les deux respectent la même base : fond presque blanc, encre bleu nuit, vert seulement pour « traité », Inter Tight ou Geist avec une mono, une seule animation forte (la démo).

### Direction A : « Relevé comptable » (recommandée)
- Filets fins, grille de tableau visible, chiffres en mono.
- La démo ressemble à un vrai document : la facture se surligne ligne par ligne, et une pastille verte « Traité » apparaît à la fin.
- Inspirations : Quid AI (n° 15) pour la facture entre sources et logiciels, Ramp (n° 1) pour la facture qui se remplit sur mobile, Numira (n° 22) et Agemandi (n° 21) pour le tableau de factures, One Page Love Metrics (n° 26) pour les chiffres.
- Registre : sérieux, vérifiable. Elle répond au frein de Claire (« l'IA va se tromper et je ne le verrai pas »).

### Direction B : « Console calme »
- Interface produit en grand, panneaux gris clair (jamais d'interface sombre), journal d'actions de l'agent en mono.
- Le visuel du hero est recadré sur l'action de l'agent (« Relance envoyée à Fournisseur X »), sous le titre.
- Inspirations : Factory (n° 11) pour la mono et les pastilles d'état, Dust (n° 2) pour l'agent nommé par tâche avec son résultat, Fin (n° 6) pour la démo en messages courts. Le journal horodaté de Well (n° 7, à côté) en donne une forme.
- Registre : outil précis. Elle met en avant la preuve « Vous validez, Ordo exécute » et le journal des actions.

### Direction retirée
- **C « Éditorial »** : retirée. Sa seule référence était la serif fine de Fin, alors que le brief impose Inter Tight ou Geist. Elle réduisait aussi la démo à un bloc parmi du texte, alors que la démo porte un indicateur (la part des visiteurs qui la voient jusqu'au bout) et deux preuves clés.

### 3 « à ne pas faire »
1. Pas de fond sombre, de halo violet, de cerveau ni de robot en 3D (n° 24, n° 10). Le brief demande un fond presque blanc et un ton sobre.
2. Pas de vert décoratif : il ne sert qu'à l'état « traité ». S'il apparaît dans les boutons, les icônes et les illustrations, il perd son sens.
3. Pas de deuxième animation forte (parallaxe, compteurs qui défilent, logos qui volent). La démo est la seule chose qui bouge vraiment.

---

## Palette, polices, design tokens, composants

Contrastes WCAG 2.1 calculés le 2026-11-12, puis recalculés lors de la refonte (mêmes valeurs). Cible : AA, soit 4,5:1 pour le texte et 3:1 pour les éléments d'interface.

### Palette

| Rôle | Hex | Usage |
|---|---|---|
| Fond | `#FAFAF7` | Fond principal, presque blanc et légèrement chaud |
| Surface | `#F1F2EE` | Cartes, panneaux de démo |
| Filet | `#E2E4DE` | Bordures décoratives, séparateurs |
| Encre | `#0E1A2E` | Titres et texte, bleu nuit (16,7:1 sur le fond) |
| Texte secondaire | `#4A5568` | Sous-titres, légendes (7,2:1 sur le fond, 6,7:1 sur la surface) |
| Accent « traité » | `#19E07A` | Pastilles, fonds d'état. Jamais pour du texte (1,7:1 sur le fond). Le mot « Traité » en encre sur la pastille : 9,9:1 |
| Accent texte | `#0B7A43` | Libellé « Traité » seulement : 5,2:1 sur le fond, 4,8:1 sur la surface, 4,9:1 sur `success.bg` |
| Alerte écart | `#C2410C` | Écart détecté dans la démo, avec parcimonie (5,0:1 sur le fond, 4,8:1 sur `warning.bg`) |

La palette suit le brief. Le risque de confusion avec le vert de Pennylane est tranché dans **Arbitrages**.

### Polices (Google Fonts)
- **Titres et texte** : Geist pour tout (titres en graisses 600 et 700, texte en 400), voir **Arbitrages**. **Corrigé** : le bench proposait Inter pour le texte courant, que le brief ne cite pas.
- **Chiffres et statuts** : Geist Mono, ou JetBrains Mono à défaut. Montants avec `font-variant-numeric: tabular-nums`.
- **Vu dans le panel** : Geist chez Dust (n° 2) et Factory (n° 11), Geist Mono chez Factory pour les statuts. Le choix est cohérent avec le secteur, mais peu distinctif : la mono et la mise en page « relevé » font la différence.

### Couleurs (tokens)

| Token | Hex | Usage |
|---|---|---|
| `color.brand.ink` | `#0E1A2E` | Encre principale, boutons primaires, anneau de focus |
| `color.brand.ink-hover` | `#1D2D4A` | Survol du bouton primaire |
| `color.brand.accent` | `#19E07A` | État « traité » : pastilles, fonds. Jamais pour du texte |
| `color.success.text` | `#0B7A43` | Libellé « Traité » seulement. **Corrigé** : n'est plus utilisé pour la validation du formulaire |
| `color.success.bg` | `#E6F9EF` | Fond de ligne « traitée » dans la démo. **Corrigé** : n'est plus le fond du message de succès du formulaire |
| `color.error.text` | `#B42318` | Erreurs de formulaire |
| `color.error.bg` | `#FEF0EE` | Fond des messages d'erreur |
| `color.warning.text` | `#C2410C` | Écart détecté (démo), alertes |
| `color.warning.bg` | `#FFF4E8` | Fond des alertes |
| `color.neutral.0` | `#FFFFFF` | Champs, cartes surélevées |
| `color.neutral.50` | `#FAFAF7` | Fond de page |
| `color.neutral.100` | `#F1F2EE` | Surfaces, panneau de démo, message de succès du formulaire |
| `color.neutral.200` | `#E2E4DE` | Filets, bordures décoratives |
| `color.neutral.400` | `#868B94` | **Ajouté** : bordure des champs de formulaire (3,4:1 sur blanc, 3,3:1 sur le fond) |
| `color.neutral.500` | `#6B7280` | Texte désactivé, placeholders (4,8:1 sur blanc, 4,6:1 sur le fond) |
| `color.neutral.700` | `#4A5568` | Texte secondaire |
| `color.neutral.900` | `#0E1A2E` | Texte principal (même valeur que `brand.ink`) |

| Paire | Ratio | Verdict |
|---|---|---|
| `neutral.900` sur `neutral.50` | 16,7:1 | AA |
| `neutral.900` sur `neutral.100` (message de succès) | 15,5:1 | AA |
| Blanc sur `brand.ink` (bouton) | 17,4:1 | AA |
| Blanc sur `brand.ink-hover` | 13,8:1 | AA |
| `neutral.700` sur `neutral.50` | 7,2:1 | AA |
| `success.text` sur `neutral.50` / `success.bg` | 5,2:1 / 4,9:1 | AA |
| `error.text` sur blanc / `error.bg` | 6,6:1 / 5,9:1 | AA |
| `warning.text` sur `neutral.50` / `warning.bg` | 5,0:1 / 4,8:1 | AA |
| `neutral.500` sur blanc | 4,8:1 | AA |
| `neutral.400` (bordure de champ) sur blanc / `neutral.50` | 3,4:1 / 3,3:1 | AA (élément d'interface) |
| `neutral.500` sur `neutral.200` (bouton désactivé) | 3,8:1 | Exempté (élément désactivé) |
| `brand.accent` sur `neutral.50` | 1,7:1 | Sous 3:1 : la pastille porte toujours le mot « Traité » en encre (9,9:1), l'état ne passe jamais par la couleur seule |
| `neutral.200` (filet) sur `neutral.50` | 1,2:1 | Décoratif uniquement |
| Anneau de focus d'origine (`rgba(14,26,46,.35)`) sur `neutral.50` | 2,2:1 | **Sous 3:1, corrigé** : contour plein `brand.ink` (16,7:1) |

### Typographie
Familles : `font.sans` = Geist (titres et texte) ; `font.mono` = Geist Mono. Chiffres : `font-variant-numeric: tabular-nums`.

| Token | Taille desktop / mobile | Graisse | Interligne | Usage |
|---|---|---|---|---|
| `type.display` | 64 / 40 px | 700 | 1.05 | Titre du hero |
| `type.h2` | 40 / 30 px | 650 | 1.15 | Titres de section |
| `type.h3` | 24 / 20 px | 600 | 1.25 | Cartes, étapes |
| `type.body-lg` | 20 / 18 px | 400 | 1.5 | Sous-titre du hero |
| `type.body` | 17 / 16 px | 400 | 1.6 | Texte courant |
| `type.small` | 14 px | 500 | 1.45 | Légendes, périmètres des chiffres |
| `type.stat` | 56 / 40 px (mono) | 500 | 1.0 | Chiffres héros |
| `type.mono-sm` | 13 px (mono) | 500 | 1.4 | Statuts, numéros de facture |

### Espacement (base 4 px)
`space.1` = 4, `space.2` = 8, `space.3` = 12, `space.4` = 16, `space.6` = 24, `space.8` = 32, `space.12` = 48, `space.16` = 64, `space.24` = 96, `space.32` = 128 px.
Sections : 128 px en desktop, 64 px en mobile. Marges latérales : 16 px en mobile. Conteneur max : 1200 px.

### Rayons
`radius.sm` = 6 px (pastilles, champs), `radius.md` = 10 px (boutons, cartes), `radius.lg` = 16 px (panneau de démo), `radius.full` = 999 px (badges d'état).

### Ombres et focus
`shadow.sm` = `0 1px 2px rgba(14,26,46,.06)` (cartes) ; `shadow.md` = `0 8px 24px rgba(14,26,46,.08)` (panneau de démo).
`focus.ring` = `outline: 2px solid #0E1A2E; outline-offset: 2px`. **Corrigé** : remplace `shadow.focus` (`0 0 0 3px rgba(14,26,46,.35)`), à 2,2:1 sur le fond. Le décalage de 2 px garde l'anneau visible autour du bouton encre.
Les ombres restent discrètes : on privilégie les filets.

### Motion
| Token | Valeur | Usage |
|---|---|---|
| `motion.duration.fast` | 120 ms | Survol, focus |
| `motion.duration.base` | 200 ms | Ouverture d'accordéon (FAQ), changement d'état |
| `motion.duration.slow` | 400 ms | Pastille « traité », surlignage de ligne dans la démo |
| `motion.ease.standard` | `cubic-bezier(.2,0,0,1)` | Défaut |
| `motion.ease.emphasis` | `cubic-bezier(.3,0,0,1.2)` | Pastille « traité » uniquement |

Avec `prefers-reduced-motion: reduce`, la démo passe en images fixes avec étapes numérotées, et les transitions sont réduites à 0 ms. La démo a toujours un bouton pause (brief, accessibilité).

### Composants clés

**Bouton primaire** : fond `brand.ink`, texte blanc, `radius.md`, hauteur 48 px (44 px minimum en mobile).
États : repos ; survol (`brand.ink-hover`) ; focus (`focus.ring`, toujours visible) ; actif (enfoncé de 1 px) ; désactivé (fond `neutral.200`, texte `neutral.500`) ; chargement (indicateur et libellé « Envoi… », bouton bloqué).

**Bouton secondaire** : fond transparent, bordure 1 px `neutral.200`, texte `brand.ink`. Mêmes états, avec un fond `neutral.100` au survol.

**Carte** (étape, témoignage, palier tarifaire) : fond `neutral.0`, bordure `neutral.200`, `radius.md`, padding `space.6`, `shadow.sm` facultative. Le palier mis en avant reçoit une bordure `brand.ink` de 2 px, pas de couleur vive.

**Formulaire de démo** : 4 champs, label visible au-dessus de chaque champ (jamais seulement un placeholder), hauteur 48 px, bordure `neutral.400`. Erreur sous le champ en `error.text`, avec une icône et `aria-describedby`. Succès dans un bloc `neutral.100` avec une bordure gauche `brand.ink` et une icône, texte en encre. **Corrigé** : le succès n'utilise plus le vert, réservé à l'état « traité ».

| À faire | À ne pas faire |
|---|---|
| Un seul bouton primaire par écran | Deux boutons primaires côte à côte |
| Libellés de CTA avec un verbe et un objet (« Réserver une démo de 20 min ») | « En savoir plus », « Cliquez ici » |
| Anneau de focus visible sur tous les éléments interactifs | `outline: none` sans remplacement |
| Vert uniquement pour l'état « traité » | Vert sur les boutons, les icônes, les illustrations ou les messages de formulaire |
| Chiffres en mono tabulaire, avec unité et périmètre | Compteurs animés qui défilent jusqu'au chiffre |
| Labels de champ toujours visibles | Placeholders utilisés comme labels |
| Messages d'erreur près du champ, qui disent comment corriger | « Erreur » seul en haut du formulaire |

---

## Arbitrages

- **Accent vert et Pennylane** : on garde `#19E07A`, réservé à la pastille « Traité » et jamais sur un bouton, parce que cette règle suffit à le distinguer du vert des boutons de Pennylane (`#00F872`, n° 25, à 1,22:1) et de la palette de Catalyze AI (n° 20). Dans la section intégrations, on ne pose aucune pastille « Traité » à côté du logo Pennylane.
- **Police** : on prend Geist pour les titres et le texte, avec Geist Mono pour les chiffres, parce qu'Inter Tight est dessinée serrée pour les grands corps et que Geist forme une famille avec la mono. Inter, que le brief ne cite pas, est écartée.
- **Barre fixe mobile** : on la fait, masquée quand le formulaire est à l'écran, parce que le brief la demande et qu'elle garde le CTA à portée de pouce sur une one-page longue. Le test de S3 vérifie seulement qu'elle ne gêne pas la lecture de la démo.
- **Titre sans chiffre** : le hero passe à l'option « Chaque facture rapprochée avec sa commande. Avant que vous la validiez. », parce que le chiffre héros de la version précédente était inventé. Ramp et Quid AI restent des inspirations pour la facture, pas pour le chiffre.
- **Prix** : Essentiel affiche « à partir de 99 € HT par mois », prix de démo calé sur le prix d'entrée public de Yooz. Équipe et Sur mesure affichent « Prix selon votre volume », parce qu'aucun repère public ne permet de fixer un deuxième prix sans l'inventer.
- **Sans photo** : le bloc « Qui sommes-nous » et les témoignages n'ont pas de photo (monogramme d'initiales pour les témoignages), parce qu'Unsplash et Pexels ont bloqué la recherche le 2026-11-13.

---

## À côté

| # | Référence | Capture | Pourquoi à côté |
|---|---|---|---|
| 3 | AI Workflow Landing Page, par Mao Lop, concept « Leap » (https://dribbble.com/shots/25092081-AI-Workflow-Landing-Page) | [capture](captures/a-cote/03-dribbble-leap.jpg) | Le visuel est un schéma de nœuds abstrait (Slack, extraction web, LLM), alors que le brief veut une démo « sur une facture anonymisée ». « 10x more efficient » est un chiffre sans périmètre (règle des allégations). Le seul détail propre, un mot en italique dans le titre, ne sert aucune exigence du brief. |
| 4 | « AI landing page website animation screens », Archon par Lazarev (épingle https://in.pinterest.com/pin/884746289449134596/ non vérifiée ; vu https://dribbble.com/shots/26000451-AI-Landing-page-website-animation-screens-Archon) | [capture](captures/a-cote/04-dribbble-archon.jpg) | Aplats saturés rouge `#DD1200`, orange et bleu, panneaux noirs à texte rose : contraire à la palette du brief (fond presque blanc, encre bleu nuit, un seul accent). L'épingle d'origine n'est pas vérifiée (mur de connexion). Détail cité dans **Preuves et témoignages**. |
| 5 | Operator, AI Agent Agency (https://land-book.com/websites/95503-operator-a-ai-agent-agency-custom-ai-agents-for-business) | Non vérifié | Non vérifié : Land-book bloque par Cloudflare, et la recherche « operator ai agent » sur la marketplace Framer ne le trouve pas. Factory (n° 11), vu, illustre la même discipline monochrome. |
| 7 | Well, AI Invoice Magnet (https://www.awwwards.com/sites/well-ai-invoice-magnet ; site actuel https://wellapp.ai/) | [Awwwards](captures/a-cote/07-awwwards-well.jpg) ; [site actuel](captures/a-cote/07-well-site.jpg) | Fond noir (`#101010` sur le site actuel, nuage de particules sur la version primée) : contraire au fond presque blanc du brief. Le produit est devenu un assistant généraliste sur WhatsApp, la facture n'est qu'une tâche parmi d'autres. Détail cité dans **Démo produit** (journal horodaté). |
| 9 | AI Automation SaaS Landing Page Design (https://www.behance.net/gallery/242896981/AI-Automation-SaaS-Landing-Page-Design) | Non vérifié | Non vérifié : Behance renvoie « HTTP ERROR 400 ». Remplacé par le n° 21. |
| 10 | Bubble Flow, AI automation landing page, Eslam (https://dribbble.com/shots/23013037-Bubble-Flow-Ai-automation-landing-page) | [capture](captures/a-cote/10-dribbble-bubble-flow.jpg) | Bulles 3D roses, violettes et bleues, fonds crème, bouton violet : contraire à la palette et au ton sobre du brief. Aucune frise en 3 étapes. L'auteur écrit lui-même que ce thème ne conviendrait pas à un service sérieux. |
| 13 | Dayos (https://saaslandingpage.com/dayos/) | [capture](captures/a-cote/13-saaslp-dayos.jpg) | Palette `#000000` et `#FFF200`, capitales condensées, et « WE'RE REVOLUTIONIZING » en grand : « révolutionner » est un mot interdit par le brief. Détail cité dans **Intégrations**. |
| 14 | Sections « stats » (https://land-book.com/sections/stats) | Non vérifié | Non vérifié : Land-book bloque par Cloudflare. Remplacé par le n° 26. |
| 16 | Loopra, CRM & AI Automation Website (https://www.behance.net/gallery/238403873/Loopra-CRM-AI-Automation-Website-UXUI-Design) | Non vérifié | Non vérifié : Behance renvoie « HTTP ERROR 400 ». Remplacé par le n° 25. |
| 17 | 11sight, B2B SaaS Platform, Lazarev (https://www.awwwards.com/sites/11sight-video-call-platform) | [capture](captures/a-cote/17-awwwards-11sight.jpg) | Fond noir et téléphone en 3D : contraire à la palette du brief et à la liste « à ne pas faire ». Plateforme d'appels vidéo, sans IA. URL morte : https://www.11sight.io/ introuvable le 2026-11-12. |
| 18 | AI Agent Landing Page & UI/UX Design, Romeo Saha (https://www.behance.net/gallery/236924567/AI-Agent-Landing-Page-UIUX-Design) | Non vérifié | Non vérifié : Behance renvoie « HTTP ERROR 400 ». D'après sa description, mode sombre « futuriste » : contre-exemple. Remplacé par le n° 24. |
| 19 | Idées « SaaS Landing Page UI Design » (https://www.pinterest.com/ideas/saas-landing-page-ui-design/902357840411/) | Non vérifié | Non vérifié : mur de connexion. Derrière la fenêtre, les vignettes visibles sont surtout claires, bleues et violettes. Le « vert et noir » annoncé n'y apparaît pas. |
| 24 | Open source ai agents landing page, FANCY (https://dribbble.com/shots/27029567-Open-source-ai-agents-landing-page-web-design-3d-animation) | [capture](captures/a-cote/24-dribbble-contre-exemple.jpg) | Contre-exemple. Fond noir, cubes-robots 3D aux yeux vert néon, palette `#020503` et `#3DAA53` : contraire au fond presque blanc, au vert réservé à « traité » et à la liste « à ne pas faire ». Sur 11 vignettes « ai agent landing page », 4 montrent un robot ou un objet 3D. |

---

## Galeries : requêtes lancées

| Plateforme | Requêtes | Résultat |
|---|---|---|
| Behance | liens d'origine n° 9, 16, 18 | Inaccessible : « HTTP ERROR 400 » au navigateur automatisé. |
| Dribbble | « invoice automation landing page », « ai agent landing page », « archon lazarev » | 4 retenues (n° 21 à 24) et l'équivalent du n° 4. Les maquettes de compta fournisseurs sont presque toutes claires, avec un tableau de factures. Les maquettes « agent IA » sont environ pour moitié sombres. |
| Dribbble (refonte) | « invoice pricing » | Page « Let's confirm you are human » (HTTP 405). Non contournée, rien vu. |
| Pinterest | liens d'origine n° 4, 19 | Mur de connexion sur les deux. Aucune capture. |
| Awwwards | liens d'origine n° 7, 17, 20 | 3 vues. Deux sites primés ont changé ou disparu depuis (Well, 11sight). |
| Land-book | liens d'origine n° 5, 14 | Inaccessible (challenge Cloudflare). |
| Lapa Ninja | liens d'origine n° 6, 11 | Inaccessible (« Sorry, you have been blocked »). Sites réels vus à la place. |
| One Page Love | liens d'origine n° 8, 15 ; sections « Metrics » et « How It Works » | 3 retenues (n° 8, 15, 26). « How It Works » vue, rien de retenu : aucun exemple B2B ou finance en tête de liste. |
| One Page Love (refonte) | sections « Pricing », « Pricing Table », « Pricing Slider », « Contact Form », « FAQ Accordion » | Rien retenu. Tarifs : festival (Kelvin), apps (Pairio, Mappy), agences (Diligent flow sur fond sombre, OhhMyDesign, Flowjam). Formulaires et FAQ : agences et sites sur fond sombre (Flashform, vert acide sur quasi-noir). Aucun palier par volume ni formulaire B2B à 4 champs. |
| Framer Marketplace | « operator ai agent » | Le template Operator (n° 5) n'apparaît pas. |
