# Brief client : site vitrine Veilla

> **Entreprise fictive**, inventée par l'agence comme cas de démonstration, nom compris. Personne ne valide ce brief : l'agence tranche tout. Aucun chiffre n'est inventé. Les seuls nombres sont des valeurs de conception (tailles, étapes, semaines), des normes nommées, ou des données publiques avec leur source et la date de lecture.

**Émetteur** : Veilla (SAS en création, Lyon), direction générale et direction médicale
**Destinataire** : agence web
**Date** : novembre 2026
**Version** : 1.0

---

## 1. Présentation de l'entreprise

- **Activité** : logiciel de télésurveillance des patients après une chirurgie ambulatoire. Le patient répond chaque jour, pendant une durée fixée par l'équipe médicale, à un court questionnaire (douleur, fièvre, saignement, nausées, cicatrice) sur smartphone, tablette ou SMS. Un algorithme à règles, paramétré par l'équipe médicale, classe les réponses ; un signal anormal déclenche une alerte vers l'infirmière de coordination de l'établissement.
- **Équipe** : une anesthésiste-réanimatrice et un ingénieur, cofondateurs, une petite équipe produit et clinique, un comité scientifique en constitution.
- **Stade** : seed. Des établissements pilotes : un CHU et des cliniques privées.
- **Statut réglementaire** : logiciel dispositif médical en cours de marquage CE, classe IIa visée. La règle 11 de l'annexe VIII du règlement (UE) 2017/745 classe en IIa les logiciels qui fournissent des informations utilisées pour prendre des décisions à des fins diagnostiques ou thérapeutiques, et ceux qui contrôlent des processus physiologiques ([EUR-Lex](https://eur-lex.europa.eu/eli/reg/2017/745/oj/fra), vu le 2026-11-13). Hébergement des données chez un hébergeur certifié HDS.

## 2. Contexte et déclencheur

- Nous avons aujourd'hui une page unique faite sur un outil no-code, en anglais, sans preuves ni mentions réglementaires.
- **Déclencheurs** :
  1. Le pilote au CHU se termine ; les premiers résultats observationnels seront publiés ensuite.
  2. Une levée de série A est prévue : les investisseurs et les établissements consultent le site avant tout rendez-vous.
  3. Des patients des sites pilotes cherchent « Veilla » sur Google et tombent sur une page qui ne leur parle pas.
- Le site doit être en ligne **avant le prochain congrès national de chirurgie ambulatoire**.

## 3. Objectifs business et KPIs

| Objectif | KPI | Cible |
|---|---|---|
| Générer des rendez-vous établissements | Demandes de démo qualifiées (formulaire établissement) | Suivi mensuel, sans cible chiffrée |
| Crédibiliser la solution | Clics vers les publications et téléchargements du dossier de preuves | Part des visiteurs « établissement », suivie sans cible chiffrée |
| Orienter les patients sans surcharger le support | Clics « Accéder à mon espace » et recours à la FAQ patient | Évolution des appels patients « comment ça marche » aux sites pilotes, suivie sans cible chiffrée |
| Soutenir la levée | Visites depuis les liens du dossier investisseurs | Suivi qualitatif |
| Accessibilité | Audit RGAA 4.1 / WCAG 2.2 AA | 0 non-conformité bloquante |
| Performance | Core Web Vitals (mobile) | LCP < 2,5 s, CLS < 0,1 (seuils « bon » des Core Web Vitals de Google) |

## 4. Cibles et personas

### Persona 1 : Claire, 48 ans, cadre de santé d'une unité de chirurgie ambulatoire (CHU)
- **Rôle** : prescriptrice et utilisatrice. Elle porte le projet auprès de la direction.
- **Job to be done** : « Quand je fais sortir un patient le jour même, je veux être alertée seulement s'il y a un vrai problème, pour sécuriser la sortie sans saturer mon équipe. »
- **Attentes** : savoir qui reçoit l'alerte et combien de temps cela prend par jour, en bref la charge pour l'équipe ; connaître l'intégration au DPI ; savoir comment on forme l'équipe ; connaître les retours d'autres unités.
- **Freins** : la peur d'une avalanche de fausses alertes, une équipe déjà saturée, les projets numériques abandonnés.
- **Ce qu'elle doit trouver** : le parcours en 4 étapes, une capture du tableau de bord, le trajet d'une alerte (qui la reçoit, à quel moment, ce qu'elle déclenche), un témoignage de pair sans chiffre.

### Persona 2 : Marc, 55 ans, directeur des opérations d'un groupe de cliniques privées
- **Rôle** : décideur budgétaire.
- **Job to be done** : « Quand j'arbitre un investissement numérique, je veux des preuves et un cadre réglementaire solide, pour développer l'ambulatoire sans risque juridique ni dépense à fonds perdus. »
- **Attentes** : effet sur le taux de sortie le jour même, les réhospitalisations et les appels de J+1 ; modèle économique ; conformité (CE, HDS, RGPD) ; sécurité ; références.
- **Freins** : le risque juridique et la responsabilité médicale, le coût de déploiement, une jeune société (va-t-elle durer ?).
- **Ce qu'il doit trouver** : la section preuves, le bloc conformité, le statut de financement exact, le bloc « Qui sommes-nous » et le comité scientifique, un CTA « Demander une présentation ». Statut de financement affiché : pas de prise en charge par l'Assurance maladie à ce jour ; la voie visée est la PECAN puis la LATM, qui exigent d'abord le marquage CE ([Centre Oscar Lambret, GaLIEN n° 74](https://www.centreoscarlambret.fr/sites/default/files/2026-05/galienn74.pdf), vu le 2026-11-13).

### Persona 3 : Jeanne, 72 ans, opérée de la cataracte (ou d'une hernie), avec sa fille Sophie, 45 ans, en appui
- **Rôle** : utilisatrice finale, souvent aidée d'un proche.
- **Job to be done** : « Quand je rentre chez moi après l'opération, je veux savoir quoi faire et être sûre que quelqu'un veille, pour me rétablir sereinement sans avoir l'impression de déranger. »
- **Attentes** : comprendre en 30 secondes ce qu'on attend d'elle, savoir qui la rappelle et quoi faire en cas d'urgence, être rassurée sur ses données.
- **Freins** : la technologie (« je ne suis pas douée »), la vue, la peur d'être « surveillée », la peur de déranger.
- **Ce qu'elle doit trouver** : le chemin « Je suis un patient » en premier sur mobile, 3 phrases simples, un gros bouton « Accéder à mon espace », le rappel « En cas d'urgence, appelez le 15 », une FAQ.

## 5. Messages clés et preuves

| Message | Preuve affichée sur le site |
|---|---|
| « Sécuriser le retour à domicile après une chirurgie ambulatoire » (hero) | Description du dispositif et de l'indication |
| « Moins de réhospitalisations, plus de sorties le jour même » | **Non utilisé** : aucune étude ne le démontre. La carte du pilote dit « Résultats du pilote : publication à venir », sans chiffre. |
| « 5 questions par jour pour le patient » | Le questionnaire lui-même (douleur, fièvre, saignement, nausées, cicatrice), montré sur la capture du téléphone |
| « Les alertes arrivent aux bonnes personnes, pas à tout le monde » | Le trajet d'une alerte : qui la reçoit, quand, ce qu'elle déclenche. Aucun taux affiché tant que le pilote n'a rien publié. |
| « Conçu avec des soignants » | Fondatrice anesthésiste-réanimatrice, comité scientifique nommé (sections destinées aux professionnels) |
| « Vos données sont hébergées en France chez un hébergeur certifié HDS » | Badge « Hébergeur certifié HDS » et lien vers la [liste officielle des hébergeurs certifiés de l'ANS](https://esante.gouv.fr/offres-services/hds/liste-des-hebergeurs-certifies) (vu le 2026-11-13). L'hébergeur de Veilla est fictif : aucun nom affiché. |
| « En cours de marquage CE » | Mention datée en pied de page. Jamais « marqué CE ». |

**Interdits** : superlatifs (« le meilleur », « révolutionnaire »), promesses de guérison ou de détection exhaustive, chiffres sans source, logos d'établissements.

## 6. Arborescence et contenus attendus

One-page avec ancres, et quelques pages annexes.

1. **Hero** : titre, sous-titre et deux CTA (« Je suis un établissement », « Je suis un patient »). Visuel : capture du tableau de bord et du questionnaire sur téléphone.
2. **Le parcours patient en 4 étapes** : 1. sortie de l'unité avec l'application activée, 2. questionnaire quotidien de 5 questions, 3. analyse des réponses, 4. l'infirmière rappelle si besoin. Illustrations simples.
3. **Le tableau de bord soignant** : capture annotée avec données fictives (liste des patients, niveau d'alerte, historique). La charge de travail est décrite sans chiffre : qui reçoit l'alerte, à quel moment.
4. **Preuves** : cartes d'études au format normé (type, n, critère, résultat, lien). La carte du pilote dit « Résultats du pilote : publication à venir », sans chiffre. Chiffres de contexte publics et sourcés seulement (HAS, Assurance maladie), jamais présentés comme des résultats de Veilla. Établissements pilotes décrits par leur type (CHU, clinique privée), sans logo.
5. **Conformité et sécurité** : statut DM et CE (« en cours »), HDS, RGPD (DPO, base légale), sécurité (chiffrement). Pas de mention ISO 27001 : Veilla n'est pas certifiée. Le tout lié aux documents.
6. **Qui sommes-nous et comité scientifique** : un bloc court, sans photo, avec le logo ou une illustration au trait. Texte : « Veilla est née à Lyon de la rencontre d'une anesthésiste-réanimatrice et d'un ingénieur. Ensemble, ils conçoivent un suivi simple pour les jours qui suivent une chirurgie ambulatoire, avec un comité scientifique de soignants. » Puis le comité scientifique : noms, titres, liens d'intérêts déclarés.
7. **Publications et presse** : liste datée, filtrable par type, alimentée via le CMS. En démo, chaque entrée est marquée « exemple ».
8. **Contact** : formulaire établissement (nom, établissement, fonction, e-mail, téléphone, message), bloc patient séparé (lien vers l'espace sécurisé, FAQ, « En cas d'urgence : 15 »).

**Pages annexes** : FAQ patient, mentions légales, politique de confidentialité, cookies, déclaration d'accessibilité, notice d'utilisation et informations réglementaires du DM, page presse (kit média).

**À produire par l'agence** : tous les contenus. Rédaction web et textes patients en langage clair, relus avec les règles de la section 7 ; captures produit avec données fictives ; illustrations du parcours ; iconographie ; logo ou illustration au trait du bloc « Qui sommes-nous » ; entrées de démonstration des publications ; optimisation SEO. Pas de photo d'équipe, pas de logo partenaire.

## 7. Contraintes

### Marque et direction artistique (reprend le README)
- Ton : calme, rassurant, factuel.
- Palette : blanc chaud, vert sauge, bleu profond. **Pas de rouge**, sauf pour représenter une alerte.
- Typographie humaniste lisible : Atkinson Hyperlegible pour le texte, Source Sans 3 pour les titres, corps 18 px minimum.

### Réglementaire
- **Dispositif médical** : la communication reste conforme à la destination déclarée du DM. Pas de fenêtre « réservé aux professionnels » : les sections Preuves, Tableau de bord et Comité portent la mention « Information destinée aux professionnels de santé ». Le chemin patient (bloc patient, FAQ) ne contient aucun des éléments que l'ANSM interdit dans une publicité auprès du public : recommandation de scientifiques ou de professionnels de santé, effet présenté comme assuré, témoignage de guérison, insistance sur une certification ([ANSM, « Quelles règles sont spécifiques aux publicités auprès du public ? »](https://ansm.sante.fr/documents/reference/quelles-regles-sont-specifiques-aux-publicites-aupres-du-public), vu le 2026-11-13). L'agence relit chaque texte avec cette liste avant intégration.
- **Données de santé** : le site vitrine ne collecte **aucune** donnée de santé. L'espace patient est une application distincte, hébergée chez un hébergeur certifié HDS.
- **RGPD** : formulaires minimaux, mentions d'information, bandeau cookies conforme aux lignes directrices de la CNIL (refus aussi simple que l'acceptation), mesure d'audience configurée pour être exemptée de consentement.
- **Déontologie** : sous chaque membre du comité scientifique, une ligne « Liens d'intérêts » et un lien vers la base publique [Transparence Santé](https://www.transparence.sante.gouv.fr/), qui publie les conventions, rémunérations et avantages liant les entreprises et les acteurs de la santé (vu le 2026-11-13).

### Accessibilité
- Cible : RGAA 4.1 / WCAG 2.2 niveau AA, avec une déclaration d'accessibilité publiée.
- Texte 18 px minimum, contraste ≥ 4,5:1, cibles tactiles ≥ 44 × 44 px, navigation clavier, `prefers-reduced-motion` respecté, pas d'information portée par la seule couleur (niveau d'alerte = couleur + icône + texte).
- Les textes patients sont rédigés en langage clair (phrases courtes, pas de jargon) et testés auprès de 5 patients de plus de 65 ans.

### SEO
- Requêtes cibles : « télésurveillance chirurgie ambulatoire », « suivi post-opératoire à domicile », « suivi patient après ambulatoire », « RAAC suivi à distance ».
- Données structurées (Organization, FAQPage), balisage sémantique, une seule H1.

### Langues
- Français au lancement. Anglais en phase 2 (investisseurs, international), avec une structure i18n prévue dès le départ.

### Technique
- CMS headless pour les publications et la presse : pas d'extensions à maintenir côté site public. Hébergement en UE. Aucun script tiers publicitaire.

## 8. Plan de recherche utilisateur (mini)

- **Objectif** : vérifier que (1) chaque public trouve sa voie en moins de 10 secondes, (2) les preuves et la conformité convainquent un établissement, (3) un patient âgé comprend quoi faire et accède à son espace seul.
- **Méthode** : **5 tests d'usabilité modérés** sur une maquette Figma cliquable (fin S5) : 2 soignants ou décideurs (cadre de santé, directeur des opérations) à distance, et 3 patients de plus de 65 ans en présentiel, sur leur propre téléphone (un aidant peut assister). 45 minutes, enregistrement avec consentement, pensée à voix haute.
- **Tâches** : « Vous êtes cadre de santé : trouvez combien de temps l'outil prendra à votre équipe. » / « Trouvez la preuve qui vous convainc le plus. » / « Vous venez d'être opérée : trouvez comment accéder à votre questionnaire. » / « Que faites-vous si vous avez de la fièvre ce soir ? »
- **Mesures** : réussite de la tâche (oui, avec aide, non), temps, erreurs, verbatims, score de confiance de 1 à 5.

### Guide d'entretien en 5 temps

1. **Mise en route (5 min)**
   - « Pouvez-vous vous présenter en quelques mots, votre rôle ou votre situation ? »
   - « Quel est votre rapport aux outils numériques au quotidien ? »
2. **Contexte (10 min)**
   - Soignants : « Racontez-moi comment se passe aujourd'hui le suivi d'un patient après une sortie en ambulatoire. »
   - Patients : « Racontez-moi votre dernier retour à la maison après une intervention. Qu'est-ce qui vous a inquiété ? »
   - « Qui contactez-vous quand quelque chose ne va pas ? »
3. **Approfondissement (10 min)**
   - Soignants : « Qu'est-ce qui vous ferait refuser une solution de télésurveillance ? » / « Quelles preuves exigez-vous ? »
   - Patients : « Répondre à un questionnaire chaque jour, cela vous paraît-il faisable ? Par quel moyen ? »
   - « Quels mots vous inquiètent (surveillance, alerte, algorithme) ? »
4. **Réaction à la maquette (15 min)**
   - « Regardez cette page 5 secondes. Que fait cette entreprise, et pour qui ? »
   - Les tâches ci-dessus. Puis : « Qu'est-ce qui vous a manqué ou gêné ? »
   - « Sur une échelle de 1 à 5, quelle confiance accordez-vous à cette solution ? Pourquoi ? »
5. **Conclusion (5 min)**
   - « Si vous deviez changer une seule chose sur cette page, ce serait quoi ? »
   - « Y a-t-il une question qu'on ne vous a pas posée ? »

## 9. UX copy

### Titre du hero

**Recommandé** : « Sécuriser le retour à domicile après une chirurgie ambulatoire »
*Sous-titre* : « Chaque jour, votre patient répond à un court questionnaire. Votre équipe n'est alertée qu'en cas de signal anormal. »

| Option | Texte | Ton | Idéal pour |
|---|---|---|---|
| A | « Moins de réhospitalisations, plus de sorties le jour même » | Ambitieux, orienté résultat | **Écarté** : aucune étude publiée ne le démontre |
| B | « Rentrez chez vous. Votre équipe soignante veille avec vous. » | Chaleureux, direct | Bloc patient, campagne destinée aux patients |
| C | « 5 questions par jour pour le patient. Une alerte seulement quand c'est utile. » | Factuel, descriptif | Cadres de santé (salon, LinkedIn) |

### Libellés des CTA

| Emplacement | Libellé |
|---|---|
| Hero (établissement) | « Je suis un établissement » |
| Hero (patient) | « Je suis un patient » |
| Section tableau de bord | « Voir le tableau de bord en détail » |
| Section preuves | « Télécharger le dossier de preuves (PDF) » |
| Section publications | « Voir toutes les publications » |
| Formulaire établissement | « Demander une présentation » |
| Bloc patient | « Accéder à mon espace patient » |
| FAQ patient | « Lire les questions fréquentes » |

### Messages du formulaire établissement

**Succès** : « Merci, votre demande est bien envoyée. Nous vous répondons à l'adresse [e-mail saisi]. En attendant, vous pouvez consulter nos publications. »

**Erreurs** (structure : ce qui s'est passé, pourquoi, comment corriger)

| Cas | Message |
|---|---|
| E-mail invalide | « Cette adresse e-mail n'est pas valide : il manque le @ ou le nom de domaine. Exemple : prenom.nom@clinique-exemple.fr » |
| Champ obligatoire vide | « Le nom de l'établissement est manquant. Nous en avons besoin pour préparer la présentation. Indiquez-le pour continuer. » |
| Échec d'envoi | « Votre demande n'a pas pu être envoyée, car la connexion a été interrompue. Vos informations sont conservées : cliquez à nouveau sur « Demander une présentation » ou écrivez-nous à contact@[domaine]. » |

Règles : message sous le champ concerné, relié par `aria-describedby`, icône et texte en `color-alert`, focus déplacé sur le premier champ en erreur. Jamais « Erreur 500 » ni « Champ invalide » seuls.

## 10. Livrables

1. Cadrage et arborescence.
2. Wireframes mobile et desktop.
3. Maquettes UI (Figma) : home, FAQ patient, page légale type, avec les états des composants.
4. Mini design system : couleurs, typo, boutons, cartes de preuve, badges de conformité.
5. Illustrations du parcours (4).
6. Intégration responsive et CMS, formulaire établissement relié au CRM.
7. Audit d'accessibilité et corrections, déclaration d'accessibilité.
8. Recette, mise en ligne, documentation du CMS.

## 11. Planning indicatif

| Semaine | Étape |
|---|---|
| S1 | Cadrage, benchmark |
| S2-S3 | Arborescence, wireframes, rédaction des textes patients |
| S4-S5 | Maquettes UI, illustrations, relecture réglementaire des textes (section 7) |
| S6-S8 | Intégration, CMS, formulaires |
| S9 | Audit d'accessibilité, test avec 5 patients, corrections |
| S10 | Recette finale, mise en ligne |

Durée totale : **10 semaines**.

## 12. Budget

Pas de budget chiffré. Aucune grille tarifaire publique n'a été ouverte pour sourcer une fourchette, et l'entreprise est fictive. Le périmètre se lit dans les livrables (section 10) et le planning (section 11).

## 13. Critères de réussite

- Un établissement comprend **en moins de 10 secondes** ce que fait Veilla et pour qui (test des 5 secondes sur 10 soignants).
- Un patient de plus de 65 ans trouve **seul** comment accéder à son espace depuis un téléphone (4 testeurs sur 5).
- Chaque chiffre affiché a une source et une date. Chaque texte du chemin patient passe la liste de l'ANSM (section 7).
- Audit AA sans non-conformité bloquante. Lighthouse accessibilité ≥ 95.
- Les demandes de démo qualifiées sont suivies chaque mois, sans cible chiffrée.
- L'équipe publie une actualité ou une publication en moins de 10 minutes, sans l'agence.
