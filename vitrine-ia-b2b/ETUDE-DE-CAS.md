# Étude de cas : site vitrine d'une startup IA B2B

> Catégorie `vitrine-ia-b2b`. Entreprise de démonstration : **Ordo**, entreprise FICTIVE (agents IA pour la compta fournisseurs des PME).
> Recherche documentaire de novembre 2026. Dust, Ramp et Pennylane ont été ouverts et capturés pour le bench le 2026-11-12. Dust, Yooz, Vocca, Mistral et toutes les sources chiffrées ont été rouverts le 2026-11-13. Voir les **Notes de méthode** en fin de document.

## Executive summary

L'IA est présente dans 35 % des levées des startups françaises au premier semestre 2026, et la compta fournisseurs est devenue un terrain disputé (Ramp, Yooz, Libeo racheté par Shine). Sur les 6 sites analysés, 4 affichent des chiffres, mais un seul (Ramp) les rattache à une note, et peu montrent le produit en train de traiter un vrai document. La meilleure opportunité pour Ordo : faire de la démo sur une facture réelle la preuve centrale, dans un registre clair et « comptable » qui tranche avec le sombre futuriste du secteur. Il faut aussi afficher un prix et rendre concrète la sécurité des données.

---

## 1. Le marché en 5 lignes

- **L'IA domine les levées** : au premier semestre 2026, 5,1 Md€ ont été levés en France. L'IA est présente dans 89 des 257 opérations (35 %) et dans 40 % des montants ([Licorne Society](https://www.licornesociety.com/blog/bilan-levees-de-fonds-s1-2026), vu le 2026-11-13). Le « 35 % » du README correspond au nombre d'opérations.
- **Les agents prennent le relais** : Dust a levé 40 M$ en mai 2026 ([Maddyness](https://www.maddyness.com/2026/05/18/ia-dust-leve-40-millions-de-dollars-pour-accelerer-sa-croissance-aux-etats-unis/), vu le 2026-11-13), en série B ([tech.eu](https://tech.eu/2026/05/18/dust-raises-40m-series-b-to-build-the-multiplayer-operating-system-for-enterprise-ai/), vu le 2026-11-13). Delos a levé 10 M€ en série A pour ses « AI workers » ([Le Monde Informatique](https://www.lemondeinformatique.fr/donnees-ia/2026-09-17-delos-leve-10-meteuro-pour-deployer-ses-ai-workers), vu le 2026-11-13).
- **La compta fournisseurs est disputée** : Ramp a lancé ses « Agents for AP » le 7 octobre 2025 ([PYMNTS](https://www.pymnts.com/news/artificial-intelligence/2025/ramp-adds-ai-agents-invoice-coding-approval-payment-processing/), vu le 2026-11-13). Shine (groupe Cegid) a racheté Libeo, annonce du 28 septembre 2026 ([FrenchWeb](https://www.frenchweb.fr/specialiste-de-la-gestion-et-du-paiement-des-factures-fournisseurs-libeo-rejoint-shine-cegid/463715), vu le 2026-11-13).
- **La réforme sert de déclencheur** : depuis le 1er septembre 2026, toutes les entreprises assujetties à la TVA établies en France doivent pouvoir recevoir des factures électroniques, via une plateforme agréée ([Moneyvox](https://www.moneyvox.fr/votre-argent/actualites/110141/facturation-electronique-ce-qui-change-vraiment-a-partir-du-1er-septembre-2026), vu le 2026-11-13). Les PME reçoivent donc des données structurées, plus faciles à traiter pour un agent.
- **Conséquence pour le site** : l'acheteur a déjà vu beaucoup de démos « IA ». Il ne croit que ce qu'il voit traité, sourcé et sécurisé.

---

## 2. Critique de 6 sites réels

> Grille : première impression (2 s), usabilité, hiérarchie visuelle, accessibilité, ce qui marche, recommandations. Les renvois « bench n° X » viennent des captures du 2026-11-12. Les mentions « vu le 2026-11-13 » viennent de la page ouverte ce jour-là. Le reste vient de descriptions publiées.

### 2.1 Dust : https://dust.tt (France)
Plateforme d'agents IA reliés aux outils internes : « Connect Dust to 70+ connectors » sur la home (vu le 2026-11-13). Plus de 3 000 organisations : « 3,000+ global organizations » sur la home (bench n° 2) et « more than 3,000 organisations » chez [tech.eu](https://tech.eu/2026/05/18/dust-raises-40m-series-b-to-build-the-multiplayer-operating-system-for-enterprise-ai/) (vu le 2026-11-13).
- **Première impression** : titre en Geist, scène 3D isométrique avec des bulles d'agents nommés par tâche (@LeadQual, @Incident, @TicketRouter), mention « Trusted by teams at 3,000+ global organizations » sous le hero (bench n° 2). L'objectif est clair (demander une démo ou essayer), mais le problème résolu reste large.
- **Usabilité** : bouton « Request a demo » et lien secondaire « Try for free → » (bench n° 2).
- **Hiérarchie** : promesse, puis preuve sociale, puis cas d'usage par métier. L'ordre est logique, mais aucun cas n'est prioritaire.
- **Accessibilité** : bouton bleu en dégradé, texte blanc à 3,2:1 au mieux, sous le seuil WCAG AA de 4,5:1 (bench n° 2).
- **Ce qui marche** : chaque agent est nommé par sa tâche et montre son résultat.
- **Recommandations** : 1) choisir un cas héros plutôt qu'un catalogue ; 2) remplacer le dégradé du bouton par un fond uni assez contrasté.

### 2.2 Mistral AI : https://mistral.ai/fr/news/le-chat-enterprise (France)
Assistant entreprise connecté aux sources de l'entreprise.
- **Première impression** : malgré l'URL en `/fr/`, la page est un article d'annonce en anglais, « Introducing Le Chat Enterprise » (vu le 2026-11-13). L'objectif commercial passe par le lien « Contact » de l'en-tête.
- **Usabilité** : offre entreprise sur contact uniquement. Les produits ont changé de nom (Le Chat, puis Vibe, d'après les résultats de recherche), ce qui brouille la navigation.
- **Hiérarchie** : la marque et l'annonce d'abord, l'offre ensuite. C'est adapté aux grands comptes, pas aux PME.
- **Accessibilité** : non observée.
- **Ce qui marche** : l'argument « privé, personnalisable » est placé tôt.
- **Recommandations** : 1) servir la page en français sur l'URL française ; 2) donner un ordre de prix pour les équipes.

### 2.3 Pennylane : https://www.pennylane.com/fr (France)
Compta et finance pour PME et experts-comptables, avec catégorisation et rapprochements suggérés par IA. C'est un outil cible d'Ordo.
- **Première impression** : onglets d'audience au-dessus de l'en-tête, « Indépendants et TPE », « PME et ETI », « Cabinet expertise comptable » (bench n° 25). On sait vite si on est concerné.
- **Usabilité** : [répertoire d'intégrations](https://www.pennylane.com/fr/integrations) filtrable par catégorie, un modèle pour Ordo.
- **Hiérarchie** : preuves en ligne courte, ISO/IEC 27001, « Made in France », « Plateforme Agréée immatriculée » (bench n° 25).
- **Accessibilité** : bouton vert `#00F872` à texte `#003D3D`, 8,5:1 (bench n° 25). Sur mobile, la capture d'écran de bureau n'est pas recadrée.
- **Ce qui marche** : l'IA présentée comme un bénéfice (« moins de saisie »), pas comme une technologie. Guides éditoriaux bien référencés ([guide IA compta](https://www.pennylane.com/fr/guide-ia-compta)).
- **Recommandations** : 1) recadrer les visuels produit pour le mobile ; 2) alléger les pages d'entrée par cible.

### 2.4 Yooz : https://www.getyooz.com/fr (France, concurrent direct)
Capture, lecture par IA, circuit de validation et intégration ERP ([Cocowork](https://cocowork.fr/yooz/)). Connecteurs Sage 100, Dynamics 365 et SAP Business One.
- **Première impression** : titre en superlatifs, « La solution de facturation électronique propulsée par l'IA la plus intelligente, puissante et sécurisée » (vu le 2026-11-13). L'objectif (« Je réserve ma démo ») est clair, le bénéfice moins.
- **Usabilité** : page [tarifs](https://www.getyooz.com/fr/tarifs) publique : « À partir de 99 € » pour l'abonnement mensuel de la version entreprise, « Nous consulter » pour la version cabinet, plus un calculateur de ROI (vu le 2026-11-13). **Corrigé** : la version précédente disait « tarifs sur devis uniquement ».
- **Hiérarchie** : « Nativement connectée avec plus de 250 applications », « 400 000 sociétés automatisent leurs achats et ventes avec Yooz », un témoignage qui cite « un gain de temps de 20% » (vu le 2026-11-13).
- **Accessibilité** : non observée. Les fiches d'intégration sont en PDF ([exemple](https://getyooz.com/hubfs/Infographie%20%20MVR/Infographie%20FR/Yooz%20-%20Infographie%20-%20Sage100%20by%20Siadeo%20-%20FR.pdf)), souvent peu accessibles aux lecteurs d'écran.
- **Ce qui marche** : la profondeur des intégrations est prouvée, avec une fiche par ERP. Le prix d'entrée est public.
- **Recommandations** : 1) donner le périmètre des chiffres (« 400 000 sociétés » : clientes directes ou via des cabinets ?) ; 2) passer les fiches PDF en pages HTML ; 3) remplacer les superlatifs du titre par le bénéfice.

### 2.5 Vocca : https://vocca.com (France)
Agents vocaux pour l'accueil des cabinets médicaux, 4,7 M€ levés en septembre 2025 ([FrenchWeb](https://www.frenchweb.fr/vocca-leve-47-millions-deuros-pour-deployer-son-ia-vocale-dans-les-cabinets-medicaux/457316), vu le 2026-11-13). Vocca figure dans les prospects du README.
- **Première impression** : une seule verticale (la santé) et un seul métier (le téléphone). Le visiteur se reconnaît immédiatement.
- **Usabilité** : non observée en détail.
- **Hiérarchie** : la promesse métier, puis des chiffres déclarés, « 100% of calls handled » et « 25+ hours of phone time back per practice, every month » (vocca.com, servi en `/en`, vu le 2026-11-13). **Corrigé** : les chiffres « 11 h par jour » et « 30 % à 100 % » de la version précédente n'apparaissent plus sur la page, ils sont retirés.
- **Accessibilité** : non observée.
- **Ce qui marche** : la verticalisation. C'est le modèle à suivre pour Ordo.
- **Recommandations** : 1) donner la source et le périmètre des chiffres ; 2) aligner la langue sur la cible (la home a été servie en anglais, et l'[annonce de levée](https://vocca.com/blog/article/vocca-raises-5-5m-to-transform-healthcare-communication-with-ai-phone-assistants) aussi, pour des cabinets français).

### 2.6 Ramp : https://ramp.com/accounts-payable (États-Unis, référence)
Bill Pay avec des agents qui imputent les lignes, contrôlent la fraude, recommandent les validations et règlent par carte ([annonce Ramp](https://ramp.com/blog/ramp-ap-agents-announcement), vu le 2026-11-13). **Corrigé** : la page Accounts Payable parle de « Ramp's agent » au singulier, pas de quatre agents (bench n° 1).
- **Première impression** : discours chiffré, « 2.4x faster », « 85,000+ businesses », « Up to 7x fewer clicks to process a bill vs Bill.com » (bench n° 1, vu le 2026-11-12). Le bénéfice est clair.
- **Usabilité** : page intégrations citée en exemple, avec un CTA clair et un annuaire d'apps ([SaaS Landing Page](https://saaslandingpage.com/articles/15-outstanding-integration-page-examples/), bench n° 12).
- **Hiérarchie** : un chiffre, puis le produit, puis la preuve, de façon répétitive mais efficace.
- **Accessibilité** : bouton à texte noir sur fond clair, 16:1 (bench n° 1).
- **Ce qui marche** : chaque chiffre porte un renvoi numéroté vers sa source (bench n° 1), et chaque agent est nommé par sa tâche.
- **Recommandations** : 1) réduire le nombre d'affirmations par écran ; 2) rapprocher la source du chiffre, plutôt qu'un simple renvoi.

---

## 3. Thèmes clés

### Thème 1 : des chiffres partout, rarement avec leur source
- **Prévalence** : 4 sites sur 6 mettent en avant des chiffres (Ramp, Vocca, Yooz, Dust). Seul Ramp rattache chaque chiffre à un renvoi numéroté. Aucun ne donne une ligne de périmètre datée sous le chiffre.
- **Observations** : « 2.4x faster » (Ramp, avec renvoi) ; « 25+ hours of phone time back » (Vocca, sans source) ; « 400 000 sociétés » et « gain de temps de 20% » (Yooz, sans périmètre) ; « 3,000+ global organizations » (Dust).
- **Interprétation** : le chiffre est devenu une convention. Ce qui fait la différence, c'est la source. Ordo, entreprise fictive, n'a aucun chiffre de résultat : sa preuve passe par la démo.

### Thème 2 : un discours horizontal ou vertical
- **Prévalence** : 3 sites sur 6 sont horizontaux (Dust, Mistral, Pennylane), 3 sont verticaux ou centrés sur une tâche (Vocca, Yooz, Ramp AP).
- **Observations** : Vocca ne parle qu'aux cabinets médicaux. Dust connecte des agents à toute l'entreprise.
- **Interprétation** : pour une seed qui vend à des PME, le discours vertical paraît plus lisible. Hypothèse à tester (voir les questions).

### Thème 3 : la sécurité et la souveraineté passent devant
- **Prévalence** : 3 sites sur 6 en font un argument visible (Dust, Mistral, Ramp avec son contrôle de fraude).
- **Observations** : section sécurité chez Dust. Offre « privée » chez Mistral.
- **Interprétation** : la phrase « vos données n'entraînent pas nos modèles » devient attendue par les acheteurs.

### Thème 4 : les intégrations comme preuve
- **Prévalence** : 3 sites sur 6 (Pennylane, Yooz, Ramp).
- **Observations** : répertoire filtrable chez Pennylane, une fiche par ERP chez Yooz, annuaire chez Ramp.
- **Interprétation** : pour un agent comptable, « ça se branche sur mon outil » est la première objection à lever.

### Thème 5 : des prix rarement complets
- **Prévalence** : 1 site sur 6 est vu sur contact uniquement (Mistral entreprise). Yooz affiche un prix d'entrée, mais la version cabinet reste sur consultation. Les autres n'ont pas été regardés sous cet angle.
- **Interprétation** : afficher un prix d'entrée et ce que contient chaque palier reste une différenciation à faible coût.

---

## 4. Insights et opportunités

| Insight | Opportunité | Impact | Effort |
|---|---|---|---|
| Les chiffres sont partout, rarement avec leur source | Aucun chiffre de résultat : la preuve passe par la démo, et chaque chiffre public affiché porte sa source | H | B |
| Peu de sites montrent un vrai document traité | Démo sur une facture anonymisée, ligne par ligne, état « traité » en vert | H | M |
| Les sites verticaux sont plus lisibles | Promesse limitée aux factures fournisseurs des PME de 20 à 250 salariés | H | B |
| L'inquiétude sur les données est attendue | Section sécurité concrète : hébergeur nommé, pas d'entraînement, DPA | H | B |
| Les intégrations sont la première objection | Pennylane, Sage et Qonto en grand dans le hero ou juste après la démo | M | B |
| Prix rarement complets | 3 paliers publics, prix d'entrée affiché | M | B |
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

- **Promesse** : un métier, une promesse que la démo vérifie (« Chaque facture rapprochée avec sa commande. »), sans chiffre inventé.
- **La démo est la preuve** : placée juste après le hero, sur une vraie facture anonymisée, avec le vert réservé à l'état « traité ». C'est la seule animation forte.
- **Ce qui distingue Ordo de Yooz et Ramp** : connecteurs natifs vers les outils des PME françaises (Pennylane, Sage, Qonto), hébergement en France avec l'hébergeur nommé, un ton sans superlatif.
- **Forme** : fond presque blanc, encre bleu nuit, mono pour les chiffres. Le site doit ressembler à un bon outil de compta, pas à un laboratoire d'IA.
- **Mobile** : CTA « Démo » fixe, démo verticale sur une seule facture, logos en défilement horizontal.

---

## 7. Questions pour la recherche utilisateur

1. Pour un DAF de PME, quelle preuve convainc le plus : voir une facture traitée, voir un écart signalé, ou lire le journal des actions ?
2. Une démo sur une facture « réelle » anonymisée est-elle plus crédible qu'une interface stylisée ?
3. Afficher un prix fait-il baisser ou monter les demandes de démo qualifiées ?
4. Quelle garantie sur les données compte le plus : l'hébergement en France, l'absence d'entraînement, ou la validation humaine avant paiement ?
5. Les experts-comptables se sentent-ils menacés ou aidés par le discours « agent » ?
6. Le mot « agent » est-il compris par un dirigeant de PME, ou faut-il dire « assistant » ?

## 8. Notes de méthode

- **Sources** : environ 60 recherches web (novembre 2026). Les sources sont la presse tech (Maddyness, FrenchWeb, tech.eu, Le Monde Informatique, PYMNTS), les pages des éditeurs, les comparateurs (Cocowork, G2) et les galeries d'analyse (SaaS Landing Page).
- **Chiffres** : chaque chiffre réel a été rouvert le 2026-11-13, avec sa source à côté. Ceux qu'aucune page ne montrait plus sont retirés : Vocca « 11 h par jour » et « 30 % à 100 % », Yooz « 80 % d'automatisation ». Dust « plus de 100 sources » est corrigé en « 70+ connectors », affiché sur la home.
- **Limites** :
  - Dust, Ramp et Pennylane ont été capturés et audités pour le bench (2026-11-12). Mistral, Yooz et Vocca ont été ouverts le 2026-11-13 pour leurs textes, leurs chiffres et leurs CTA, sans capture ni mesure de contraste.
  - Les chiffres des entreprises (clients, gains) sont déclaratifs.
  - Les prévalences portent sur 6 sites. Elles sont indicatives, pas statistiques.
- **Ce qu'on ne fait pas** : pas de capture ni d'audit de contraste pour Mistral, Yooz et Vocca. Le bench couvre déjà les trois sites qui servent la maquette.
