# Brief client : site vitrine Strate Orbital

> **Document de démonstration.** Strate Orbital est une entreprise **fictive** créée pour le portfolio de l'agence. Tous les chiffres, dates, noms et partenariats ci-dessous sont illustratifs et marqués *(fictif)*. Le nom est provisoire : une vérification INPI et EUIPO s'impose avant toute réutilisation.

Émetteur : direction générale de Strate Orbital *(fictif)*
Destinataire : l'agence
Version : 1.0, novembre 2026

---

## 1. Qui nous sommes

- **Mission** : mesurer l'humidité des sols depuis l'espace, chaque jour, à l'échelle de la parcelle, pour l'agriculture et la gestion de l'eau.
- **Technologie** : une constellation de nanosatellites (format 6U) qui mesurent l'humidité par réflectométrie des signaux GNSS en bande L (GNSS-R). Les données sont fusionnées avec des modèles hydrologiques et calibrées sur des sondes au sol.
- **Origine** : un essaimage d'un laboratoire public de recherche en géophysique spatiale, créé en 2024 *(fictif)*, avec 18 personnes à Toulouse *(fictif)*.
- **Statut** : un démonstrateur en orbite depuis 2026, et une constellation de 12 satellites visée pour 2028 *(fictif)*.

## 2. Contexte et déclencheur

- Notre site actuel est une page unique en anglais, faite au lancement. Elle ne montre ni la donnée ni l'équipe.
- Le déclencheur : la préparation de notre série A (cible du 1er semestre 2027 *(fictif)*), trois appels d'offres publics (agences de l'eau, régions) et 6 recrutements d'ingénieurs en 2027.
- Les investisseurs et les acheteurs nous jugent sur le site avant le premier rendez-vous. Les levées spatiales européennes ont atteint des niveaux records au premier semestre 2026 et la concurrence pour l'attention est forte.

## 3. Objectifs business et KPIs

| Objectif | KPI | Cible à 6 mois après la mise en ligne |
|---|---|---|
| Générer des contacts partenaires qualifiés | Formulaires « Contact partenaires » avec un type d'organisation renseigné | 15 par mois |
| Appuyer la levée | Téléchargements du dossier investisseurs (sur demande) et rendez-vous obtenus | 40 demandes |
| Recruter | Candidatures via les offres de la home | 25 par offre |
| Crédibiliser auprès des acheteurs publics | Visites de la page Données d'au moins 60 s | 35 % des sessions |
| Presse | Téléchargements du kit presse | 20 par trimestre |

Les mesures se font avec une analytics sans cookie (Plausible ou Matomo en mode exemption CNIL) et un suivi des événements sur les CTA.

## 4. Cibles et personas

### P1 : Claire, associée dans un fonds deeptech (Paris ou Munich)
- **Job to be done** : « Quand je reçois un deck spatial, je veux vérifier en 5 minutes que la techno est réelle et que l'équipe sait livrer, pour décider si je prends un premier rendez-vous. »
- **Elle attend** : le niveau de maturité technologique (TRL), une roadmap réaliste, la traction commerciale (lettres d'intention, pilotes), l'équipe et la propriété intellectuelle.
- **Ses freins** : le risque de lancement, la dépendance aux subventions, un marché agricole jugé lent à payer.
- **Ce qu'elle doit trouver en 30 s** : la mission, une preuve en orbite, le marché adressable, et un contact.

### P2 : Marc, responsable du service données dans une agence de l'eau
- **Job to be done** : « Quand je prépare un marché de suivi de la sécheresse, je veux savoir si cette donnée est fiable, documentée et livrable dans mes formats, pour l'inscrire au cahier des charges sans risque. »
- **Il attend** : la résolution, la revisite, la validation au sol, les formats (GeoTIFF, API, WMS), la continuité de service et la conformité aux marchés publics.
- **Ses freins** : « encore un fournisseur de démonstrateurs », l'absence de publication scientifique, la souveraineté des données.
- **Ce qu'il doit trouver** : un exemple de carte sur son type de territoire, une fiche technique, les publications et un contact technique nommé.

### P3 : Inès, ingénieure GNC ou traitement du signal, 5 ans d'expérience dans un grand groupe
- **Job to be done** : « Quand j'envisage de quitter un grand groupe, je veux voir des problèmes techniques concrets et des lancements datés, pour juger si le projet est sérieux avant de postuler. »
- **Elle attend** : des problèmes techniques intéressants, des lancements concrets, l'équipe, le télétravail, et le salaire ou le BSPCE.
- **Ses freins** : la stabilité d'une startup, le salaire comparé à un grand groupe, la peur d'un projet « slideware ».
- **Ce qu'elle doit trouver** : 3 offres précises avec le problème à résoudre, des visages, et la timeline des lancements.

## 5. Messages clés et preuves

| Message | Preuve à afficher |
|---|---|
| « L'humidité des sols, chaque jour, à la parcelle. » | Exemple de carte et chiffres de résolution et de revisite *(fictif : 1 km natif, 100 m affiné, revisite 24 h en 2028)* |
| « Une mesure, pas une estimation. » | Courbe de comparaison avec les sondes au sol, et une publication évaluée par les pairs (lien DOI) |
| « Déjà en orbite. » | Timeline : démonstrateur SO-1 lancé en 2026 *(fictif)*, première image datée |
| « Des données utiles pour l'eau, l'agriculture et l'assurance climatique. » | 3 cas d'usage avec la décision rendue possible (irrigation, alerte sécheresse, indice paramétrique) |
| « Soutenus par des acteurs publics européens. » | Logos **avec la nature exacte du soutien** (« lauréat de l'appel X », « contrat d'étude ESA ») et un accord écrit pour chaque logo |

Règle : chaque chiffre est daté et sourcé, et chaque vue d'artiste est légendée.

## 5 bis. UX copy

### Titre du hero

**Recommandé** : « L'humidité des sols, mesurée depuis l'espace, chaque jour. »
Sous-titre : « Une constellation de nanosatellites pour piloter l'irrigation, anticiper la sécheresse et assurer le risque climatique. »

| Option | Texte | Ton | Idéal pour |
|---|---|---|---|
| A | « L'humidité des sols, mesurée depuis l'espace, chaque jour. » | Factuel, précis | Toutes cibles : version par défaut |
| B | « Voir la sécheresse avant qu'elle ne se voie. » | Narratif, bénéfice | Acheteurs publics, presse |
| C | « Soil moisture from orbit. Daily. Field-scale. » | Technique, sec | Version EN, investisseurs et ingénieurs |

### Libellés des CTA

| Emplacement | Libellé | Pourquoi |
|---|---|---|
| Hero, primaire | « Contacter l'équipe partenariats » | Le verbe et le destinataire sont explicites, au lieu d'un simple « Contact » |
| Hero, secondaire | « Explorer la carte d'exemple » | Il annonce ce qu'on va voir |
| Technologie | « Lire les publications » | Spécifique au niveau 3 |
| Timeline | « Suivre nos lancements » (inscription à la lettre d'information) | Engagement léger |
| Recrutement | « Voir les 3 postes ouverts » | Le chiffre crée de la concrétude |
| Presse | « Télécharger le kit presse (ZIP, 12 Mo) » | Le format et le poids sont annoncés |
| Formulaire | « Envoyer ma demande » | Première personne, action claire |

### Messages du formulaire

- **Succès** : « Demande envoyée. Merci, [Prénom]. Votre message est arrivé à l'équipe partenariats : nous répondons sous 2 jours ouvrés. En attendant, vous pouvez explorer la carte d'exemple. »
- **Erreur de champ** (e-mail) : « Adresse e-mail incomplète. Il manque le domaine après le @ : vérifiez-la (exemple : prenom@organisation.fr). »
- **Erreur d'envoi** (serveur) : « Votre demande n'a pas pu être envoyée. La connexion avec notre serveur a échoué, et vos informations sont conservées. Réessayez dans un instant ou écrivez directement à partenaires@[domaine]. »

Structure de chaque message : ce qui s'est passé, puis pourquoi, puis comment corriger.

## 6. Arborescence et contenus attendus

Le site est une page unique avec des ancres, plus des pages légales et des offres d'emploi en pages filles.

1. **Hero** : un visuel orbital léger (SVG animé ou une seule scène 3D sur desktop), la phrase de mission, le CTA principal « Contacter l'équipe partenariats » (évolution du « Contact partenaires » du README) et le CTA secondaire « Explorer la carte d'exemple ».
2. **La technologie à 3 niveaux** : onglets « En bref » (3 phrases et un schéma), « Pour les ingénieurs » (GNSS-R, chaîne de traitement, bilan de précision) et « Publications » (liste avec DOI).
3. **Applications** : agriculture (irrigation), eau (gestion de la ressource, alerte sécheresse), assurance climatique (indice paramétrique). Pour chacune : le problème, la donnée fournie et la décision rendue possible.
4. **Feuille de route** : une timeline horizontale à défilement lent sur desktop et verticale sur mobile, avec les statuts *réalisé / partiel / à venir*.
5. **Données** : une carte d'exemple avec un curseur temporel sur 30 jours, une légende accessible et un tableau de valeurs en alternative.
6. **Partenaires et financeurs** : des logos sobres en monochrome, avec la nature du soutien au survol et en texte.
7. **Équipe et recrutement** : 6 portraits, 3 offres et un lien vers la page carrière.
8. **Presse et contact** : 3 retombées, un kit presse (ZIP), un formulaire segmenté (investisseur / client / presse / candidat), une adresse et un plan.

Contenus à fournir par le client : textes validés FR/EN, photos d'équipe (séance photo à prévoir), données de carte (échantillon exportable), publications, logos avec autorisations et fiches de poste.

## 7. Contraintes

- **Marque** : un logotype provisoire. Pas d'emprunt à l'identité d'une agence spatiale ni d'un concurrent.
  - Palette : noir profond, blanc, orange signal.
  - Typographie : IBM Plex Sans et IBM Plex Mono.
  - Mode sombre par défaut, avec une bascule vers le mode clair.
- **Confidentialité** :
  - Aucune spécification de charge utile au-delà de ce qui a été publié.
  - Aucun client nommé sans accord.
  - Le dossier investisseurs se demande par formulaire et n'est pas en libre accès.
- **Export et double usage** : faire relire les contenus techniques avant publication, au regard du règlement (UE) 2021/821 sur les biens à double usage et de nos obligations contractuelles (ESA, CNES).
- **Accessibilité** :
  - Viser WCAG 2.2 AA. Les acheteurs publics peuvent demander une déclaration d'accessibilité.
  - Animations désactivables (`prefers-reduced-motion`), carte doublée d'un tableau, contrastes vérifiés (l'orange n'est jamais utilisé pour du texte courant sur fond clair).
- **SEO** : requêtes cibles sur « humidité des sols satellite », « soil moisture data API », « sécheresse agricole données ». Balises hreflang FR/EN, données structurées Organization et JobPosting.
- **Langues** : FR et EN complets au lancement. L'anglais est la langue par défaut pour le trafic hors de France.
- **Technique** :
  - Performance : Lighthouse mobile ≥ 90 et LCP < 2,5 s.
  - Hébergement dans l'UE, sans cookie tiers.
  - CMS éditable par l'équipe (Webflow, Framer ou Astro avec un CMS headless).

## 8. Livrables

- Plateforme de messages et arborescence validées.
- Maquettes desktop et mobile (Figma) avec un mini système de design (couleurs, typo, composants).
- Le site intégré FR/EN, avec le CMS et la timeline et les offres d'emploi éditables.
- Le module carte (tuiles statiques et curseur temporel).
- Le kit presse (logos, photos, fiche entreprise).
- Une formation à l'édition (1 h) et la documentation.
- La recette accessibilité et performance.

## 9. Planning indicatif (10 semaines)

| Semaines | Étape |
|---|---|
| S1 | Atelier de cadrage, collecte des contenus, audit |
| S2 | Plateforme de messages, arborescence, wireframes |
| S3-S4 | Direction artistique (2 pistes, puis 1), maquettes desktop |
| S5 | Maquettes mobile, prototype de la timeline et de la carte |
| S6-S8 | Intégration, CMS, module carte, traductions |
| S9 | Recette (contenus, accessibilité, performance, double usage) |
| S10 | Mise en ligne, formation, suivi analytics |

## 10. Budget

Fourchettes indicatives en France (2026). Ce sont des estimations de l'agence, pas des chiffres sourcés.
- **Freelance senior** (design et intégration Webflow ou Framer, FR/EN, carte simple) : 6 000 à 12 000 € HT.
- **Studio ou agence** (stratégie, DA, intégration, module carte, recette accessibilité) : 15 000 à 35 000 € HT.
- **En sus** : séance photo de l'équipe (1 jour, 1 500 à 3 000 €), traduction professionnelle EN (environ 0,12 à 0,20 € par mot), hébergement et CMS (300 à 800 € par an).
- Enveloppe validée par le client *(fictif)* : **25 000 € HT tout compris**.

## 11. Critères de réussite

- Un investisseur comprend la mission, la preuve en orbite et la manière de nous contacter en moins de 30 secondes (test avec 5 personnes).
- Un ingénieur trouve le niveau technique et les publications en 2 clics.
- Lighthouse mobile ≥ 90, aucune erreur bloquante à l'audit WCAG 2.2 AA.
- Les KPIs de la section 3 sont atteints à 6 mois.
- L'équipe publie seule une actualité, un jalon de timeline et une offre d'emploi.
- Aucun contenu retiré après la relecture juridique (double usage, logos).

## 12. Mini plan de recherche utilisateur

- **Objectif** : vérifier que chaque persona trouve en moins de 30 s la preuve dont il a besoin (P1 : la preuve en orbite et le contact ; P2 : la fiche technique et les publications ; P3 : les postes et les lancements), et que le niveau « En bref » est compris sans jargon.
- **Méthode** :
  - S2 : 5 entretiens semi-directifs de 30 min (2 investisseurs, 2 acheteurs publics ou agricoles, 1 ingénieur), en visio.
  - S5 : 5 tests d'usabilité sur le prototype Figma, avec des tâches chronométrées.
- **Recrutement** : le réseau du client (business angels, partenaires d'études), une association professionnelle de l'eau et LinkedIn pour les ingénieurs. Incitation : un compte rendu des résultats, ou un bon de 50 €.
- **Livrable** : une synthèse de 2 pages (thèmes, verbatims, 5 recommandations priorisées).

**Guide d'entretien en 5 temps** (30 min)

1. **Mise en route** (3 min)
   - « Pouvez-vous présenter votre rôle et ce sur quoi vous travaillez en ce moment ? »
   - « Combien de dossiers ou de fournisseurs spatiaux voyez-vous par mois, à peu près ? »
2. **Contexte** (7 min)
   - « La dernière fois que vous avez évalué une startup ou une donnée satellitaire, comment vous y êtes-vous pris ? »
   - « Quel rôle a joué son site web dans cette évaluation ? »
3. **Approfondissement** (10 min)
   - « Qu'est-ce qui vous a fait douter d'un acteur spatial par le passé ? »
   - « Quelle preuve vous convainc le plus : une publication, une image en orbite, un client, un financeur ? Pourquoi ? »
   - « Qu'est-ce qui vous ferait fermer l'onglet ? »
4. **Réaction à la maquette** (8 min)
   - « Regardez cette page 5 secondes. Que fait cette entreprise ? » (test des 5 secondes)
   - « Trouvez où contacter l'équipe pour un partenariat ou postuler. » (tâche chronométrée, verbalisation à voix haute)
   - « Qu'est-ce qui vous manque pour passer à l'étape suivante ? »
5. **Conclusion** (2 min)
   - « Si vous ne deviez changer qu'une chose sur cette page, ce serait quoi ? »
   - « Y a-t-il quelqu'un d'autre que nous devrions interroger ? »
