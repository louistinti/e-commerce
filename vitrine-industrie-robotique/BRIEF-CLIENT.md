# Brief client : site vitrine Vibra

> **Document de démonstration.** Vibra est une entreprise **fictive** créée pour le portfolio de l'agence. Aucun chiffre n'est inventé : toute donnée chiffrée affichée ici vient d'une source publique, citée à côté avec son URL et sa date de consultation. Les autres nombres sont des valeurs de conception (tailles, durées de planning, nombre de champs). Les noms de personnes et de sites sont fictifs. Le nom « Vibra » sert uniquement à cette démonstration et n'est pas destiné à être déposé.

Émetteur : direction de Vibra *(fictif)*
Destinataire : l'agence
Version : 1.1, novembre 2026

---

## 1. Qui nous sommes

- **Offre** : des capteurs vibratoires et de température sans fil, une passerelle 4G et un logiciel web d'alerte pour la maintenance prédictive des **PME industrielles**.
- **Promesse** : détecter une dégradation de machine tournante (roulement, balourd, désalignement, cavitation) avant la panne, assez tôt pour planifier l'intervention pendant un arrêt prévu.
- **Modèle** : un abonnement par point de mesure, capteurs compris, et un pilote court sur une machine.
- **Équipe** : basée à Saint-Étienne, avec des techniciens terrain par région.

## 2. Contexte et déclencheur

- Aujourd'hui, nos ventes passent par le bouche-à-oreille et les salons. Le site actuel est un template sans preuve ni fiche technique.
- Le déclencheur :
  - Nos premiers pilotes ont abouti à des clients qui acceptent de témoigner.
  - Une campagne commerciale régionale (Auvergne-Rhône-Alpes, Grand Est).
  - Le prochain salon Global Industrie.
- Nos acheteurs se méfient du marketing. Ils appellent, ils veulent voir une machine réelle et lire une fiche technique.

## 3. Objectifs business et indicateurs

| Objectif | Indicateur suivi |
|---|---|
| Générer des pilotes | Demandes « Tester sur une machine » qualifiées (site industriel, nombre de machines) |
| Faciliter le contact direct | Clics sur le bouton d'appel (mobile) |
| Équiper les prescripteurs | Téléchargements de la fiche technique PDF |
| Rassurer | Lecture des témoignages (défilement jusqu'à la section 6) |
| Convertir | Taux de transformation pilote en client (suivi CRM) |

Pas de cible chiffrée : l'entreprise est fictive, toute cible serait inventée. On suit l'évolution de chaque indicateur.

Mesure avec une analytics sans cookie et un suivi des événements (appel, PDF, formulaire). Les formulaires sont reliés au CRM HubSpot.

## 4. Cibles et personas

### P1 : Patrick, responsable maintenance dans une PME agroalimentaire (Loire)
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

### P2 : Sandrine, directrice d'usine en plasturgie (Ain)
- **Job to be done** : « Quand je dois défendre un budget devant la direction, je veux un chiffre d'arrêt évité et une référence comparable, pour engager un pilote sans prendre de risque. »
- **Elle attend** : le coût d'un arrêt, un engagement court (pilote), des références dans son secteur et un prix lisible.
- **Ses freins** : le retour sur investissement non prouvé, l'abonnement contre l'investissement, l'impact sur les équipes.
- **Elle veut voir** : le chiffre du coût d'arrêt, un témoignage d'une usine comparable avec le nom du site, et les conditions du pilote.

### P3 : Karim, responsable informatique et réseau industriel (groupe multisite)
- **Job to be done** : « Quand la maintenance veut installer des objets connectés, je veux comprendre l'architecture et les flux de données en 10 minutes, pour valider ou bloquer le projet en connaissance de cause. »
- **Il attend** : l'architecture (capteur, passerelle 4G, cloud), l'hébergement des données, la sécurité et la réversibilité.
- **Ses freins** : un objet connecté sur le réseau de l'usine, le cloud hors de l'UE, l'absence de documentation.
- **Il veut voir** : un schéma d'architecture, « aucune connexion au réseau usine », l'hébergement UE et une fiche sécurité téléchargeable.

## 5. Messages clés et preuves

| Message | Preuve à afficher |
|---|---|
| « Zéro arrêt surprise. » | Capture du logiciel montrant une tendance qui monte, l'alerte, puis l'intervention planifiée. Aucun délai d'anticipation chiffré : Vibra est fictive et n'a pas de mesure publiable. |
| « Installé sans câble, sans arrêter la ligne. » | 3 étapes dessinées au trait (fixation magnétique, activation de la passerelle, appairage) |
| « Une alerte = une machine, un défaut, une action. » | Capture du tableau de bord annotée |
| « Ça marche chez des industriels comme vous. » | 3 témoignages en HTML : nom, fonction, site, machine, sans portrait. Fictifs, et signalés comme tels sur la démo. |
| « Vos données restent en Europe et hors de votre réseau. » | Passerelle 4G autonome, hébergement UE, fiche sécurité |
| « Une heure d'arrêt a un coût. Calculez le vôtre. » | Chiffre de référence sourcé : une heure d'arrêt non planifié coûte 36 000 $ dans une grande usine de biens de grande consommation ([Siemens, *The True Cost of Downtime 2024*](https://assets.new.siemens.com/siemens/assets/api/uuid:1b43afb5-2d07-47f7-9eb7-893fe7d0bc59/TCOD-2024_original.pdf), vu le 2026-11-13), affiché avec son périmètre (grandes usines), puis un mini calculateur |

Règles : pas de « 100 % », pas de jargon IA, chaque chiffre a un périmètre et une source.

## 5 bis. UX copy

### Titre du hero

**Recommandé** : « Zéro arrêt surprise. »
Sous-titre : « Des capteurs de vibration sans fil qui vous alertent avant la panne. Posés sans câble, sans arrêter la ligne. »

| Option | Texte | Ton | Idéal pour |
|---|---|---|---|
| A | « Zéro arrêt surprise. » | Direct, promesse | Version par défaut (README) |
| B | « Vos machines vous préviennent avant de casser. » | Concret, bénéfice | Responsables maintenance, campagnes LinkedIn |
| C | « Combien vous coûte une heure d'arrêt ? » | Économique | Directeurs d'usine, landing page salon |

### Libellés des CTA

| Emplacement | Libellé | Pourquoi |
|---|---|---|
| Hero, primaire | « Tester sur une machine » | Une offre concrète, au lieu de « Demander une démo » |
| Hero, secondaire et barre fixe mobile | « Appeler un technicien » | Indique qui répond ; c'est le canal préféré des PME |
| Coût d'un arrêt | « Calculer mon coût d'arrêt » | Possessif, action immédiate |
| Fiche technique | « Télécharger la fiche technique (PDF, 2 pages) » | Format et longueur annoncés |
| Retours d'usine | « Lire le retour complet » | Spécifique |
| Formulaire | « Demander mon pilote » | Rappelle l'engagement limité |

### Messages du formulaire

- **Succès** : « Demande de pilote reçue. Merci, [Prénom]. [Nom du technicien régional] vous rappelle pour choisir la machine à équiper. Besoin plus urgent ? Appelez le [numéro]. »
- **Erreur de champ** (téléphone) : « Numéro de téléphone incomplet. Il faut 10 chiffres pour que le technicien puisse vous rappeler. Vérifiez le numéro (exemple : 04 77 00 00 00). »
- **Erreur d'envoi** (serveur) : « Votre demande n'a pas pu partir. La connexion avec notre serveur a été interrompue, et vos informations sont conservées. Réessayez, ou appelez-nous directement au [numéro]. »

Structure de chaque message : ce qui s'est passé, puis pourquoi, puis comment corriger.

## 6. Arborescence et contenus attendus

Le site est une page unique, plus la fiche technique, les mentions légales et une page de confirmation de pilote.

1. **Hero** : une photo d'atelier avec un cadrage serré sur le capteur posé, le titre « Zéro arrêt surprise », le CTA principal « Tester sur une machine » et le CTA secondaire « Appeler un technicien » (bouton fixe sur mobile).
2. **Le coût d'un arrêt** : un grand chiffre sourcé (Siemens TCOD 2024, voir section 5) et un calculateur à 2 champs (chiffre d'affaires horaire, heures d'arrêt par an).
3. **Installation en 3 étapes** : 3 dessins au trait, sans durée annoncée.
4. **Ce que voit le responsable maintenance** : une capture du tableau de bord annotée en 3 points (score de santé, tendance, alerte avec action).
5. **Secteurs** : agroalimentaire, plasturgie, métallurgie. Pour chacun : les machines typiques et le défaut typique.
6. **Retours d'usine** : 3 témoignages courts avec nom, fonction, site et machine, sans portrait.
7. **Fiche technique** : PDF de 2 pages maximum, téléchargeable sans formulaire, et un résumé HTML (IP, autonomie, plage de fréquence, température, certification).
8. **Qui sommes-nous, contact et pilote** :
   - Un bloc « Qui sommes-nous » court, sans photo, avec le logo : « Vibra conçoit à Saint-Étienne des capteurs de vibration sans fil et le logiciel qui les lit. Nos techniciens posent les capteurs chez vous et restent vos interlocuteurs. Vous parlez à quelqu'un qui connaît vos machines. »
   - Un formulaire court (nom, société, site, nombre de machines, téléphone), un numéro direct, le nom du technicien par région.

À produire par l'agence :
- La séance photo en atelier, cadrée serré sur le capteur posé (hero).
- Les 3 dessins d'installation au trait.
- Les captures du logiciel, avec des données de démonstration.
- La fiche technique de démonstration : rubriques et unités, sans valeur, puisque le capteur est fictif.
- Les 3 témoignages fictifs, signalés comme tels.

## 7. Contraintes

- **Marque** :
  - Palette : gris acier, blanc, jaune sécurité.
  - Typographie : Barlow Condensed pour les titres, Barlow pour le texte.
  - Pas de jaune en texte sur fond blanc.
  - Ne pas imiter la signalétique d'un fabricant de capteurs existant.
- **Données affichées** :
  - Aucune donnée machine réelle sur les captures : données de démonstration.
  - Aucun chiffre de résultat attribué à Vibra.
- **Conformité produit** : la fiche de démonstration n'affiche aucune certification (ATEX, CE, IP), puisque le produit n'existe pas.
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
| S1 | Atelier de cadrage, entretiens utilisateurs |
| S2 | Arborescence, wireframes, liste de plans photo |
| S3 | Séance photo en atelier, dessins d'installation, direction artistique |
| S4 | Maquettes desktop et mobile |
| S5-S6 | Intégration, calculateur, CRM, fiche technique |
| S7 | Recette (contenus, sources des chiffres, accessibilité, performance) |
| S8 | Mise en ligne, formation |

## 10. Budget

Pas de montant : aucune grille tarifaire publique n'a été ouverte pour ce périmètre, et l'entreprise est fictive. Les postes à chiffrer le moment venu :
- Design et intégration (Webflow ou WordPress).
- Stratégie, direction artistique, calculateur, liaison CRM, fiche technique.
- Séance photo en atelier et déplacements.
- Traduction EN de la fiche technique.

## 11. Critères de réussite

- Un responsable maintenance trouve en moins de 10 secondes sur mobile comment appeler et comment obtenir la fiche technique (test avec 5 utilisateurs terrain).
- Aucune photo de banque d'images sur le site.
- Lighthouse mobile ≥ 90, aucune erreur bloquante WCAG 2.2 AA.
- Les indicateurs de la section 3 sont suivis dès la mise en ligne.
- L'équipe ajoute seule un témoignage et met à jour la fiche technique.
- Chaque chiffre affiché a sa source et son périmètre.

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
   - « Vous voulez parler à quelqu'un tout de suite : que faites-vous ? » puis « Trouvez la plage de température du capteur dans la fiche technique. » (tâches chronométrées)
   - « Qu'est-ce qui sonne faux ou "marketing" sur cette page ? »
5. **Conclusion** (2 min)
   - « Qu'est-ce qui manque pour que vous demandiez un pilote ? »
   - « Connaissez-vous un collègue d'une autre usine que nous pourrions interroger ? »
