# Brief client : site vitrine Vibra

> **Document de démonstration.** Vibra est une entreprise **fictive** créée pour le portfolio de l'agence. Tous les chiffres, noms de sites et témoignages ci-dessous sont illustratifs et marqués *(fictif)*. Le nom est provisoire : une vérification INPI et EUIPO s'impose avant réutilisation, car « Vibra » est un terme courant dans le secteur des vibrations.

Émetteur : direction de Vibra *(fictif)*
Destinataire : l'agence
Version : 1.0, novembre 2026

---

## 1. Qui nous sommes

- **Offre** : des capteurs vibratoires et de température sans fil, une passerelle 4G et un logiciel web d'alerte pour la maintenance prédictive des **PME industrielles** (50 à 500 salariés).
- **Promesse** : détecter une dégradation de machine tournante (roulement, balourd, désalignement, cavitation) jusqu'à **3 semaines avant la panne** *(fictif : moyenne observée sur les pilotes 2025-2026, à documenter)*.
- **Modèle** : un abonnement par point de mesure, capteurs compris *(fictif)*, et un pilote de 6 semaines sur une machine.
- **Équipe** : 14 personnes à Saint-Étienne, dont 3 techniciens terrain *(fictif)*.

## 2. Contexte et déclencheur

- Aujourd'hui, nos ventes passent par le bouche-à-oreille et les salons. Le site actuel est un template sans preuve ni fiche technique.
- Le déclencheur :
  - 20 pilotes réalisés, dont 9 clients convertis, avec 6 accords de témoignage *(fictif)*.
  - Une campagne commerciale régionale (Auvergne-Rhône-Alpes, Grand Est) au T1 2027.
  - Le salon Global Industrie au printemps 2027.
- Nos acheteurs se méfient du marketing. Ils appellent, ils veulent voir une machine réelle et lire une fiche technique.

## 3. Objectifs business et KPIs

| Objectif | KPI | Cible à 6 mois |
|---|---|---|
| Générer des pilotes | Demandes « Tester sur une machine » qualifiées (site industriel, nombre de machines) | 12 par mois |
| Faciliter le contact direct | Clics sur le bouton d'appel (mobile) | 40 par mois |
| Équiper les prescripteurs | Téléchargements de la fiche technique PDF | 80 par mois |
| Rassurer | Lecture des témoignages (défilement jusqu'à la section 6) | 50 % des sessions |
| Convertir | Taux de transformation pilote en client | ≥ 45 % (suivi CRM) |

Mesure avec une analytics sans cookie et un suivi des événements (appel, PDF, formulaire). Les formulaires sont reliés au CRM (HubSpot ou Pipedrive).

## 4. Cibles et personas

### P1 : Patrick, responsable maintenance dans une PME agroalimentaire (180 salariés, Loire)
- **Job to be done** : « Quand une machine critique tombe en panne sans prévenir, je veux être averti assez tôt pour planifier l'intervention pendant un arrêt prévu, pour ne plus passer mes nuits à réparer dans l'urgence. »
- **Il attend** :
  - Une installation sans câblage ni arrêt de ligne.
  - Des alertes claires (quelle machine, quel défaut, quelle urgence).
  - Un export vers sa GMAO.
  - Un interlocuteur technique joignable.
- **Ses freins** :
  - « Encore un outil à surveiller. »
  - Les fausses alertes.
  - Le manque de temps et d'effectif.
  - Une mauvaise expérience avec un analyseur portatif.
- **Il veut voir** : une vraie photo de capteur posé sur un moteur, les 3 étapes d'installation, une capture d'alerte et un numéro de téléphone.

### P2 : Sandrine, directrice d'usine en plasturgie (320 salariés, Ain)
- **Job to be done** : « Quand je dois défendre un budget devant la direction, je veux un chiffre d'arrêt évité et une référence comparable, pour engager un pilote sans prendre de risque. »
- **Elle attend** : le coût d'un arrêt évité, un engagement court (pilote), des références dans son secteur et un prix lisible.
- **Ses freins** : le retour sur investissement non prouvé, l'abonnement contre l'investissement, l'impact sur les équipes.
- **Elle veut voir** : le chiffre du coût d'arrêt, un témoignage d'une usine comparable avec le nom du site, et les conditions du pilote.

### P3 : Karim, responsable informatique et réseau industriel (groupe de 3 sites)
- **Job to be done** : « Quand la maintenance veut installer des objets connectés, je veux comprendre l'architecture et les flux de données en 10 minutes, pour valider ou bloquer le projet en connaissance de cause. »
- **Il attend** : l'architecture (capteur, passerelle 4G, cloud), l'hébergement des données, la sécurité et la réversibilité.
- **Ses freins** : un objet connecté sur le réseau de l'usine, le cloud hors de l'UE, l'absence de documentation.
- **Il veut voir** : un schéma d'architecture, « aucune connexion au réseau usine », l'hébergement UE et une fiche sécurité téléchargeable.

## 5. Messages clés et preuves

| Message | Preuve à afficher |
|---|---|
| « Zéro arrêt surprise. » | Chiffre d'anticipation moyen sur les pilotes, avec son périmètre *(fictif : 19 jours en médiane, 34 défauts détectés)* |
| « Installé en 30 minutes, sans câble, sans arrêter la ligne. » | 3 étapes photographiées et minutées (fixation magnétique, activation de la passerelle, appairage) |
| « Une alerte = une machine, un défaut, une action. » | Capture du tableau de bord annotée |
| « Ça marche chez des industriels comme vous. » | 3 témoignages en HTML : photo, nom, fonction, site, machine *(fictif)* |
| « Vos données restent en Europe et hors de votre réseau. » | Passerelle 4G autonome, hébergement UE, fiche sécurité |
| « Un arrêt coûte plus cher qu'un an d'abonnement. » | Chiffre de référence sourcé (Siemens TCOD 2024, ABB) et un mini calculateur |

Règles : pas de « 100 % », pas de jargon IA, chaque chiffre a un périmètre.

## 5 bis. UX copy

### Titre du hero

**Recommandé** : « Zéro arrêt surprise. »
Sous-titre : « Des capteurs de vibration sans fil qui vous alertent jusqu'à 3 semaines avant la panne. Installés en 30 minutes, sans arrêter la ligne. »

| Option | Texte | Ton | Idéal pour |
|---|---|---|---|
| A | « Zéro arrêt surprise. » | Direct, promesse | Version par défaut (README) |
| B | « Vos machines préviennent 3 semaines avant de casser. » | Concret, bénéfice | Responsables maintenance, campagnes LinkedIn |
| C | « Une panne évitée paie un an d'abonnement. » | Économique | Directeurs d'usine, landing page salon |

### Libellés des CTA

| Emplacement | Libellé | Pourquoi |
|---|---|---|
| Hero, primaire | « Tester sur une machine » | Une offre concrète, au lieu de « Demander une démo » |
| Hero, secondaire et barre fixe mobile | « Appeler un technicien » | Indique qui répond ; c'est le canal préféré des PME |
| Coût d'un arrêt | « Calculer mon coût d'arrêt » | Possessif, action immédiate |
| Fiche technique | « Télécharger la fiche technique (PDF, 2 pages) » | Format et longueur annoncés |
| Retours d'usine | « Lire le retour complet » | Spécifique |
| Formulaire | « Demander mon pilote de 6 semaines » | Rappelle l'engagement limité |

### Messages du formulaire

- **Succès** : « Demande de pilote reçue. Merci, [Prénom]. [Nom du technicien régional] vous appelle sous 48 h ouvrées pour choisir la machine à équiper. Besoin plus urgent ? Appelez le [numéro]. »
- **Erreur de champ** (téléphone) : « Numéro de téléphone incomplet. Il faut 10 chiffres pour que le technicien puisse vous rappeler. Vérifiez le numéro (exemple : 04 77 00 00 00). »
- **Erreur d'envoi** (serveur) : « Votre demande n'a pas pu partir. La connexion avec notre serveur a été interrompue, et vos informations sont conservées. Réessayez, ou appelez-nous directement au [numéro]. »

Structure de chaque message : ce qui s'est passé, puis pourquoi, puis comment corriger.

## 6. Arborescence et contenus attendus

Le site est une page unique, plus la fiche technique, les mentions légales et une page de confirmation de pilote.

1. **Hero** : une photo d'atelier réelle avec un cadrage serré sur le capteur posé, le titre « Zéro arrêt surprise », le CTA principal « Tester sur une machine » et le CTA secondaire « Appeler un technicien » (bouton fixe sur mobile).
2. **Le coût d'un arrêt** : un grand chiffre sourcé et un calculateur à 2 champs (chiffre d'affaires horaire, heures d'arrêt par an).
3. **Installation en 30 minutes** : 3 étapes illustrées, chacune avec sa durée.
4. **Ce que voit le responsable maintenance** : une capture du tableau de bord annotée en 3 points (score de santé, tendance, alerte avec action).
5. **Secteurs** : agroalimentaire, plasturgie, métallurgie. Pour chacun : les machines typiques et le défaut typique.
6. **Retours d'usine** : 3 témoignages avec photo, nom et site.
7. **Fiche technique** : PDF de 2 pages maximum, téléchargeable sans formulaire, et un résumé HTML (IP, autonomie, plage de fréquence, température, certification).
8. **Contact et pilote** : formulaire court (nom, société, site, nombre de machines, téléphone), numéro direct, nom du commercial par région.

Contenus à fournir : photos d'atelier (une séance photo chez 2 clients, avec leur accord), captures du logiciel, fiche technique, témoignages validés par écrit, chiffres des pilotes.

## 7. Contraintes

- **Marque** :
  - Palette : gris acier, blanc, jaune sécurité.
  - Typographie : Barlow Condensed pour les titres, Barlow pour le texte.
  - Pas de jaune en texte sur fond blanc.
  - Ne pas imiter la signalétique d'un fabricant de capteurs existant.
- **Confidentialité** :
  - Les témoignages et photos ne se publient qu'avec un accord écrit.
  - Aucune donnée machine réelle d'un client sur les captures (anonymiser).
- **Conformité produit** : ne mentionner une certification (ATEX, CE, IP) que si elle est obtenue, avec sa référence.
- **Accessibilité** :
  - Viser WCAG 2.2 AA.
  - Cibles tactiles de 48 px minimum, car l'usage se fait aussi sur le terrain avec des gants ou sur tablette.
  - Contrastes vérifiés, alternatives textuelles pour les photos et les captures.
- **SEO** : requêtes « maintenance prédictive PME », « capteur vibration sans fil », « surveillance roulement moteur », « analyse vibratoire » et requêtes régionales. Données structurées Organization et Product.
- **Langues** : FR au lancement. EN en phase 2 (fiche technique EN dès le lancement pour les groupes).
- **Technique** :
  - Lighthouse mobile ≥ 90.
  - Photos en AVIF/WebP, avec un poids de page inférieur à 1,5 Mo.
  - Hébergement UE, sans cookie tiers.
  - CMS simple pour ajouter un témoignage.

## 8. Livrables

- Arborescence et wireframes.
- Maquettes desktop et mobile (Figma).
- Direction de la séance photo : liste de plans et cadrages serrés.
- Le site intégré, avec le CMS, le calculateur et le formulaire relié au CRM.
- La mise en page de la fiche technique (PDF de 2 pages).
- Une recette accessibilité et performance, et une formation de 1 h.

## 9. Planning indicatif (8 semaines)

| Semaines | Étape |
|---|---|
| S1 | Atelier, collecte, entretiens avec 2 clients |
| S2 | Arborescence, wireframes, liste de plans photo |
| S3 | Séance photo (1 à 2 jours sur site), direction artistique |
| S4 | Maquettes desktop et mobile |
| S5-S6 | Intégration, calculateur, CRM, fiche technique |
| S7 | Recette (contenus, accessibilité, performance, validation juridique des témoignages) |
| S8 | Mise en ligne, formation |

## 10. Budget

Fourchettes indicatives en France (2026). Ce sont des estimations de l'agence, pas des chiffres sourcés.
- **Freelance** (design et intégration Webflow ou WordPress, FR) : 4 000 à 8 000 € HT.
- **Studio ou agence** (stratégie, DA, intégration, calculateur, CRM, fiche technique) : 10 000 à 22 000 € HT.
- **Séance photo industrielle** : 1 200 à 2 500 € par jour, plus les déplacements.
- **Traduction EN de la fiche technique** : environ 300 à 600 €.
- Enveloppe validée par le client *(fictif)* : **16 000 € HT, photos comprises**.

## 11. Critères de réussite

- Un responsable maintenance trouve en moins de 10 secondes sur mobile comment appeler et comment obtenir la fiche technique (test avec 5 utilisateurs terrain).
- Aucune photo de banque d'images sur le site.
- Lighthouse mobile ≥ 90, aucune erreur bloquante WCAG 2.2 AA.
- Les KPIs de la section 3 sont atteints à 6 mois.
- L'équipe ajoute seule un témoignage et met à jour la fiche technique.
- Chaque chiffre affiché est sourcé ou documenté (pilotes) et validé par la direction.

## 12. Mini plan de recherche utilisateur

- **Objectif** :
  - Vérifier qu'un responsable maintenance comprend l'offre, trouve le téléphone et la fiche technique en moins de 10 s sur mobile.
  - Vérifier qu'une directrice d'usine juge la preuve suffisante pour engager un pilote.
  - Identifier les objections non traitées (informatique, fausses alertes, prix).
- **Méthode** :
  - S1 : 5 entretiens sur site ou par téléphone de 30 min (3 responsables maintenance, 1 directeur d'usine, 1 responsable informatique), choisis parmi les clients pilotes et les prospects.
  - S4 : 5 tests d'usabilité du prototype mobile, si possible en atelier sur le smartphone du participant.
- **Incitation** : une visite technique offerte, ou un mois d'abonnement.
- **Livrable** : une synthèse de 2 pages (thèmes, verbatims, objections, 5 recommandations priorisées).

**Guide d'entretien en 5 temps** (30 min)

1. **Mise en route** (3 min)
   - « Pouvez-vous décrire votre poste et le parc machines dont vous êtes responsable ? »
   - « Combien de personnes dans votre équipe maintenance ? »
2. **Contexte** (7 min)
   - « Racontez-moi la dernière panne imprévue : quelle machine, combien de temps d'arrêt, comment vous l'avez gérée ? »
   - « Comment surveillez-vous vos machines aujourd'hui (rondes, analyseur portatif, prestataire) ? »
3. **Approfondissement** (10 min)
   - « Quand vous cherchez une solution technique, où regardez-vous en premier : le site, un collègue, un salon, un commercial ? »
   - « Qu'est-ce qui vous a déjà fait renoncer à un outil connecté ? »
   - « Quel chiffre ou quelle preuve vous ferait dire "on essaie" ? »
4. **Réaction à la maquette** (8 min)
   - « Regardez cette page 5 secondes sur votre téléphone. Que vend cette entreprise ? »
   - « Vous voulez parler à quelqu'un tout de suite : que faites-vous ? » puis « Trouvez la température maximale du capteur. » (tâches chronométrées)
   - « Qu'est-ce qui sonne faux ou "marketing" sur cette page ? »
5. **Conclusion** (2 min)
   - « Qu'est-ce qui manque pour que vous demandiez un pilote ? »
   - « Connaissez-vous un collègue d'une autre usine que nous pourrions interroger ? »
