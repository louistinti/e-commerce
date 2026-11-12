# Étude de cas : site vitrine santé / medtech (télésurveillance)

> Document de travail agence. **Veilla** est une entreprise **fictive** (nom provisoire, à vérifier à l'INPI). Les entreprises citées sont réelles et servent uniquement de références d'analyse.

## Executive summary

La télésurveillance médicale a quitté le stade expérimental en France : une voie de remboursement de droit commun (LATM) existe, mais la HAS y filtre sévèrement sur les preuves. Les six sites analysés partagent les mêmes codes (bleu et blanc, entrées par public, statut réglementaire, publications) et parlent surtout aux médecins, rarement au patient âgé. Les points faibles récurrents sont des chiffres d'éditeur sans contexte, des contenus vieillissants et un patient relégué au second plan. Veilla peut se différencier avec un one-page qui traite à égalité l'établissement et le patient, des preuves sourcées et datées, et une accessibilité AA réelle.

---

## 1. Le marché en 5 lignes

1. Près de 2 800 HealthTech en France ont levé 2,3 Md€ en capital en 2025 (−9 % sur un an) ([Panorama France HealthTech 2026, France Biotech / AFSSI](https://www.afssi.fr/wp-content/uploads/2026/05/Panorama-France-Biotech-2026-AFSSI.pdf), [communiqué](https://france-biotech.fr/wp-content/uploads/2026/02/France_Biotech_CP_Panorama_France_HealthTech_2026_VDEF.pdf)).
2. L'IA est présente dans 35 % des 257 levées françaises du 1er semestre 2026, tous secteurs confondus ([Licorne Society](https://www.licornesociety.com/levees-de-fonds)).
3. Le remboursement de la télésurveillance passe par la LATM (droit commun), précédée éventuellement d'un an de PECAN (prise en charge transitoire) ([HAS, principes LATM](https://has-sante.fr/upload/docs/application/pdf/2025-09/principes_devaluation_de_la_cnedimts_liste_des_activites_de_telesurveillance_medicale_latm.pdf), [G_NIUS](https://gnius.esante.gouv.fr/en/financing/reimbursement-profiles/remote-monitoring-reimbursement)).
4. Resilience PRO a obtenu le premier avis favorable de la HAS pour la LATM (octobre 2023) ; un autre dispositif a reçu un avis négatif en mars 2026 ([Quotidien du Médecin](https://cardiologie.lequotidiendumedecin.fr/sante-societe/politique-de-sante/quel-avenir-pour-la-telesurveillance-medicale)). En oncologie, le forfait est de 28 € par patient et par mois selon un établissement ([Centre Oscar Lambret](https://www.centreoscarlambret.fr/sites/default/files/2026-05/galienn74.pdf)).
5. L'acheteur (l'établissement) cherche d'abord des preuves, la conformité et un modèle de financement : le site doit être une démonstration.

> Le classement « 2e secteur le plus financé en France en 2026 » du README n'a pas pu être confirmé : ne pas le reprendre sans source.

---

## 2. Critique de 6 sites réels

Grille « design critique » : première impression (2 s), usabilité, hiérarchie visuelle, accessibilité, ce qui marche, recommandations.
**Aucun site n'a pu être ouvert** (réseau bloqué). Les observations viennent des pages indexées et de leurs extraits ; les points visuels marqués *(à vérifier)* sont des hypothèses à confirmer en navigation.

### 2.1 Resilience Care (France) : télésurveillance en oncologie
- **URL** : https://www.resilience.care/healthcare-providers/oncology (US : https://www.resilience.care/us)
- **Positionnement** : plateforme soignant (DM classe IIa, CE) et application patient. Premier remboursement pérenne en oncologie.
- **Première impression** : l'objectif est clair dès l'URL (« healthcare providers / oncology »), le public cible est le soignant. Ce qui attire l'œil n'est pas observable *(à vérifier)*.
- **Usabilité** : navigation par public (soignants / patients), rubriques séparées pour les [publications scientifiques](https://www.resilience.care/us/scientifics-publications) et la [recherche](https://www.resilience.care/en/research), [landing pages thématiques](https://www.resilience.care/en/landing-page/oncology-remote-monitoring). La multiplication des versions FR, EN et US complique le parcours.
- **Hiérarchie visuelle** : le statut réglementaire et le remboursement sont mis en avant d'après les descriptions ; l'ordre exact des blocs reste à vérifier.
- **Accessibilité** : non observable *(contraste et taille à auditer)*.
- **Ce qui marche** : les preuves (essais, ASCO) traitées comme du contenu à part entière ; la segmentation par public.
- **Recommandations** : 1. unifier les versions linguistiques ; 2. donner au patient une entrée visible depuis la home.

### 2.2 Cureety (France) : télésurveillance en oncologie
- **URL** : https://www.cureety.com/en-us ; patient : https://www.cureety.com/en-us/patient
- **Positionnement** : suivi des symptômes classés CTCAE, DM classe I, gratuit pour le patient, sur prescription.
- **Première impression** : « Oncology Remote Monitoring Platform », un titre explicite. La version indexée par défaut est en anglais (en-us) pour un acteur très implanté en France.
- **Usabilité** : page patient séparée, centre d'aide avec des articles courts (activer son compte, se connecter), page [Research](https://www.cureety.com/en-us/research).
- **Hiérarchie visuelle** : *(à vérifier)*.
- **Accessibilité** : *(à auditer)*. Le centre d'aide en articles courts est un bon signe pour les patients.
- **Ce qui marche** : un chiffre d'étude concret (appels par patient passés de 5,6 à 1,9 sur 4 mois, selon l'éditeur) ; l'ISO 27001 affiché.
- **Recommandations** : 1. servir le français par défaut aux visiteurs français ; 2. qualifier chaque chiffre (type d'étude, n, date).

### 2.3 Implicity (France et États-Unis) : télésurveillance des implants cardiaques
- **URL** : https://implicity.com/cied-remote-monitoring/
- **Positionnement** : plateforme multi-constructeurs avec IA de filtrage des alertes. « FDA cleared Class II » et « CE marked » selon l'éditeur.
- **Première impression** : bénéfice soignant chiffré (−85 % d'alertes FA inutiles selon l'éditeur), compréhensible par un cardiologue en 2 secondes, pas par un patient.
- **Usabilité** : pages par solution (Cardiac, HF, Research Tool), site patient séparé (patients-info.implicity.com).
- **Hiérarchie visuelle** : *(à vérifier)*.
- **Accessibilité** : *(à auditer)*.
- **Ce qui marche** : un chiffre-bénéfice précis et l'argument « rien à installer », qui répond à la DSI.
- **Recommandations** : 1. contextualiser le chiffre (source, n) ; 2. relier depuis la home vers l'information patient.

### 2.4 Maela (France) : suivi péri-opératoire, ambulatoire et RAAC (concurrent le plus proche)
- **URL** : https://www.maela.fr (pages indexées, par ex. https://www.maela.fr/2019/01/11/jab2019/)
- **Positionnement** : « sécuriser le retour à domicile », avec un plateau infirmier dédié qui traite les alertes ; déployé au CHU d'Amiens ([étude de cas Medtronic](https://www.medtronic.com/content/dam/medtronic-wide/public/western-europe/strategic-partnerships/ihs/integrated-health-solutions-amiens-fr.pdf)).
- **Première impression** : les contenus indexés les plus visibles sont des actualités de congrès 2016-2019 : le site semble peu entretenu.
- **Usabilité** : site WordPress classique, avec un blog d'actualités en entrée principale *(à vérifier)*.
- **Hiérarchie visuelle** : *(à vérifier)*.
- **Accessibilité** : *(à auditer)*.
- **Ce qui marche** : un ancrage clinique (AFC, JAB, SFCE, prix du public AFC 2016) ; une différenciation par le service humain.
- **Recommandations** : 1. dater et rafraîchir les preuves ; 2. mettre en avant le plateau infirmier comme réponse à la charge soignante.

### 2.5 Withings Health Solutions (France, référence internationale)
- **URL** : https://www.withings.com/us/en/health-solutions/remote-patient-monitoring
- **Positionnement** : RPM de bout en bout, appareils cellulaires sans application côté patient, tableau de bord soignant, aide à la facturation (États-Unis).
- **Première impression** : un discours B2B centré sur le programme RPM et la charge de travail *(à vérifier visuellement)*.
- **Usabilité** : home « Health Solutions » séparée du grand public, pages par segment (physicians group, FQHC), [Insight hub](https://www.withings.com/us/en/health-solutions/insight-hub/how-to-start-a-remote-patient-monitoring-program-without-creating-extra-workload).
- **Hiérarchie visuelle** : *(à vérifier)*. La marque est réputée pour la qualité de ses visuels produit.
- **Accessibilité** : *(à auditer)*.
- **Ce qui marche** : du contenu qui répond à l'objection n°1 (la surcharge de travail), une segmentation par acheteur.
- **Recommandations** (pour nous) : 1. reprendre le format « répondre à une objection par bloc » ; 2. ne pas copier la profondeur du site, qui n'est pas transposable en one-page.

### 2.6 Biofourmis (États-Unis, référence internationale)
- **URL** : https://biofourmis.com/care-delivery
- **Positionnement** : « Technology-enabled solutions for care, anywhere ». Hospitalisation à domicile et suivi post-aigu pour de grands systèmes de santé.
- **Première impression** : une promesse corporate générique, sans public explicite.
- **Usabilité** : pages offre et section « news-insights » alimentée par des annonces de partenariats.
- **Hiérarchie visuelle** : *(à vérifier)*.
- **Accessibilité** : *(à auditer)*.
- **Ce qui marche** : chaque établissement partenaire devient une preuve et un contenu.
- **Recommandations** : 1. une promesse plus concrète ; 2. une présence du patient. Contre-exemple pour notre double cible.

---

## 3. Thèmes clés

### T1. Le patient est un public secondaire (5 sites sur 6)
- **Observations** : Implicity et Cureety relèguent le patient sur un sous-domaine ou une page à part ; Resilience l'aborde via l'application ; Withings et Biofourmis s'adressent aux acheteurs B2B. Seul Cureety propose un parcours patient documenté (centre d'aide).
- **Interprétation** : le secteur vend aux établissements et considère le patient comme un utilisateur captif. Pour Veilla, dont les patients sont souvent âgés, c'est une opportunité de différenciation et de baisse des appels au support.

### T2. La preuve clinique est l'argument central (6 sites sur 6)
- **Observations** : rubriques publications et recherche (Resilience, Cureety), chiffre-bénéfice (Implicity, Cureety), congrès (Maela), partenariats d'établissements (Biofourmis), contenu sur la charge de travail (Withings).
- **Interprétation** : les preuves sont nécessaires mais peu qualifiées (chiffres d'éditeur sans n ni date). La rigueur de présentation peut devenir un marqueur de marque.

### T3. Le statut réglementaire est affiché (4 sites sur 6)
- **Observations** : classe de DM et CE (Resilience, Cureety, Implicity), FDA (Implicity), ISO 27001 (Cureety).
- **Interprétation** : c'est un critère d'achat éliminatoire pour les établissements. Les jeunes acteurs doivent en parler même quand le statut est « en cours ».

### T4. Anglais par défaut, y compris chez les acteurs français (4 sites sur 6)
- **Observations** : Cureety (en-us indexé), Implicity, Resilience (versions EN et US), Withings (US).
- **Interprétation** : la stratégie internationale passe avant le patient français. Pour Veilla, le français est le choix du lancement, l'anglais viendra en phase 2.

### T5. La fraîcheur des contenus conditionne la confiance (1 cas critique sur 6)
- **Observations** : les contenus indexés de Maela datent de 2016-2019.
- **Interprétation** : un site medtech daté laisse supposer une entreprise en difficulté. Il faut un module presse et publications facile à alimenter.

---

## 4. Insights → Opportunités

| Insight | Opportunité | Impact | Effort |
|---|---|---|---|
| Le patient est secondaire sur 5 sites sur 6 | Deux CTA dans le hero, chemin patient en premier sur mobile, FAQ patient | H | M |
| Les chiffres sont rarement qualifiés | Cartes de preuve normées (étude, n, critère, résultat, date, lien) | H | B |
| La charge soignante est l'objection n°1 (Withings, Maela, fausses alertes signalées en oncologie) | Bloc « Combien de temps pour votre équipe ? » avec données du pilote | H | M |
| Le statut réglementaire est un critère éliminatoire | Bloc conformité lisible, avec badges et statut exact (« en cours ») | H | B |
| Le bleu et blanc clinique est omniprésent | Palette blanc chaud, sauge et bleu profond, différenciante et rassurante | M | B |
| Les contenus vieillissants minent la confiance | CMS publications et presse, date de mise à jour visible | M | M |
| L'anglais est servi par défaut aux Français | FR au lancement, structure i18n prête pour l'EN | M | B |
| Le financement n'est expliqué nulle part simplement | Encadré « Financement » (PECAN, LATM ou budget établissement, selon le statut réel) | M | M |

## 5. Erreurs à éviter

- Promettre un résultat clinique non démontré (« zéro réhospitalisation »).
- Écrire « remboursé », « marqué CE » ou « certifié HDS » par anticipation.
- Confondre hébergeur certifié HDS et éditeur.
- Utiliser des photos de banque d'images de médecins.
- Mettre du rouge en dehors des alertes.
- Collecter des données de santé via un formulaire du site vitrine.
- Afficher des logos d'établissements sans accord écrit, ou des chiffres sans source ni date.

## 6. Conclusion appliquée à Veilla

- **Promesse** : « Moins de réhospitalisations, plus de sorties le jour même » doit être présentée comme un objectif tant qu'aucune étude ne la démontre. Hero de repli : « Sécuriser le retour à domicile après une chirurgie ambulatoire ».
- **Architecture** : one-page à deux voies. Établissement : preuves, charge soignante, conformité, financement. Patient : 4 étapes, 2 minutes par jour, qui rappelle, « urgence = 15 ».
- **Preuves** : cartes normées et logos sous accord. **Conformité** : badges et documents liés.
- **Différenciation** : patient âgé traité comme un public de premier rang (AA vérifié, 18 px minimum, mobile patient en premier) et rigueur des preuves.
- **DA** : blanc chaud, sauge, bleu profond ; ton calme et factuel.

## 7. Questions à valider en recherche utilisateur

1. **Cadres de santé** : qu'est-ce qui vous ferait refuser une solution de télésurveillance en moins d'une minute sur son site ?
2. **Directions** : quelles preuves exigez-vous avant un premier rendez-vous (étude publiée, retour d'un pair, chiffres internes) ?
3. **Directions** : le financement (PECAN, LATM) est-il un prérequis ou un bonus au stade du premier contact ?
4. **Patients de plus de 65 ans** : comprenez-vous, en lisant le hero, ce qu'on attend de vous après l'opération ?
5. **Patients** : préférez-vous répondre par SMS, sur une application, ou être appelé ?
6. **Patients et aidants** : qui, dans la famille, lit ce type de page ? Le patient, ou son enfant ?
7. **Tous** : quels mots inquiètent (« surveillance », « alerte », « algorithme ») et lesquels rassurent ?

## 8. Notes de méthode

- **Sources** : recherche web (WebSearch) en novembre 2026 ; presse spécialisée (Quotidien du Médecin, Quotidien du Pharmacien), institutions (HAS, G_NIUS/ANS, France Biotech), sites des éditeurs (pages indexées).
- **Limites** :
  - Aucun site n'a pu être ouvert (WebFetch bloqué par le réseau de la session : ENOTFOUND). Première impression, hiérarchie visuelle et accessibilité ne sont **pas observées** ; elles sont marquées *(à vérifier)*.
  - Les chiffres de performance cités viennent des éditeurs eux-mêmes ; ils ne sont pas vérifiés de manière indépendante.
  - Maela : seules des pages de 2016 à 2019 sont indexées. L'état actuel du site est inconnu.
  - La prévalence des thèmes porte sur un échantillon de 6 sites : c'est un indicateur qualitatif, pas une mesure statistique.
- **Prochaine étape** : une session de navigation de 2 h (captures desktop et mobile, audit de contraste avec un outil) pour compléter les champs *(à vérifier)*.
