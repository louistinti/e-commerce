# Étude de cas : site vitrine d'une startup IA B2B

> Catégorie `vitrine-ia-b2b`. Entreprise de démonstration : **Ordo**, entreprise FICTIVE (agents IA pour la compta fournisseurs des PME).
> Recherche documentaire de novembre 2026. Les sites n'ont pas pu être ouverts (réseau bloqué). Voir les **Notes de méthode** en fin de document.

## Executive summary

Les startups IA B2B captent environ un tiers des opérations de financement en France en 2026, et la compta fournisseurs est devenue un terrain disputé (Ramp, Yooz, Libeo racheté par Shine). Sur les 6 sites analysés, la plupart affirment des gains chiffrés sans en donner le périmètre, et peu montrent le produit en train de traiter un vrai document. La meilleure opportunité pour Ordo : faire de la démo sur une facture réelle la preuve centrale, dans un registre clair et « comptable » qui tranche avec le sombre futuriste du secteur. Il faut aussi afficher les prix et rendre concrète la sécurité des données.

---

## 1. Le marché en 5 lignes

- **L'IA domine les levées** : au premier semestre 2026, 5,1 Md€ ont été levés en France. L'IA est présente dans 40 % des montants et dans 35 % des opérations ([Licorne Society](https://www.licornesociety.com/blog/bilan-levees-de-fonds-s1-2026)). Le « 35 % » du README correspond au nombre d'opérations.
- **Les agents prennent le relais** : Dust a levé 40 M$ en série B en mai 2026 ([Maddyness](https://www.maddyness.com/2026/05/18/ia-dust-leve-40-millions-de-dollars-pour-accelerer-sa-croissance-aux-etats-unis/)), Delos 10 M€ pour ses « AI workers » ([Le Monde Informatique](https://www.lemondeinformatique.fr/actualites/lire-delos-leve-10-meteuro-pour-deployer-ses--ai-workers-100791.html)).
- **La compta fournisseurs est disputée** : Ramp a lancé des agents dédiés en octobre 2025 ([PYMNTS](https://www.pymnts.com/news/artificial-intelligence/2025/ramp-adds-ai-agents-invoice-coding-approval-payment-processing/)). Shine (groupe Cegid) a racheté Libeo en septembre 2026 ([FrenchWeb](https://www.frenchweb.fr/specialiste-de-la-gestion-et-du-paiement-des-factures-fournisseurs-libeo-rejoint-shine-cegid/463715)).
- **La réforme sert de déclencheur** : depuis le 1er septembre 2026, toute entreprise doit pouvoir recevoir des factures électroniques via une plateforme agréée ([Moneyvox](https://www.moneyvox.fr/actu/110141/facturation-electronique-ce-qui-change-vraiment-a-partir-du-1er-septembre-2026)). Les PME reçoivent donc des données structurées, plus faciles à traiter pour un agent.
- **Conséquence pour le site** : l'acheteur a déjà vu dix démos « IA ». Il ne croit que ce qu'il voit traité, chiffré et sécurisé.

---

## 2. Critique de 6 sites réels

> Grille : première impression (2 s), usabilité, hiérarchie visuelle, accessibilité, ce qui marche, recommandations. Les points marqués *[à vérifier]* viennent de descriptions ou d'une connaissance antérieure du site, pas d'une visite en novembre 2026.

### 2.1 Dust : https://dust.tt (France)
Plateforme d'agents IA reliés aux outils internes (plus de 100 sources). L'entreprise revendique plus de 3 000 organisations ([tech.eu](https://tech.eu/2026/05/18/dust-raises-40m-series-b-to-build-the-multiplayer-operating-system-for-enterprise-ai/)).
- **Première impression** : promesse « des agents pour chaque équipe » et logos clients *[à vérifier]*. L'objectif est clair (demander une démo ou essayer), mais le problème résolu reste large.
- **Usabilité** : double CTA démo et essai. Navigation par produit, solutions et sécurité *[à vérifier]*.
- **Hiérarchie** : promesse, puis preuve sociale, puis cas d'usage par métier. L'ordre est logique, mais aucun cas n'est prioritaire.
- **Accessibilité** : non observable (page non ouverte).
- **Ce qui marche** : cas d'usage classés par équipe, sécurité traitée comme une section à part entière.
- **Recommandations** : 1) choisir un cas héros plutôt qu'un catalogue ; 2) chiffrer un résultat client dans le hero.

### 2.2 Mistral AI : https://mistral.ai/fr/news/le-chat-enterprise (France)
Assistant entreprise déployable en auto-hébergement, en cloud privé ou en service hébergé, connecté à SharePoint et Drive.
- **Première impression** : identité visuelle très marquée *[à vérifier]*. L'objectif commercial (contacter les ventes) passe après la marque.
- **Usabilité** : offre entreprise sur contact uniquement. Les produits ont changé de nom (Le Chat, puis Vibe, d'après les résultats), ce qui brouille la navigation.
- **Hiérarchie** : la marque d'abord, l'offre ensuite. C'est adapté aux grands comptes, pas aux PME.
- **Accessibilité** : non observable.
- **Ce qui marche** : l'argument « européen, déployable chez vous » est placé tôt.
- **Recommandations** : 1) stabiliser le nommage des produits ; 2) donner un ordre de prix pour les équipes.

### 2.3 Pennylane : https://www.pennylane.com/fr/pme/solutions-comptabilite (France)
Compta et finance pour PME et experts-comptables, avec catégorisation et rapprochements suggérés par IA. C'est un outil cible d'Ordo.
- **Première impression** : entrée par cible (PME, indépendants, experts-comptables). On sait vite si on est concerné.
- **Usabilité** : [répertoire d'intégrations](https://www.pennylane.com/fr/integrations) filtrable par catégorie, un modèle pour Ordo.
- **Hiérarchie** : site très vaste. Le visiteur doit choisir parmi beaucoup de chemins.
- **Accessibilité** : non observable.
- **Ce qui marche** : l'IA présentée comme un bénéfice (« moins de saisie »), pas comme une technologie. Guides éditoriaux bien référencés ([guide IA compta](https://www.pennylane.com/fr/guide-ia-compta)).
- **Recommandations** : 1) harmoniser les dates de la réforme, qui sont contradictoires d'une page à l'autre ; 2) alléger les pages d'entrée par cible.

### 2.4 Yooz : https://www.getyooz.com (France, concurrent direct)
Capture, lecture par IA, circuit de validation et intégration ERP ([Cocowork](https://cocowork.fr/yooz/)). Connecteurs Sage 100, Dynamics 365 et SAP Business One.
- **Première impression** : discours d'éditeur classique *[à vérifier]*. L'objectif (devis ou démo) est clair, le bénéfice moins.
- **Usabilité** : tarifs sur devis uniquement, une friction pour une PME.
- **Hiérarchie** : fonctionnalités et connecteurs d'abord, résultats ensuite.
- **Accessibilité** : non observable. Les fiches d'intégration sont en PDF ([exemple](https://getyooz.com/hubfs/Infographie%20%20MVR/Infographie%20FR/Yooz%20-%20Infographie%20-%20Sage100%20by%20Siadeo%20-%20FR.pdf)), souvent peu accessibles aux lecteurs d'écran.
- **Ce qui marche** : la profondeur des intégrations est prouvée, avec une fiche par ERP.
- **Recommandations** : 1) donner le périmètre des chiffres (« 80 % d'automatisation » de quoi ?) ; 2) passer les fiches PDF en pages HTML ; 3) afficher un prix d'entrée.

### 2.5 Vocca : https://vocca.com (France)
Agents vocaux pour l'accueil des cabinets médicaux, seed de 4,7 M€ en 2025 ([FrenchWeb](https://www.frenchweb.fr/vocca-leve-47-millions-deuros-pour-deployer-son-ia-vocale-dans-les-cabinets-medicaux/457316)). Vocca figure dans les prospects du README.
- **Première impression** : une seule verticale (la santé) et un seul métier (le téléphone). Le visiteur se reconnaît immédiatement.
- **Usabilité** : non observable en détail.
- **Hiérarchie** : la promesse métier et des résultats clients chiffrés (« 11 h gagnées par jour et par site », taux de réponse passé de 30 % à 100 %, chiffres déclarés).
- **Accessibilité** : non observable.
- **Ce qui marche** : la verticalisation, avec des résultats au niveau du client. C'est le modèle à suivre pour Ordo.
- **Recommandations** : 1) donner la source et le périmètre des chiffres ; 2) aligner la langue sur la cible (l'[annonce de levée](https://vocca.com/blog/article/vocca-raises-5-5m-to-transform-healthcare-communication-with-ai-phone-assistants) est en anglais, pour des cabinets français).

### 2.6 Ramp : https://ramp.com/accounts-payable (États-Unis, référence)
Bill Pay avec quatre agents : imputation, fraude, résumé de validation, paiement ([annonce Ramp](https://ramp.com/blog/ramp-ap-agents-announcement)).
- **Première impression** : discours entièrement chiffré (« 2,4 fois plus rapide », « jusqu'à 7 fois moins de clics que Bill.com »). Le bénéfice est clair.
- **Usabilité** : page intégrations citée en exemple, avec un CTA clair et un annuaire d'apps ([SaaS Landing Page](https://saaslandingpage.com/articles/15-outstanding-integration-page-examples/)).
- **Hiérarchie** : un chiffre, puis le produit, puis la preuve, de façon répétitive mais efficace.
- **Accessibilité** : non observable.
- **Ce qui marche** : chaque affirmation porte un chiffre, et chaque agent est nommé par sa tâche.
- **Recommandations** : 1) réduire le nombre d'affirmations par écran ; 2) sourcer les chiffres, qui viennent des données internes de Ramp.

---

## 3. Thèmes clés

### Thème 1 : des gains chiffrés, rarement avec leur périmètre
- **Prévalence** : 4 sites sur 6 mettent en avant des gains chiffrés (Ramp, Vocca, Yooz, Dust). Aucun des 4 ne donne de périmètre visible dans les sources consultées.
- **Observations** : « 2,4 fois plus rapide » (Ramp, données internes) ; « 11 h par jour » (Vocca, chiffre déclaré) ; « 80 % d'automatisation » (Yooz, supports de l'éditeur).
- **Interprétation** : le chiffre est devenu une convention. Ce qui fait la différence, c'est le chiffre **vérifiable**.

### Thème 2 : un discours horizontal ou vertical
- **Prévalence** : 3 sites sur 6 sont horizontaux (Dust, Mistral, Pennylane), 3 sont verticaux ou centrés sur une tâche (Vocca, Yooz, Ramp AP).
- **Observations** : Vocca ne parle qu'aux cabinets médicaux. Dust propose des agents « pour chaque équipe ».
- **Interprétation** : pour une seed qui vend à des PME, le discours vertical convertit mieux. Hypothèse à tester (voir les questions).

### Thème 3 : la sécurité et la souveraineté passent devant
- **Prévalence** : 3 sites sur 6 en font un argument visible (Dust, Mistral, Ramp avec son agent fraude).
- **Observations** : section sécurité dédiée chez Dust. Déploiement « chez vous » chez Mistral.
- **Interprétation** : la phrase « vos données n'entraînent pas nos modèles » devient attendue par les acheteurs.

### Thème 4 : les intégrations comme preuve
- **Prévalence** : 3 sites sur 6 (Pennylane, Yooz, Ramp).
- **Observations** : répertoire filtrable chez Pennylane, une fiche par ERP chez Yooz, annuaire chez Ramp.
- **Interprétation** : pour un agent comptable, « ça se branche sur mon outil » est la première objection à lever.

### Thème 5 : des prix rarement publics pour l'offre IA
- **Prévalence** : 2 sites sur 6 au moins sont sur devis ou contact (Yooz, Mistral entreprise). Les autres restent à vérifier.
- **Interprétation** : afficher les prix est une différenciation à faible coût pour Ordo.

---

## 4. Insights et opportunités

| Insight | Opportunité | Impact | Effort |
|---|---|---|---|
| Les chiffres sont partout, jamais avec leur périmètre | Chaque chiffre accompagné d'une ligne de périmètre (échantillon, période) | H | B |
| Peu de sites montrent un vrai document traité | Démo sur une facture anonymisée, ligne par ligne, état « traité » en vert | H | M |
| Les sites verticaux sont plus lisibles | Promesse limitée aux factures fournisseurs des PME de 20 à 250 salariés | H | B |
| L'inquiétude sur les données est attendue | Section sécurité concrète : hébergeur nommé, pas d'entraînement, DPA | H | B |
| Les intégrations sont la première objection | Pennylane, Sage et Qonto en grand dans le hero ou juste après la démo | M | B |
| Tarifs souvent cachés | 3 paliers publics | M | B |
| Le sombre futuriste est la norme visuelle IA | Registre clair, « relevé comptable » | M | B |
| La réforme crée un afflux de factures structurées | Accroche secondaire : « Vous recevez des e-factures ? Ordo les traite. » | M | B |
| Démo interactive rare (invoicemon sur One Page Love) | Phase 2 : « déposez une facture d'exemple » | M | H |

---

## 5. Conventions et erreurs à éviter

**Conventions** (que tout le monde suit) : hero centré avec double CTA, mur de logos, captures dans un faux navigateur, « comment ça marche » en 3 étapes, grille d'intégrations, badges de sécurité, témoignages avec photo.

**Erreurs à éviter** :
- Le jargon (« révolutionner », « autonome », « nouvelle génération ») et les visuels de cerveaux ou de robots.
- Une vidéo de 2 minutes en lecture automatique avec le son. Une boucle muette de 15 à 25 secondes, avec un bouton pause, suffit.
- Des logos d'intégration ou des badges de certification non acquis.
- Plusieurs animations concurrentes.
- Un formulaire de démo à plus de 4 champs.
- L'anglais par défaut pour une cible PME française.

---

## 6. Conclusion appliquée à Ordo (fictif)

- **Promesse** : un métier, un chiffre (« 4 h gagnées par semaine sur la compta fournisseurs »), avec son périmètre sous le chiffre.
- **La démo est la preuve** : placée juste après le hero, sur une vraie facture anonymisée, avec le vert réservé à l'état « traité ». C'est la seule animation forte.
- **Ce qui distingue Ordo de Yooz et Ramp** : connecteurs natifs vers les outils des PME françaises (Pennylane, Sage, Qonto), prix publics, hébergement en France avec l'hébergeur nommé.
- **Forme** : fond presque blanc, encre bleu nuit, mono pour les chiffres. Le site doit ressembler à un bon outil de compta, pas à un laboratoire d'IA.
- **Mobile** : CTA « Démo » fixe, démo verticale sur une seule facture, logos en défilement horizontal.

---

## 7. Questions à valider en recherche utilisateur

1. Pour un DAF de PME, quel chiffre convainc le plus : des heures gagnées, un pourcentage de factures traitées sans intervention, ou un délai de clôture ?
2. Une démo sur une facture « réelle » anonymisée est-elle plus crédible qu'une interface stylisée ?
3. Afficher les prix fait-il baisser ou monter les demandes de démo qualifiées ?
4. Quelle garantie sur les données compte le plus : l'hébergement en France, l'absence d'entraînement, ou la validation humaine avant paiement ?
5. Les experts-comptables se sentent-ils menacés ou aidés par le discours « agent » ?
6. Le mot « agent » est-il compris par un dirigeant de PME, ou faut-il dire « assistant » ?

## 8. Notes de méthode

- **Sources** : environ 60 recherches web (novembre 2026). Les sources sont la presse tech (Maddyness, FrenchWeb, tech.eu, Le Monde Informatique), les pages des éditeurs, les comparateurs (Cocowork, G2) et les galeries d'analyse (SaaS Landing Page).
- **Limites** :
  - Aucun site n'a pu être ouvert (accès réseau bloqué). Les critiques portent sur les descriptions publiées et sur une connaissance antérieure des sites. Elles sont marquées *[à vérifier]* quand c'est le cas.
  - L'accessibilité n'a pas pu être évaluée sur pièce (contrastes et tailles non mesurés).
  - Les chiffres des entreprises (clients, gains) sont déclaratifs.
  - Les prévalences portent sur 6 sites. Elles sont indicatives, pas statistiques.
- **Prochaine étape** : capture des 6 homes (desktop et mobile), audit de contraste avec un outil (par exemple WAVE ou axe), puis mise à jour des sections marquées *[à vérifier]*.
