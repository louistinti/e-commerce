# Étude de cas : site vitrine santé / medtech (télésurveillance)

> Document de travail agence. **Veilla** est une entreprise **fictive**, nom compris. Les entreprises citées sont réelles et servent uniquement de références d'analyse. Aucun chiffre n'est inventé : chaque donnée chiffrée a sa source et sa date de lecture.

## Executive summary

La télésurveillance médicale a quitté le stade expérimental en France : une voie de remboursement de droit commun (LATM) existe, mais la HAS y filtre sévèrement sur les preuves. Les six sites analysés partagent les mêmes codes (bleu et blanc, entrées par public, statut réglementaire, publications) et parlent surtout aux médecins, rarement au patient âgé. Les points faibles récurrents sont des chiffres d'éditeur sans contexte, des contenus vieillissants et un patient relégué au second plan. Veilla peut se différencier avec un one-page qui traite à égalité l'établissement et le patient, des preuves sourcées et datées, et une accessibilité AA réelle.

---

## 1. Le marché en 5 lignes

1. Près de 2 800 entreprises HealthTech en France ; elles ont levé 2,3 Md€ en 2025, en baisse de 9 % sur un an, dont 1,0 Md€ en capital-risque ([communiqué Panorama France HealthTech 2026, France Biotech](https://france-biotech.fr/wp-content/uploads/2026/02/France_Biotech_CP_Panorama_France_HealthTech_2026_VDEF.pdf), vu le 2026-11-13).
2. L'IA est présente dans 37 % des 409 levées françaises analysées depuis janvier 2026, tous secteurs confondus ([Licorne Society](https://www.licornesociety.com/levees-de-fonds), page mise à jour en continu, vue le 2026-11-13).
3. Le remboursement de la télésurveillance passe par la LATM, le droit commun ([G_NIUS](https://gnius.esante.gouv.fr/en/financing/reimbursement-profiles/remote-monitoring-reimbursement), vu le 2026-11-13). Une année de PECAN, la prise en charge anticipée, peut la précéder ([HAS, principes LATM](https://has-sante.fr/upload/docs/application/pdf/2025-09/principes_devaluation_de_la_cnedimts_liste_des_activites_de_telesurveillance_medicale_latm.pdf), vu le 2026-11-13). Pour être remboursé, un dispositif doit être marqué CE, certifié par l'ANS et évalué favorablement par la CNEDiMTS ([Centre Oscar Lambret, GaLIEN n° 74, mai 2026](https://www.centreoscarlambret.fr/sites/default/files/2026-05/galienn74.pdf), vu le 2026-11-13).
4. Resilience PRO a obtenu en octobre 2023 le premier avis favorable de la HAS pour la LATM, Cureety a suivi en janvier 2025, CONTINUUM+ CONNECT a reçu un avis négatif en mars 2026. En oncologie, le forfait de l'opérateur (le soignant qui télésurveille) est de 28 € par mois et par patient (même source : Centre Oscar Lambret, vu le 2026-11-13).
5. L'acheteur (l'établissement) cherche d'abord des preuves, la conformité et un modèle de financement : le site doit être une démonstration.

---

## 2. Critique de 6 sites réels

Grille « design critique » : première impression (2 s), usabilité, hiérarchie visuelle, accessibilité, ce qui marche, recommandations.
Resilience, Cureety et Implicity ont été ouverts dans un vrai navigateur le 2026-11-12 pour le bench ([BENCH.md](BENCH.md)) : leurs fiches reprennent ce qui a été vu. Withings bloque par Cloudflare, Maela renvoie une erreur 403 (2026-11-13), Biofourmis n'a pas été ouvert : pour ces trois sites, les observations viennent des pages indexées, et les points visuels sont notés *non observé*.

### 2.1 Resilience Care (France) : télésurveillance en oncologie
- **URL** : https://www.resilience.care/healthcare-providers/oncology (US : https://www.resilience.care/us)
- **Positionnement** : plateforme soignant et application patient. Pied de page vu le 2026-11-12 : « Class IIa medical device », « CE 0459 », « reimbursed by the French Assurance Maladie », « Update : March 2026 » (bench n° 5). Premier avis favorable de la HAS pour la LATM (section 1).
- **Première impression** : une fenêtre « This site is intended for healthcare professionals » s'ouvre avant la page, avec une sortie vers patients.resilience.care. Derrière, un titre serif (EB Garamond 64 px) sur blanc. Le public cible est le soignant.
- **Usabilité** : navigation par public (soignants / patients), rubriques séparées pour les [publications scientifiques](https://www.resilience.care/us/scientifics-publications) et la [recherche](https://www.resilience.care/en/research), [landing pages thématiques](https://www.resilience.care/en/landing-page/oncology-remote-monitoring). La multiplication des versions FR, EN et US complique le parcours.
- **Hiérarchie visuelle** : 4 grands chiffres d'études, chacun avec appel de note, et un lien « See sources » ; la mention réglementaire datée en pied de page (bench n° 5).
- **Accessibilité** : bouton « Request a demo » à 13,6:1. Sur mobile, la fenêtre « professionnels » ne s'affiche pas (bench M3).
- **Ce qui marche** : les preuves traitées comme du contenu à part entière, chaque chiffre relié à sa source ; la segmentation par public.
- **Recommandations** : 1. unifier les versions linguistiques ; 2. donner au patient une entrée visible depuis la home, pas seulement depuis la fenêtre de filtre.

### 2.2 Cureety (France) : télésurveillance en oncologie
- **URL** : https://www.cureety.com/en-us ; patient : https://www.cureety.com/en-us/patient
- **Positionnement** : suivi des symptômes classés CTCAE, gratuit pour le patient, sur prescription. Inscrit sur la LATM en janvier 2025 après une PECAN (section 1).
- **Première impression** : à la première visite, une fenêtre fait choisir entre « Patient or caregiver » (bouton vert) et « Healthcare professional » (bouton bleu) (bench n° 10). Titre de la home vu le 2026-11-13 : « Your expertise, extended to every moment of treatment ». La version servie est en anglais (en-us) pour un acteur très implanté en France.
- **Usabilité** : page patient séparée, avec 4 étapes numérotées et un bloc aidants. Pas de centre d'aide : un formulaire de contact (bench n° 10). Page [Research](https://www.cureety.com/en-us/research).
- **Hiérarchie visuelle** : page patient en étapes de 01 à 04, boutons « Contact us » et « Ask a question » (bench n° 10).
- **Accessibilité** : texte courant en 18 px sur mobile, mais deux boutons côte à côte aux libellés de 14 px et une connexion cachée dans le menu (bench M2).
- **Ce qui marche** : un chiffre d'étude affiché avec le nom de l'étude, une baisse de 66 % des appels entrants (étude Minerva, selon l'éditeur) ; la certification ISO/IEC 27001:2022 affichée ([cureety.com/en-us](https://www.cureety.com/en-us), vu le 2026-11-13).
- **Recommandations** : 1. servir le français par défaut aux visiteurs français ; 2. qualifier chaque chiffre (type d'étude, n, date) : le « 94 % of patients feel more supported » de la page patient n'a pas de source visible (bench n° 10).

### 2.3 Implicity (France et États-Unis) : télésurveillance des implants cardiaques
- **URL** : https://implicity.com/cied-remote-monitoring/
- **Positionnement** : plateforme multi-constructeurs avec IA de filtrage des alertes. « FDA cleared Class II » et « CE marked » selon l'éditeur ; les notes de bas de page donnent le statut de chaque module (bench n° 6).
- **Première impression** : une fenêtre « contenu réservé aux professionnels de santé » s'ouvre avant la page (bench). Les chiffres-bénéfices (−79 % de faux positifs, −85 % d'alertes FA inutiles, 28 % de patients reconnectés) sont dans des paragraphes de 14 à 15 px avec appels de note, pas en grands chiffres (bench n° 6, vu le 2026-11-12). Un cardiologue les trouve, un patient non.
- **Usabilité** : pages par solution (Cardiac, HF, Research Tool), site patient séparé (patients-info.implicity.com). La page « Clinical Evidence » réunit chiffres et cartes d'études (bench n° 26).
- **Hiérarchie visuelle** : sur « Clinical Evidence », 4 grands chiffres en tête, puis des cartes d'études avec revue, année et citation complète (bench n° 26).
- **Accessibilité** : bouton « Request a demo » blanc sur `#2B8F9C` à 3,8:1, sous le seuil AA de 4,5:1 (WCAG) (bench n° 6).
- **Ce qui marche** : des chiffres-bénéfices précis, chacun relié à une référence publiée, et l'argument « rien à installer », qui répond à la DSI.
- **Recommandations** : 1. sortir les chiffres des paragraphes ; 2. relier depuis la home vers l'information patient.

### 2.4 Maela (France) : suivi péri-opératoire, ambulatoire et RAAC (concurrent le plus proche)
- **URL** : https://www.maela.fr (pages indexées, par ex. https://www.maela.fr/2019/01/11/jab2019/)
- **Positionnement** : plateforme de suivi à distance avec un centre d'appel infirmier, pour « faciliter le retour à domicile des patients » ; déployée dans le service de neurochirurgie du CHU d'Amiens pour un parcours RAAC du rachis ([étude de cas Medtronic](https://www.medtronic.com/content/dam/medtronic-wide/public/western-europe/strategic-partnerships/ihs/integrated-health-solutions-amiens-fr.pdf), vu le 2026-11-13).
- **Première impression** : *non observée* (erreur 403). Les pages indexées les plus visibles sont d'anciennes actualités de congrès, comme celle de 2019 d'après son adresse : le site semble peu entretenu.
- **Usabilité** : *non observée*.
- **Hiérarchie visuelle** : *non observée*.
- **Accessibilité** : *non observée*.
- **Ce qui marche** : un ancrage clinique (actualités de congrès) ; une différenciation par le service humain, le centre d'appel infirmier.
- **Recommandations** : 1. dater et rafraîchir les preuves ; 2. mettre en avant le centre d'appel infirmier comme réponse à la charge soignante.

### 2.5 Withings Health Solutions (France, référence internationale)
- **URL** : https://www.withings.com/us/en/health-solutions/remote-patient-monitoring
- **Positionnement** : RPM de bout en bout, appareils cellulaires sans application côté patient, tableau de bord soignant, aide à la facturation (États-Unis).
- **Première impression** : *non observée* (challenge Cloudflare, bench n° 4). D'après les pages indexées, un discours B2B centré sur le programme RPM et la charge de travail.
- **Usabilité** : home « Health Solutions » séparée du grand public, pages par segment (physicians group, FQHC), [Insight hub](https://www.withings.com/us/en/health-solutions/insight-hub/how-to-start-a-remote-patient-monitoring-program-without-creating-extra-workload).
- **Hiérarchie visuelle** : *non observée*.
- **Accessibilité** : *non observée*.
- **Ce qui marche** : du contenu qui répond à l'objection de la surcharge de travail, une segmentation par acheteur.
- **Recommandations** (pour nous) : 1. reprendre le format « répondre à une objection par bloc » ; 2. ne pas copier la profondeur du site, qui n'est pas transposable en one-page.

### 2.6 Biofourmis (États-Unis, référence internationale)
- **URL** : https://biofourmis.com/care-delivery
- **Positionnement** : « Technology-enabled solutions for care, anywhere ». Hospitalisation à domicile et suivi post-aigu pour de grands systèmes de santé.
- **Première impression** : une promesse corporate générique, sans public explicite (d'après les pages indexées).
- **Usabilité** : pages offre et section « news-insights » alimentée par des annonces de partenariats.
- **Hiérarchie visuelle** : *non observée*.
- **Accessibilité** : *non observée*.
- **Ce qui marche** : chaque établissement partenaire devient une preuve et un contenu.
- **Recommandations** : 1. une promesse plus concrète ; 2. une présence du patient. Contre-exemple pour notre double cible.

---

## 3. Thèmes clés

### T1. Le patient est un public secondaire (5 sites sur 6)
- **Observations** : Implicity relègue le patient sur un sous-domaine ; Resilience le renvoie vers un autre site depuis sa fenêtre « professionnels » ; Withings et Biofourmis s'adressent aux acheteurs B2B ; Maela n'a pas pu être observé. Seul Cureety donne au patient un vrai chemin : choix du public à la première visite, page patient en 4 étapes, bloc aidants (bench n° 10).
- **Interprétation** : le secteur vend aux établissements et considère le patient comme un utilisateur captif. Pour Veilla, dont les patients sont souvent âgés, c'est une opportunité de différenciation et de baisse des appels au support.

### T2. La preuve clinique est l'argument central (6 sites sur 6)
- **Observations** : rubriques publications et recherche (Resilience, Cureety), chiffre-bénéfice (Implicity, Cureety), congrès (Maela), partenariats d'établissements (Biofourmis), contenu sur la charge de travail (Withings).
- **Interprétation** : les preuves sont nécessaires mais inégalement qualifiées. Resilience et Implicity relient chaque chiffre à une référence ; Cureety affiche aussi un « 94 % » sans source visible. La rigueur de présentation peut devenir un marqueur de marque.

### T3. Le statut réglementaire est affiché (3 sites sur 6)
- **Observations** : classe de DM et CE (Resilience, Implicity), FDA (Implicity), ISO 27001 (Cureety).
- **Interprétation** : c'est un critère d'achat éliminatoire pour les établissements. Les jeunes acteurs doivent en parler même quand le statut est « en cours ».

### T4. Anglais par défaut, y compris chez les acteurs français (4 sites sur 6)
- **Observations** : Cureety (en-us), Implicity, Resilience (versions EN et US), Withings (US).
- **Interprétation** : la stratégie internationale passe avant le patient français. Pour Veilla, le français est le choix du lancement, l'anglais viendra en phase 2.

### T5. La fraîcheur des contenus conditionne la confiance (1 cas critique sur 6)
- **Observations** : les pages indexées de Maela les plus visibles sont d'anciennes actualités, comme https://www.maela.fr/2019/01/11/jab2019/.
- **Interprétation** : un site medtech daté laisse supposer une entreprise en difficulté. Il faut un module presse et publications facile à alimenter.

---

## 4. Insights → Opportunités

| Insight | Opportunité | Impact | Effort |
|---|---|---|---|
| Le patient est secondaire sur 5 sites sur 6 | Deux CTA dans le hero, chemin patient en premier sur mobile, FAQ patient | H | M |
| Les chiffres sont inégalement qualifiés | Cartes de preuve normées (étude, n, critère, résultat, date, lien) | H | B |
| La charge soignante est une objection centrale (Withings, Maela, faux positifs chez Implicity) | Bloc « Combien de temps pour votre équipe ? » qui montre qui reçoit l'alerte et quand, sans chiffre tant que le pilote n'a rien publié | H | M |
| Le statut réglementaire est un critère éliminatoire | Bloc conformité lisible, avec badges et statut exact (« en cours ») | H | B |
| Le bleu et blanc clinique est omniprésent | Palette blanc chaud, sauge et bleu profond, différenciante et rassurante | M | B |
| Les contenus vieillissants minent la confiance | CMS publications et presse, date de mise à jour visible | M | M |
| L'anglais est servi par défaut aux Français | FR au lancement, structure i18n prête pour l'EN | M | B |
| Le financement n'est expliqué nulle part simplement | Encadré « Financement » : pas de prise en charge à ce jour, voie visée PECAN puis LATM après le marquage CE | M | M |

## 5. Erreurs à éviter

- Promettre un résultat clinique non démontré (« zéro réhospitalisation »).
- Écrire « remboursé », « marqué CE » ou « certifié HDS » par anticipation.
- Confondre hébergeur certifié HDS et éditeur.
- Utiliser des photos de banque d'images de médecins.
- Mettre du rouge en dehors des alertes.
- Collecter des données de santé via un formulaire du site vitrine.
- Afficher des logos d'établissements, ou des chiffres sans source ni date.

## 6. Conclusion appliquée à Veilla

- **Promesse** : hero « Sécuriser le retour à domicile après une chirurgie ambulatoire ». L'accroche « Moins de réhospitalisations, plus de sorties le jour même » n'est pas utilisée : aucune étude ne la démontre.
- **Architecture** : one-page à deux voies. Établissement : preuves, charge soignante, conformité, financement. Patient : 4 étapes, 5 questions par jour, qui rappelle, « urgence = 15 ».
- **Preuves** : cartes normées ; la carte du pilote dit « Résultats du pilote : publication à venir », sans chiffre ; aucun logo. **Conformité** : badges et documents liés.
- **Équipe** : un bloc « Qui sommes-nous » court, sans photo, puis le comité scientifique avec ses liens d'intérêts.
- **Différenciation** : patient âgé traité comme un public de premier rang (AA vérifié, 18 px minimum, mobile patient en premier) et rigueur des preuves.
- **DA** : blanc chaud, sauge, bleu profond ; ton calme et factuel.

## 7. Questions pour la recherche utilisateur

1. **Cadres de santé** : qu'est-ce qui vous ferait refuser une solution de télésurveillance en moins d'une minute sur son site ?
2. **Directions** : quelles preuves exigez-vous avant un premier rendez-vous (étude publiée, retour d'un pair, chiffres internes) ?
3. **Directions** : le financement (PECAN, LATM) est-il un prérequis ou un bonus au stade du premier contact ?
4. **Patients de plus de 65 ans** : comprenez-vous, en lisant le hero, ce qu'on attend de vous après l'opération ?
5. **Patients** : préférez-vous répondre par SMS, sur une application, ou être appelé ?
6. **Patients et aidants** : qui, dans la famille, lit ce type de page ? Le patient, ou son enfant ?
7. **Tous** : quels mots inquiètent (« surveillance », « alerte », « algorithme ») et lesquels rassurent ?

## 8. Notes de méthode

- **Sources** : recherche web en novembre 2026 ; navigation avec un vrai navigateur le 2026-11-12 (bench) ; chaque chiffre de la section 1 relu sur sa source le 2026-11-13. Institutions (HAS, G_NIUS/ANS, France Biotech), centre de lutte contre le cancer (Oscar Lambret), sites des éditeurs.
- **Limites** :
  - Withings (Cloudflare), Maela (erreur 403) et Biofourmis (non ouvert) ne sont pas observés : leurs fiches s'appuient sur des pages indexées.
  - Les chiffres de performance cités viennent des éditeurs eux-mêmes ; ils ne sont pas vérifiés de manière indépendante.
  - La prévalence des thèmes porte sur un échantillon de 6 sites : c'est un indicateur qualitatif, pas une mesure statistique.
