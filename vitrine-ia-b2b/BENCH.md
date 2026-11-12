# Benchmark visuel : Ordo (IA B2B, entreprise fictive)

## Limites, à lire en premier

Mise à jour du 2026-11-12, faite avec un vrai navigateur (Chrome piloté par Playwright).

- **Ce qui a été vu** : 14 des 20 références d'origine ont été ouvertes et capturées, dont 11 sur leur lien d'origine. Pour 3 autres, le lien d'origine était bloqué et une page équivalente a été ouverte à la place : le site réel de Fin (n° 6) et de Factory (n° 11), le shot Dribbble d'Archon (n° 4). 6 références ont été ajoutées (n° 21 à 26). Captures en 1440 × 900 px, au-dessus de la ligne de flottaison, dans [`captures/`](captures/), plus 2 captures complémentaires (site actuel de Well au n° 7, page de Ramp au n° 12) et 4 captures mobiles. Les couleurs et les polices citées ont été relevées dans la page (`getComputedStyle`), pas devinées. Les chiffres cités sont ceux affichés le 2026-11-12.
- **Ce qui reste bloqué** : Behance (n° 9, 16, 18) renvoie « HTTP ERROR 400 » au navigateur automatisé. Land-book (n° 5, 14) et Lapa Ninja (n° 6, 11) bloquent par Cloudflare. Pinterest (n° 4, 19) affiche un mur de connexion : rien n'a été capturé (pas de page de connexion dans le dépôt). Ces références gardent leur texte, marqué « non vérifié ».
- **Corrections importantes** :
  - **Well (n° 7)**, présentée comme « la référence la plus proche », a changé de produit : le site actuel est un assistant généraliste sur WhatsApp, sur fond noir. La facture n'y est plus qu'une tâche parmi d'autres.
  - **Bubble Flow (n° 10)** ne montre aucune frise en 3 étapes : c'est un concept à bulles 3D roses et violettes. Il passe en contre-exemple.
  - **Ramp (n° 1)** ne nomme pas quatre agents sur sa page : elle parle de « Ramp's agent », au singulier. Les agents nommés par tâche se voient chez Dust (n° 2).
  - **Fin (n° 6)** : l'exemple du hero est un changement d'adresse avec un justificatif PDF, pas un remboursement.
  - **11sight (n° 17)** : l'aperçu primé est un téléphone 3D sur fond noir, pas un SaaS sobre, et le site ne répond plus.
  - **Quid AI (n° 15)** est la vraie référence la plus proche : une facture au centre du hero, des agents pour la compta fournisseurs, un bloc « pas d'entraînement sur vos données ». Le site est hors ligne, One Page Love en garde une copie.
- **Palette** : l'accent d'Ordo (`#19E07A`) est presque identique au vert des boutons de Pennylane (`#00F872`) et au vert de Catalyze AI (`#1AD079`, n° 20). La palette n'est pas changée (le brief impose un vert électrique), mais le point est à trancher avec Ordo. Voir la synthèse.
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

## Hero

| # | Référence | URL | Source | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 1 | Ramp, page Accounts Payable | https://ramp.com/accounts-payable | Site réel (États-Unis) | [capture](captures/01-ramp-ap.jpg) | Fond blanc, titre « A month of AP done in minutes. » en Lausanne 64 px, graisse 400, encre `#0C0A08`. Bouton jaune-vert `#E4F222` à texte noir (16:1). À droite, une animation « Routing to approvals. » fait défiler de vraies lignes de factures (fournisseur, montant, date, numéro). Chiffres confirmés : « 2.4x faster » dans le sous-titre, « 85,000+ businesses », puis plus bas « Up to 7x fewer clicks to process a bill vs Bill.com », « Up to 95% », OCR « 99% accuracy ». Chaque chiffre porte un renvoi numéroté (1, 2, 3). **Correction** : la page ne nomme pas quatre agents. Elle parle de « Ramp's agent », qui impute, vérifie par rapprochement à deux et trois voies, recommande les validations et repère les fournisseurs payables par carte. Les quatre agents viennent de l'annonce d'octobre 2025 citée dans l'étude de cas. **À reprendre** : de vraies lignes de factures dans le hero, et le renvoi numéroté sous chaque chiffre, qui sert de ligne de périmètre. **À éviter** : le jaune fluo. |
| 2 | Dust | https://dust.tt | Site réel (France, site en anglais) | [capture](captures/02-dust.jpg) | Fond blanc, titre « Multiplayer AI for human-agent collaboration » en Geist 69 px, graisse 550, encre `#191715`, texte `#57534D`. Bouton bleu en dégradé `#4BABFF` vers `#1C91FF`, texte blanc à 3,2:1 au mieux, sous le seuil AA. Le visuel est une scène isométrique avec des avatars et des bulles d'agents nommés par tâche (@LeadQual, @Incident, @TicketRouter), chacune montrant un résultat. Confirmé : « Trusted by teams at 3,000+ global organizations », menu « Solutions » classé par équipe (Sales, Support, Marketing…) et par secteur. La page annonce « 70+ connectors ». Un encart d'événement a été fermé avant la capture. **À reprendre** : nommer chaque agent par sa tâche et montrer son résultat dans une bulle (pour Ordo : « Lecture », « Rapprochement », « Relance »). **À éviter** : la scène 3D isométrique. |
| 3 | AI Workflow Landing Page, par Mao Lop | https://dribbble.com/shots/25092081-AI-Workflow-Landing-Page | Dribbble | [capture](captures/03-dribbble-leap.jpg) | Concept pour « Leap ». Fond blanc, titre « Automate any workflow with AI » avec le seul mot « workflow » en italique, sous-titre « 10x more efficient », boutons noirs. À droite, un schéma de nœuds dans un cadre (déclencheur Slack, extraction web, LLM, Typefully). La description promet « 5x your velocity ». **À reprendre** : un seul mot en italique dans le titre. **À éviter** : le schéma abstrait. Pour Ordo, la facture elle-même le remplace, comme chez Quid AI (n° 15). |
| 4 | « AI landing page website animation screens » (Archon, par Lazarev) | Épingle d'origine : https://in.pinterest.com/pin/884746289449134596/ (non vérifiée : mur de connexion). Vu à la place : https://dribbble.com/shots/26000451-AI-Landing-page-website-animation-screens-Archon | Pinterest, puis Dribbble (shot d'origine du même studio) | [capture](captures/04-dribbble-archon.jpg) | Même titre que l'épingle. C'est une animation qui fait défiler les écrans du site d'Archon (mise en conformité FedRAMP pour vendre du logiciel au gouvernement américain). Palette relevée sur Dribbble : rouge `#DD1200`, noir `#080607`. Panneaux noirs à texte rose, aplats orange et bleus. **Correction** : ce n'est pas un enchaînement hero puis démo, c'est une vitrine d'écrans. Et ce n'est pas « minimaliste » au sens clair : les blocs sont pleins et saturés. **À reprendre** : la grande phrase qui contient un chiffre (« 20% of the U.S. software market ») en guise d'intertitre. **À éviter** : les aplats saturés. |
| 5 | Operator, AI Agent Agency | https://land-book.com/websites/95503-operator-a-ai-agent-agency-custom-ai-agents-for-business | Land-book (template Framer) | Non vérifié | **Non vérifié** : Land-book bloque par Cloudflare, et la recherche « operator ai agent » sur la marketplace Framer ne le trouve pas. Texte d'origine, d'après la fiche : noir et blanc strict, grosse typo en pied de page. **À reprendre** : la discipline monochrome, qui laisse la place au seul accent vert. Factory (n° 11), vu, illustre la même discipline sur fond clair. |

## Démo produit

| # | Référence | URL | Source | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 6 | Fin, agent de service client | Fiche d'origine : https://www.lapa.ninja/post/fin-ai/ (non vérifiée : Cloudflare). Vu à la place : https://fin.ai/ | Lapa Ninja, puis site réel | [capture](captures/06-fin.jpg) | Titre en serif fine (« Serrif », 72 px, graisse 300), texte en Saans, tube 3D orange en fond. Bouton noir « View demo ». Chiffres : « 76% resolution rate, across 12,000+ businesses ». Le logo porte « from salesforce ». La démo est une conversation : le client signale un déménagement, Fin demande un justificatif, le PDF « UtilityBill.pdf » arrive, Fin confirme la nouvelle adresse. **Correction** : l'exemple n'est ni un remboursement ni une annulation. L'idée tient : l'agent termine une tâche à partir d'une pièce jointe. L'agent d'exploitation porte un nom, « Operator ». **À reprendre** : la démo en messages courts, avec un PDF qui arrive puis une confirmation. Pour Ordo : facture reçue, « rapprochée avec la commande », pastille « Traité ». **À éviter** : l'objet 3D décoratif. |
| 7 | Well, AI Invoice Magnet | https://www.awwwards.com/sites/well-ai-invoice-magnet | Awwwards (mention honorable, 19 mai 2025) | [capture](captures/07-awwwards-well.jpg) ; [site actuel](captures/07-well-site.jpg) | Version primée : fond noir, nuage de particules gris, bouton « Start collecting », compteur GitHub. Catégorie Awwwards « Business & Corporate », pas comptabilité. **Correction majeure** : le site actuel (https://wellapp.ai/) a changé de produit. Titre « Sharper founders, side quests handled », assistant généraliste sur WhatsApp, fond `#101010`, Inter 72 px graisse 500, photos noir et blanc d'un modèle. La facture n'est plus qu'une tâche parmi d'autres (billets de concert, prospects). Plus bas, un journal horodaté : « 10:40 Hexa Cloud invoice fetched and filed », « 14:20 Copyhaus receipt matched to the card payment ». **À reprendre** : le journal horodaté, pour la direction B. **À éviter** : le fond noir. Ce n'est plus la référence la plus proche : c'est Quid AI (n° 15). |
| 8 | invoicemon | https://onepagelove.com/invoicemon | One Page Love (publié le 17 juin 2026) | [capture](captures/08-onepagelove-invoicemon.jpg) | Confirmé. La fiche parle d'une « scroll-to-demo interactive experience », tags « In-Page Demo » et « Interactive », police Inter, tons beige. Sur le site (https://invoicemon.com/), sous le titre « A complete invoicing workflow in your browser » (Inter 36 px, graisse 600, encre `#1A1816`), l'éditeur de facture complet est utilisable dans la page : lignes, quantités, totaux. Ce n'est pas un agent IA mais un générateur de factures. **À reprendre** en phase 2 : une démo jouable sur une facture d'exemple, plutôt qu'une simple vidéo. |
| 9 | AI Automation SaaS Landing Page Design | https://www.behance.net/gallery/242896981/AI-Automation-SaaS-Landing-Page-Design | Behance | Non vérifié | **Non vérifié** : Behance renvoie une erreur 400. Texte d'origine, d'après la description : étude de cas complète, utile pour la structure « comment ça marche » et « démo ». Remplacée par le n° 21, vu, qui couvre ces deux sections sur le même sujet (comptabilité fournisseurs). |

## Comment ça marche / flux

| # | Référence | URL | Source | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 10 | Bubble Flow, AI automation landing page (Eslam) | https://dribbble.com/shots/23013037-Bubble-Flow-Ai-automation-landing-page | Dribbble | [capture](captures/10-dribbble-bubble-flow.jpg) | **Correction** : aucune frise en 3 étapes n'apparaît dans le shot. C'est un concept très coloré : bulles 3D roses, violettes et bleues, fonds crème, gribouillis violets, titres dans une police arrondie, bouton violet. L'auteur écrit lui-même qu'il pensait que ce thème coloré ne conviendrait pas à un service sérieux. **Contre-exemple** pour Ordo (décor 3D, violet). Pour la frise, voir les n° 21 et 23. |
| 11 | Factory | Fiche d'origine : https://www.lapa.ninja/post/factory/ (non vérifiée : Cloudflare). Vu à la place : https://factory.ai/, qui redirige vers https://factory.com/ | Lapa Ninja, puis site réel | [capture](captures/11-factory.jpg) | Fond `#F9F9F9`, titre en capitales « AI CODING AGENTS FOR THE ENTERPRISE » en Geist 60 px, graisse 500. Sous-titre, boutons et commande `curl` en Geist Mono. Plus bas, l'interface en sombre : liste de sessions avec une pastille orange d'état. Confirmé : la mono porte les statuts et les commandes. C'est exactement le couple Geist et Geist Mono des tokens d'Ordo. **À reprendre** : la mono pour les statuts et les numéros. **À éviter** : la mono gris clair `#8A8380` pour du texte (3,5:1, sous AA). |

## Intégrations

| # | Référence | URL | Source | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 12 | 15 Outstanding Integration Page Examples (page intégrations de Ramp) | https://saaslandingpage.com/articles/15-outstanding-integration-page-examples/ | SaaS Landing Page (article publié le 27 décembre 2023, mis à jour le 23 octobre 2026) | [capture](captures/12-saaslp-integrations.jpg) ; [Ramp](captures/12b-saaslp-ramp-integrations.jpg) | Ramp est le n° 6 de l'article. La capture montre « Explore Integrations », un champ de recherche, des filtres par catégorie (Accounting, Expense Automation, HR and payroll, Procurement…), « 123 Integrations », puis une grille logo, nom et catégorie (Xero, NetSuite, Sage Intacct, QuickBooks). L'article cite aussi Resend (n° 7) : un annuaire en trois parties, apps disponibles, à venir et sur mesure. C'est la réponse au brief, qui veut des « connecteurs en cours, marqués comme tels ». **À reprendre** : 3 logos en grand (Pennylane, Sage, Qonto), puis une liste avec catégorie et un groupe « bientôt disponible ». |
| 13 | Dayos | https://saaslandingpage.com/dayos/ | SaaS Landing Page (septembre 2025) | [capture](captures/13-saaslp-dayos.jpg) | Fiche : police Suisse Int'l, palette `#000000` et `#FFF200`. Hero en capitales condensées « AGENTIC COPILOT FOR YOUR ENTERPRISE », à côté d'une colonne de blocs 3D empilés aux logos de Workday et ServiceNow. Confirmé : l'agent est montré comme une couche posée sur les logiciels existants. Plus bas, « WE'RE REVOLUTIONIZING » en grand. **À reprendre** : les logos des outils existants dans le visuel principal. **À éviter** : le jaune, les capitales condensées et le mot « revolutionizing », interdit dans le brief. |

## Preuves et chiffres

| # | Référence | URL | Source | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 14 | Sections « stats » | https://land-book.com/sections/stats | Land-book (galerie de sections) | Non vérifié | **Non vérifié** : Land-book bloque par Cloudflare. Remplacé par le n° 26, la galerie « Metrics » de One Page Love, vue. |
| 15 | Quid AI | https://onepagelove.com/quid-ai | One Page Love (publié le 23 septembre 2025) | [capture](captures/15-onepagelove-quid-ai.jpg) | **La référence la plus proche d'Ordo.** Le site est hors ligne, One Page Love garde une copie (https://onepagelove.com/preserved/2025-09-23-quid-ai.html), ouverte. Titre « AI agents for your AP/AR workflows » en Space Grotesk 60 px, graisse 500, encre `#190806`, la fin surlignée en rose pâle. Le visuel est une facture au centre, avec les champs extraits en étiquettes (centre de coût, numéro, compte général), les sources à gauche (Office, Slack, Gmail, Stripe) et les logiciels comptables à droite (DATEV, LexOffice, NetSuite, Sage). Ensuite : logos clients, AP puis AR, alertes Slack, un chat (« approve all invoices under €500 from this vendor »), un témoignage de CFO, les intégrations, un bloc sécurité en 3 points (RGPD, « Your data will not be used to train AI models available publicly », chiffrement), une FAQ. Pas de tarifs. Bouton `#F94B38` à texte blanc : 3,45:1, sous AA. **À reprendre** : la facture au centre entre sources et logiciels, et le bloc sécurité en 3 points avec la phrase sur l'entraînement. **À éviter** : le bouton rouge-orangé sous le seuil. |

## Sobriété B2B et sécurité

| # | Référence | URL | Source | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 16 | Loopra, CRM & AI Automation Website | https://www.behance.net/gallery/238403873/Loopra-CRM-AI-Automation-Website-UXUI-Design | Behance (novembre 2025) | Non vérifié | **Non vérifié** : erreur 400. Texte d'origine, d'après la description : « communication produit claire et navigation structurée pour une audience B2B ». Remplacé par le n° 25 (Pennylane), un vrai site B2B français vu. |
| 17 | 11sight, B2B SaaS Platform (Lazarev) | https://www.awwwards.com/sites/11sight-video-call-platform | Awwwards (mention honorable, 7 juillet 2022) | [capture](captures/17-awwwards-11sight.jpg) | Plateforme d'appels vidéo entrants, pas d'IA. Palette de la fiche : `#49C5B6` et blanc, tags « Clean », « Parallax », « Data Visualization ». **Correction** : l'aperçu primé est un fond noir avec un téléphone en 3D et une courbe verte, pas un hero sobre. Le site (https://www.11sight.io/) ne répond plus : nom de domaine introuvable le 2026-11-12. Référence faible, à retirer du moodboard. |

## Palette, typo et contre-exemples

| # | Référence | URL | Source | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 18 | AI Agent Landing Page & UI/UX Design, par Romeo Saha | https://www.behance.net/gallery/236924567/AI-Agent-Landing-Page-UIUX-Design | Behance | Non vérifié | **Non vérifié** : erreur 400. Texte d'origine : **contre-exemple**, mode sombre « futuriste », réalisé avec Midjourney et After Effects. Remplacé par le n° 24, vu. |
| 19 | Idées « SaaS Landing Page UI Design » | https://www.pinterest.com/ideas/saas-landing-page-ui-design/902357840411/ | Pinterest (page d'idées) | Non vérifié | **Non vérifié** : mur de connexion, pas de capture. Derrière la fenêtre, les vignettes visibles sont surtout claires, bleues et violettes, une seule est sombre. **Correction** : le « vert et noir » annoncé n'apparaît pas dans cette partie visible. Sur Dribbble, la recherche « ai agent landing page » donne environ 5 vignettes sombres sur 11, dont 2 en vert néon. Le vert vif dosé sur fond clair se voit en revanche chez Pennylane (n° 25). |
| 20 | Catalyze AI, SaaS website (Halo Lab) | https://www.awwwards.com/sites/catalyze-ai-saas-website | Awwwards (mention honorable, 17 mars 2023) | [capture](captures/20-awwwards-catalyze.jpg) | Palette de la fiche : marine `#07133B` et vert `#1AD079`. Le site (https://catalyzeai.webflow.io/) est en ligne : fond `#F8F9FB`, encre `#07133B`, titre en Hellix 58 px, graisse 600, texte en Poppins, 3 chiffres sous le hero (400mm+, $3Tn, $77Bn). Les liens « Sign up » et « Log in » sont en vert sur fond clair : 1,9:1. **Observation clé** : c'est presque la palette d'Ordo (encre `#0E1A2E`, accent `#19E07A`), primée dès 2023. **À éviter** : le vert en texte, que les tokens d'Ordo interdisent déjà. |

---

## Références ajoutées (vues le 2026-11-12)

Elles remplacent les références bloquées ou fausses, sur le même rôle. Les numéros suivent ceux du bench.

| # | Référence | URL | Source | Capture | Ce qu'on retient |
|---|---|---|---|---|---|
| 21 | Accounts Payable Automation SaaS Website (Agemandi) | https://dribbble.com/shots/27640668-Accounts-Payable-Automation-SaaS-Website | Dribbble | [capture](captures/21-dribbble-ap-automation.jpg) | Remplace les n° 9 et 10. Hero « AI-powered Accounts Payable. » au-dessus d'un tableau de bord (liste des factures fournisseurs, statuts). Puis une frise à onglets numérotés : 01 Capture, 02 Extract & store, 03 Recognise, 04 Auto-match, 05 Approve & pay, avec un panneau marine par étape. Un bloc auditabilité affiche « 10 years » de conservation des pièces. La description dit ouvrir « with a product dashboard rather than an abstract promise about AI ». **À reprendre** : la frise à onglets numérotés, un panneau par étape (3 chez Ordo), et le bloc piste d'audit pour Claire, la DAF. **À éviter** : la photo de banque d'images et le bleu-violet `#354AEA`. |
| 22 | Landing Page for Invoice Management platform (Nadia Kapyrina, pour Numira) | https://dribbble.com/shots/27166316-Landing-Page-for-Invoice-Management-platform | Dribbble | [capture](captures/22-dribbble-numira.jpg) | Palette publiée : `#F2F6F7`, `#010F14`, `#B1D9D0`, `#263B4A`. Grand aplat sarcelle foncé, page blanche, et au centre un tableau de factures (fournisseur, montant, date, pièce, statut). Sections « Collect Documents from Anywhere » et « Simple Pricing That Fits Any Team ». La description vise un « calm tone », sans page « heavy or technical ». **À reprendre** : le tableau de factures comme visuel principal, c'est la direction A. |
| 23 | Remittance Reconciliation Software Website Design (Crevio, pour FiscalPro) | https://dribbble.com/shots/27821027-Remittance-Reconciliation-Software-Website-Design | Dribbble (studio Crevio) | [capture](captures/23-dribbble-fiscalpro.jpg) | Titre « Reconcile PDF Remittance Advice in Xero. Instantly. » : l'outil comptable est nommé dans le titre. Au-dessus du tableau de bord, 4 pastilles d'étape (Upload a file, Review, Reconcile, Completion), et des statuts « Paid » en vert, « Pending » en orange. **À reprendre** : nommer les outils dans le titre ou le sous-titre (« dans Pennylane, Sage ou Qonto », déjà dans le brief) et des étapes en pastilles. **À éviter** : le fond photo de fleurs floues. |
| 24 | Open source ai agents landing page (FANCY) | https://dribbble.com/shots/27029567-Open-source-ai-agents-landing-page-web-design-3d-animation | Dribbble (studio FANCY) | [capture](captures/24-dribbble-contre-exemple.jpg) | **Contre-exemple**, remplace le n° 18. Fond noir, cubes-robots 3D argentés aux yeux vert néon sur un tapis lumineux, palette `#020503` et `#3DAA53`. Tout ce que la liste « à ne pas faire » interdit. Il représente bien la recherche : sur 11 vignettes « ai agent landing page », 4 montrent un robot ou un objet 3D. |
| 25 | Pennylane | https://www.pennylane.com/fr | Site réel (France) | [capture](captures/25-pennylane.jpg) | Remplace le n° 16. Fond blanc, encre sarcelle `#003D3D`, titre en Manrope 52 px, graisse 600. Bouton vert électrique `#00F872` à texte `#003D3D` (8,5:1). Onglets d'audience au-dessus de l'en-tête : « Indépendants et TPE », « PME et ETI », « Cabinet expertise comptable ». Preuves : « +1 500 000 dirigeants… », « +300 intégrations », ISO/IEC 27001, « Made in France », bloc « Plateforme Agréée immatriculée » pour la facture électronique. **Observation clé** : ce vert et l'accent d'Ordo sont presque identiques (1,22:1 entre eux). Ordo se branche sur Pennylane : risque d'être pris pour un module Pennylane. **À reprendre** : l'onglet « Cabinet expertise comptable » pour le persona Sophie, et les preuves de conformité en ligne courte. |
| 26 | Metrics Section Examples | https://onepagelove.com/section/metrics | One Page Love (galerie de 150 sections) | [capture](captures/26-onepagelove-metrics.jpg) | Remplace le n° 14. Kelvin : 4 chiffres sur une ligne, sous un filet, avec un libellé en petites capitales. The Queue : 3 pourcentages, chacun avec une ligne d'explication dessous. Confirme le format « grand chiffre, unité, ligne de périmètre ». Aucun des exemples vus n'utilise la mono : c'est un choix propre à Ordo. |

### Galeries : requêtes lancées

| Plateforme | Requêtes | Résultat |
|---|---|---|
| Behance | liens d'origine n° 9, 16, 18 | Inaccessible : « HTTP ERROR 400 » au navigateur automatisé. |
| Dribbble | « invoice automation landing page », « ai agent landing page », « archon lazarev » | 4 retenues (n° 21 à 24) et l'équivalent du n° 4. Les maquettes de compta fournisseurs sont presque toutes claires, avec un tableau de factures. Les maquettes « agent IA » sont environ pour moitié sombres. |
| Pinterest | liens d'origine n° 4, 19 | Mur de connexion sur les deux. Aucune capture. |
| Awwwards | liens d'origine n° 7, 17, 20 | 3 vues. Deux sites primés ont changé ou disparu depuis (Well, 11sight). |
| Land-book | liens d'origine n° 5, 14 | Inaccessible (challenge Cloudflare). |
| Lapa Ninja | liens d'origine n° 6, 11 | Inaccessible (« Sorry, you have been blocked »). Sites réels vus à la place. |
| One Page Love | liens d'origine n° 8, 15 ; sections « Metrics » et « How It Works » | 3 retenues (n° 8, 15, 26). « How It Works » vue, rien de retenu : aucun exemple B2B ou finance en tête de liste. |
| Framer Marketplace | « operator ai agent » | Le template Operator (n° 5) n'apparaît pas. |

---

## Mobile

Trois sites vus en 390 × 844 px :

| Site | Capture | Ce qu'on observe |
|---|---|---|
| Ramp, Accounts Payable | [hero](captures/mobile-ramp.jpg) ; [démo facture](captures/mobile-ramp-facture.jpg) | Titre centré, champ e-mail et bouton jaune en pleine largeur, puis l'animation de factures empilée dessous, dans une carte grise. Plus bas, une facture se remplit ligne par ligne (« Draft Invoice #CI-14884 », catégorie, département, lieu), avec les états « Auto coding… » puis « Checking for discrepancies… ». Seul l'en-tête est fixe : aucun bouton fixe en bas. |
| Fin | [capture](captures/mobile-fin.jpg) | Le bouton noir « Contact sales » reste dans l'en-tête fixe, en haut. La démo en conversation passe sous les boutons, au format vertical, sans adaptation particulière. Aucun élément fixe en bas. |
| Pennylane | [capture](captures/mobile-pennylane.jpg) | Les onglets d'audience défilent horizontalement en haut. L'en-tête reste collé en haut, mais sans bouton : seulement le logo et le menu. Le bouton vert est dans le hero, pas fixe. La photo d'écran de bureau n'est pas recadrée pour le mobile. |

Ce que ces observations changent pour Ordo :
- **Démo verticale** : confirmée. Ramp montre qu'une facture tient en largeur mobile si on garde 3 colonnes courtes par ligne. C'est le modèle de la démo d'Ordo : une facture qui se remplit, puis l'état « Traité ».
- **CTA fixe** : aucun des 3 sites n'a de barre fixe en bas. Fin garde son CTA dans l'en-tête fixe. La barre « Réserver une démo » en bas du brief reste un choix d'Ordo, non observé dans le panel. Elle doit se masquer quand le formulaire est à l'écran, pour ne pas le doubler.
- **Défilement horizontal** : vu chez Pennylane pour les onglets d'audience, pas pour les logos. Les logos d'intégration en défilement horizontal restent une proposition non vérifiée.
- **Visuels** : éviter la capture d'écran desktop réduite (Pennylane). Prévoir un visuel recadré pour le mobile.

---

## Synthèse du moodboard

### Ajustements après observation (2026-11-12)
- **Direction A renforcée** : les trois exemples les plus proches du sujet mettent la facture ou le tableau de factures au centre. Quid AI (n° 15) en hero, Ramp (n° 1) dans son animation et sa démo mobile, Numira (n° 22) en visuel principal. La recommandation est maintenue, avec ces preuves en plus. Well, citée avant comme modèle, ne l'est plus (n° 7).
- **Agents nommés** : l'idée vient de Dust (n° 2) et de Fin (« Operator », n° 6), pas de la page de Ramp. Elle reste valable pour Ordo.
- **Frise** : Bubble Flow (n° 10) est retiré au profit d'Agemandi (n° 21, 5 onglets numérotés) et de FiscalPro (n° 23, 4 pastilles).
- **Boutons** : deux sites du panel ont un bouton principal sous le seuil AA (Dust 3,2:1, Quid AI 3,45:1). Le bouton encre d'Ordo est à 17,4:1 : à garder.
- **Palette** : non changée, voir ci-dessous.

### Direction A : « Relevé comptable »
- Fond presque blanc, filets fins, grille de tableau visible, chiffres en mono.
- La démo ressemble à un vrai document : la facture se surligne ligne par ligne, et une pastille verte « Traité » apparaît à la fin.
- Références vues : Quid AI (n° 15) pour la facture entre sources et logiciels, Ramp mobile pour la facture qui se remplit ligne par ligne, Numira (n° 22) pour le tableau.
- Registre : sérieux, vérifiable, rassurant pour une DAF. **C'est la direction recommandée.**

### Direction B : « Console calme »
- Interface produit en très grand (n° 1, 11), avec des panneaux gris clair et un journal d'actions de l'agent en mono.
- Le hero est une capture recadrée sur l'action de l'agent (« Relance envoyée à Fournisseur X »).
- Références vues : Factory (n° 11) pour la mono et les pastilles d'état, le journal horodaté de Well (n° 7).
- Registre : outil puissant, plus tech, adapté si la cible glisse vers les ETI.

### Direction C : « Éditorial »
- Grand titre serré en Inter Tight, beaucoup de blanc, peu de visuels, chiffres héros en très grand corps.
- La démo est un bloc unique, centré, avec du texte autour comme dans un article.
- Référence vue : Fin (n° 6), titre en serif fine et démo en conversation à côté.
- Registre : premium et calme, idéal pour la relation investisseurs. Moins démonstratif pour les PME.

### Palette recommandée

Contrastes WCAG 2.1 calculés le 2026-11-12.

| Rôle | Hex | Usage |
|---|---|---|
| Fond | `#FAFAF7` | Fond principal, presque blanc et légèrement chaud |
| Surface | `#F1F2EE` | Cartes, panneaux de démo |
| Filet | `#E2E4DE` | Bordures, séparateurs |
| Encre | `#0E1A2E` | Titres et texte, bleu nuit (16,7:1 sur le fond) |
| Texte secondaire | `#4A5568` | Sous-titres, légendes (7,2:1 sur le fond, 6,7:1 sur la surface) |
| Accent « traité » | `#19E07A` | Pastilles, fonds d'état. Jamais pour du texte sur fond clair (1,7:1 sur le fond). Le mot « Traité » en encre sur la pastille : 9,9:1 |
| Accent texte | `#0B7A43` | Vert foncé pour le texte « Traité » : 5,2:1 sur le fond, 4,8:1 sur la surface, 4,9:1 sur `success.bg`. Conforme AA |
| Alerte écart | `#C2410C` | Écart détecté dans la démo, avec parcimonie (5,0:1 sur le fond, 4,8:1 sur `warning.bg`) |

**Pourquoi la palette ne change pas, et ce qu'il faut trancher.** Deux observations touchent l'accent vert. Pennylane (n° 25) met un vert presque identique (`#00F872`) sur tous ses boutons, et Ordo se branche sur Pennylane. Catalyze AI (n° 20) avait dès 2023 une palette marine et vert très proche (`#07133B`, `#1AD079`). Le brief impose pourtant un vert électrique, et la règle d'Ordo (vert seulement pour l'état « traité », jamais sur un bouton) le distingue déjà de ces deux sites, qui mettent le vert sur leurs boutons ou leurs liens. La palette reste donc telle quelle. **À valider avec Ordo** : voir la pastille « Traité » à côté du logo Pennylane dans la section intégrations. Si elle se confond, décaler l'accent plutôt que de le mettre sur les boutons.

### Polices (Google Fonts)
- **Titres et texte** : Inter Tight (titres, graisses 600 et 700) et Inter (texte courant), ou Geist, qui est aussi disponible sur Google Fonts.
- **Chiffres et statuts** : Geist Mono, ou JetBrains Mono à défaut. Montants avec `font-variant-numeric: tabular-nums`.
- **Vu dans le panel** : Geist chez Dust (n° 2) et Factory (n° 11), Geist Mono chez Factory pour les statuts et les commandes. Le choix est cohérent avec le secteur, mais peu distinctif : c'est le rôle de la mono et de la mise en page « relevé » de faire la différence.

### 3 « à ne pas faire »
1. Pas de fond sombre, de halo violet ni de cerveau ou de robot en 3D (n° 24, et n° 10 pour les bulles 3D). C'est le code d'une bonne part du secteur, et il contredit le registre comptable.
2. Pas de vert décoratif : il ne sert qu'à l'état « traité ». S'il apparaît dans les boutons, les icônes et les illustrations, il perd son sens.
3. Pas de deuxième animation forte (parallaxe, compteurs qui défilent, logos qui volent). La démo est la seule chose qui bouge vraiment.

---

## Design tokens (proposition)

### Couleurs

| Token | Hex | Usage |
|---|---|---|
| `color.brand.ink` | `#0E1A2E` | Encre principale, boutons primaires |
| `color.brand.ink-hover` | `#1D2D4A` | Survol du bouton primaire |
| `color.brand.accent` | `#19E07A` | État « traité » : pastilles, fonds. Jamais pour du texte |
| `color.success.text` | `#0B7A43` | Texte « Traité » et validation de formulaire |
| `color.success.bg` | `#E6F9EF` | Fond des messages de succès |
| `color.error.text` | `#B42318` | Erreurs de formulaire |
| `color.error.bg` | `#FEF0EE` | Fond des messages d'erreur |
| `color.warning.text` | `#C2410C` | Écart détecté (démo), alertes |
| `color.warning.bg` | `#FFF4E8` | Fond des alertes |
| `color.neutral.0` | `#FFFFFF` | Champs, cartes surélevées |
| `color.neutral.50` | `#FAFAF7` | Fond de page |
| `color.neutral.100` | `#F1F2EE` | Surfaces, panneau de démo |
| `color.neutral.200` | `#E2E4DE` | Filets, bordures |
| `color.neutral.500` | `#6B7280` | Texte désactivé, placeholders (4,8:1 sur blanc, 4,6:1 sur le fond) |
| `color.neutral.700` | `#4A5568` | Texte secondaire |
| `color.neutral.900` | `#0E1A2E` | Texte principal (même valeur que `brand.ink`) |

Contrastes calculés le 2026-11-12 avec la formule WCAG 2.1. Cible : AA, soit 4,5:1 pour le texte et 3:1 pour les éléments d'interface.

| Paire | Ratio | Verdict |
|---|---|---|
| `neutral.900` sur `neutral.50` | 16,7:1 | AA |
| Blanc sur `brand.ink` (bouton) | 17,4:1 | AA |
| Blanc sur `brand.ink-hover` | 13,8:1 | AA |
| `neutral.700` sur `neutral.50` | 7,2:1 | AA |
| `success.text` sur `neutral.50` / `success.bg` | 5,2:1 / 4,9:1 | AA |
| `error.text` sur blanc / `error.bg` | 6,6:1 / 5,9:1 | AA |
| `warning.text` sur `neutral.50` / `warning.bg` | 5,0:1 / 4,8:1 | AA |
| `neutral.500` sur blanc | 4,8:1 | AA |
| `neutral.500` sur `neutral.200` (bouton désactivé) | 3,8:1 | Exempté (élément désactivé) |
| `brand.accent` sur `neutral.50` | 1,7:1 | Sous 3:1 : la pastille porte toujours le mot « Traité » en encre (9,9:1), l'état ne passe jamais par la couleur seule |
| `neutral.200` (filet) sur `neutral.50` | 1,2:1 | Décoratif uniquement : les champs de formulaire ont besoin d'une bordure plus foncée (au moins 3:1) |

### Typographie
Familles : `font.sans` = Inter Tight (titres) et Inter (texte) ; `font.mono` = Geist Mono. Chiffres : `font-variant-numeric: tabular-nums`.

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

### Ombres
`shadow.sm` = `0 1px 2px rgba(14,26,46,.06)` (cartes) ; `shadow.md` = `0 8px 24px rgba(14,26,46,.08)` (panneau de démo) ; `shadow.focus` = `0 0 0 3px rgba(14,26,46,.35)` (anneau de focus).
Les ombres restent discrètes : on privilégie les filets.

### Motion
| Token | Valeur | Usage |
|---|---|---|
| `motion.duration.fast` | 120 ms | Survol, focus |
| `motion.duration.base` | 200 ms | Ouverture d'accordéon (FAQ), changement d'état |
| `motion.duration.slow` | 400 ms | Pastille « traité », surlignage de ligne dans la démo |
| `motion.ease.standard` | `cubic-bezier(.2,0,0,1)` | Défaut |
| `motion.ease.emphasis` | `cubic-bezier(.3,0,0,1.2)` | Pastille « traité » uniquement |

Avec `prefers-reduced-motion: reduce`, la démo passe en images fixes avec étapes numérotées, et les transitions sont réduites à 0 ms.

### Composants clés

**Bouton primaire** : fond `brand.ink`, texte blanc, `radius.md`, hauteur 48 px (44 px minimum en mobile).
États : repos ; survol (`brand.ink-hover`) ; focus (`shadow.focus`, toujours visible) ; actif (enfoncé de 1 px) ; désactivé (fond `neutral.200`, texte `neutral.500`) ; chargement (indicateur et libellé « Envoi… », bouton bloqué).

**Bouton secondaire** : fond transparent, bordure 1 px `neutral.200`, texte `brand.ink`. Mêmes états, avec un fond `neutral.100` au survol.

**Carte** (étape, témoignage, palier tarifaire) : fond `neutral.0`, bordure `neutral.200`, `radius.md`, padding `space.6`, `shadow.sm` facultative. Le palier mis en avant reçoit une bordure `brand.ink` de 2 px, pas de couleur vive.

**Formulaire de démo** : 4 champs, label visible au-dessus de chaque champ (jamais seulement un placeholder), hauteur 48 px. Erreur sous le champ en `error.text`, avec une icône et `aria-describedby`. Succès dans un bloc `success.bg`.

| À faire | À ne pas faire |
|---|---|
| Un seul bouton primaire par écran | Deux boutons primaires côte à côte |
| Libellés de CTA avec un verbe et un objet (« Réserver une démo de 20 min ») | « En savoir plus », « Cliquez ici » |
| Anneau de focus visible sur tous les éléments interactifs | `outline: none` sans remplacement |
| Vert uniquement pour l'état « traité » | Vert sur les boutons, les icônes ou les illustrations |
| Chiffres en mono tabulaire, avec unité et périmètre | Compteurs animés qui défilent jusqu'au chiffre |
| Labels de champ toujours visibles | Placeholders utilisés comme labels |
| Messages d'erreur près du champ, qui disent comment corriger | « Erreur » seul en haut du formulaire |
