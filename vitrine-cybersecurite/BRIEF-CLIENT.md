# Brief client : site vitrine Rempart

> Document de travail. **Rempart est une entreprise fictive** créée pour un site de démonstration. Les chiffres internes (clients, délais, prix) sont des hypothèses à remplacer par celles du vrai client. Les certifications citées servent d'exemples et ne doivent pas être affichées sans justificatif.

Émetteur : Rempart, direction générale et marketing
Destinataire : l'agence
Date : novembre 2026

---

## 1. Présentation de l'entreprise

- **Activité** : surveillance de sécurité 24/7 (SOC managé) pour PME et ETI de 20 à 500 postes. L'offre comprend la détection, la réponse à incident, des sauvegardes supervisées, la sensibilisation des équipes et l'accompagnement à la conformité NIS2.
- **Modèle** : abonnement mensuel à **prix fixe par poste**, sans frais de mise en service au-delà de 50 postes (hypothèse).
- **Promesse** : « Votre PME surveillée 24 h/24, sans recruter d'équipe sécurité. »
- **Équipe (hypothèse)** : 25 personnes, dont 12 analystes SOC basés en France et un SOC Manager attitré par client.

## 2. Contexte et déclencheur

- NIS2 fait passer le nombre d'entités régulées en France d'environ 500 à environ 15 000. La loi « Résilience » est attendue pour fin 2026. Les dirigeants de PME nous demandent « est-ce que je suis concerné ? » avant même de parler sécurité.
- Le site actuel (hypothèse) est une plaquette de 2019 : jargon technique, aucun prix, un formulaire « contact » unique. Il génère moins de 5 demandes qualifiées par mois.
- Nos commerciaux passent leurs premiers rendez-vous à expliquer les bases. Nous voulons que le site fasse ce travail.

## 3. Objectifs business et KPIs

| Objectif | KPI | Cible à 6 mois |
|---|---|---|
| Générer des leads qualifiés | Demandes de diagnostic gratuit | 30 par mois |
| Activer le quiz comme capteur de leads | Taux de complétion du test express | ≥ 55 % des quiz démarrés |
| | Quiz terminés puis rapport demandé | ≥ 25 % |
| Rendre l'urgence accessible | Appels sur le numéro d'urgence depuis le site (suivi d'appels) | Suivi, sans cible |
| Raccourcir le cycle de vente | Leads ayant consulté la grille tarifaire avant le RDV | ≥ 60 % |
| Visibilité | Positions top 10 sur « SOC managé PME », « NIS2 PME », « surveillance cybersécurité PME » | 3 requêtes sur 5 |
| Performance | Core Web Vitals en vert sur mobile | 100 % des pages |

## 4. Cibles et personas

### Persona 1 : Claire, 52 ans, dirigeante d'une PME industrielle (120 salariés)
- **Job to be done** : « Quand un client me demande des garanties cyber, je veux savoir vite où j'en suis et quoi répondre, pour ne pas perdre le contrat. »
- **Situation** : un client donneur d'ordre lui envoie un questionnaire « sécurité fournisseurs NIS2 ».
- **Freins** : elle ne comprend pas le vocabulaire, craint un budget sans fond et se méfie des vendeurs de peur.
- **Attentes** : savoir en 2 minutes si elle est concernée, avoir un prix, un interlocuteur humain et une réponse à donner à son client.
- **Ce qui la convertit** : le quiz, la grille tarifaire, la checklist NIS2 et un témoignage d'un pair.

### Persona 2 : Karim, 38 ans, responsable informatique seul (ETI de services, 300 postes)
- **Job to be done** : « Quand une alerte tombe la nuit ou pendant mes congés, je veux que quelqu'un de compétent la traite, pour ne plus porter seul ce risque. »
- **Situation** : il gère tout seul l'infrastructure, les postes et le support. Il ne peut pas surveiller les alertes la nuit.
- **Freins** : il a peur de perdre la main, doute de la qualité des analystes et redoute un déploiement lourd.
- **Attentes** : un périmètre précis (ce qui est couvert, ce qui ne l'est pas), le délai de prise en charge, un rapport mensuel, la compatibilité avec ses outils et la réversibilité.
- **Ce qui le convertit** : la section « Ce que couvre l'offre » détaillée, la timeline d'attaque, les certifications, un exemple de rapport.

### Persona 3 : Laurent, 45 ans, dirigeant d'une PME attaquée ce matin
- **Job to be done** : « Quand mon entreprise est bloquée par une attaque, je veux joindre un expert en moins d'une minute, pour limiter les dégâts. »
- **Situation** : les écrans affichent une demande de rançon et il cherche « aide cyberattaque » sur mobile.
- **Freins** : la panique, aucun temps pour lire.
- **Attentes** : un numéro tout de suite, quelqu'un qui décroche, et les trois premiers gestes.
- **Ce qui le convertit** : le bouton « Urgence : nous appeler » fixe et le bloc « Les 3 réflexes en attendant notre appel ».

## 5. Messages clés et preuves

| Message | Preuve à afficher |
|---|---|
| Surveillé 24 h/24 par des humains, en France | Photo réelle de l'équipe (pas de banque d'images), nombre d'analystes, localisation du SOC |
| On agit, on ne fait pas qu'alerter | Timeline minute par minute et délai moyen de prise en charge (à mesurer) |
| Un prix clair, sans surprise | Grille par poste et simulateur « nombre de postes → prix mensuel » |
| NIS2 sans jargon | Test « Suis-je concerné ? » et checklist PDF datée |
| Sérieux et certifié | ISO 27001 et qualification ANSSI (PDIS pour la détection, PRIS pour la réponse) **uniquement si obtenues**. Sinon, afficher les partenaires technologiques. |
| Des PME comme vous | 3 témoignages avec nom, fonction, secteur et taille d'entreprise |

## 6. Arborescence et contenus attendus

Le site est un one-page avec ancres, plus 4 pages annexes pour le SEO et les obligations légales.

1. **Hero** : titre, sous-titre (« Détection, réponse et conformité NIS2, à prix fixe par poste »), CTA « Faire le test (2 min) », CTA secondaire « Demander mon diagnostic gratuit » et le numéro d'urgence en haut à droite.
2. **Test express** : 5 questions (sauvegardes testées, double authentification, mises à jour, sensibilisation, personne d'astreinte). Le résultat donne un niveau (faible, moyen, élevé) et 3 recommandations, sans e-mail. Le rapport détaillé est envoyé contre un e-mail.
3. **Ce que couvre l'offre** : 4 cartes (Détection, Réponse, Sauvegarde, Formation) et un encart « Ce qui n'est pas inclus ».
4. **En cas d'attaque** : une timeline en 6 étapes (T+0 alerte, T+5 min analyse, T+15 min isolement du poste, T+30 min appel du dirigeant, T+4 h restauration, J+2 rapport). Les délais sont des hypothèses à valider.
5. **NIS2 expliquée** : 3 paragraphes, le test « Suis-je concerné ? » et la checklist PDF, avec la mention « Transposition française en cours, mis à jour le [date] ».
6. **Certifications et partenaires**.
7. **Tarifs** : 3 paliers par poste et par mois (Essentiel, Pro, NIS2), avec un simulateur. Les montants de la démo sont fictifs : 12, 19 et 27 € HT par poste et par mois, à calibrer.
8. **Contact** : un bloc urgence (numéro en rouge discret, disponible 24/7) et un formulaire de diagnostic (nom, entreprise, nombre de postes, téléphone, créneau).

Pages annexes : mentions légales, politique de confidentialité, gestion des cookies, page « NIS2 pour les PME » (version longue, cible SEO) et page « Urgence cyberattaque » (pour la recherche mobile).

Contenus fournis par Rempart : textes validés, photos d'équipe, logos partenaires, certificats, 3 témoignages, grille tarifaire. L'agence fournit la rédaction SEO, les icônes et les illustrations (schémas, pas de personnages menaçants).

## 7. Plan de recherche utilisateur (mini)

- **Objectif** : vérifier qu'un dirigeant non technique comprend l'offre, fait confiance au prix affiché et termine le quiz. Vérifier aussi que le numéro d'urgence se trouve en moins de 5 secondes sur mobile.
- **Méthode** : 5 entretiens de 45 min avec des dirigeants et responsables informatiques de PME de 20 à 300 postes (2 personas Claire, 2 personas Karim, 1 dirigeant déjà attaqué). Ensuite, 5 tests d'usabilité modérés sur la maquette mobile (S3), avec 3 tâches : faire le test, trouver le prix pour 80 postes, appeler en urgence.
- **Recrutement** : le réseau du client, une CCI ou un club d'entreprises. Une incitation de 50 € en bon d'achat (hypothèse).

**Guide d'entretien en 5 temps**

| Temps | Durée | Questions |
|---|---|---|
| 1. Mise en route | 5 min | Présentez votre entreprise et votre rôle en deux mots. Qui s'occupe de l'informatique chez vous aujourd'hui ? |
| 2. Contexte | 10 min | Racontez la dernière fois que vous avez pensé à la cybersécurité : qu'est-ce qui l'a déclenché ? Un client ou un assureur vous a-t-il déjà demandé des garanties ? Que savez-vous de NIS2 ? |
| 3. Approfondissement | 15 min | Comment choisiriez-vous un prestataire de sécurité : qui consultez-vous, que regardez-vous ? Qu'est-ce qui vous ferait fuir sur un site de ce type ? Quel budget vous semble raisonnable par poste et par mois ? |
| 4. Réaction à la maquette | 10 min | (Hero affiché 5 s, puis masqué.) Que propose cette entreprise ? (Quiz.) Faites le test à voix haute : quelle question vous gêne ? (Tarifs.) Ce prix vous paraît-il complet ? Que manque-t-il ? |
| 5. Conclusion | 5 min | Si vous ne deviez retenir qu'une chose de ce site, ce serait quoi ? Qu'est-ce qui vous ferait demander un diagnostic aujourd'hui ? |

## 8. UX copy

**Titre du hero recommandé** : « Votre PME surveillée 24 h/24, sans recruter d'équipe sécurité »
Sous-titre : « Détection, réponse et préparation NIS2, à prix fixe par poste. Des analystes en France vous appellent avant que ça dégénère. »

| Option | Texte | Ton | Idéal pour |
|---|---|---|---|
| A | « Des experts veillent sur votre PME, jour et nuit » | Rassurant, humain | Les dirigeants inquiets, peu techniques (Claire) |
| B | « Une alerte à 3 h du matin ? On s'en occupe. » | Direct, concret | Le responsable informatique seul (Karim), les campagnes LinkedIn |
| C | « NIS2 : êtes-vous concerné ? Réponse en 2 minutes » | Pédagogique, opportuniste | Les landing pages SEO et publicitaires NIS2 |

**Libellés des CTA**

| Emplacement | Libellé | Pourquoi |
|---|---|---|
| Hero, principal | « Faire le test (2 min) » | Un verbe d'action, une durée qui fixe l'effort |
| Hero, secondaire | « Demander mon diagnostic gratuit » | Spécifique et possessif |
| Fin du quiz | « Recevoir mon rapport détaillé » | Annonce ce qu'on obtient en échange de l'e-mail |
| Tarifs | « Calculer mon prix » / « Choisir l'offre Pro » | Une action concrète par palier |
| NIS2 | « Télécharger la checklist NIS2 (PDF, 2 pages) » | Le format et la taille sont annoncés |
| Urgence | « Urgence : appeler le 0X XX XX XX XX » | Le numéro est visible dans le bouton, cliquable |
| Formulaire | « Envoyer ma demande de diagnostic » | Pas de « Envoyer » ni de « Valider » seuls |

**Message de succès (formulaire de diagnostic)**
> « Demande reçue. Un analyste vous rappelle sous 4 h ouvrées au numéro indiqué, pour fixer un créneau de diagnostic de 30 min. En cas d'attaque en cours, n'attendez pas : appelez le 0X XX XX XX XX. »

**Messages d'erreur** (structure : ce qui s'est passé, pourquoi, comment corriger)

| Cas | Message |
|---|---|
| Téléphone invalide | « Ce numéro ne semble pas complet. Il faut 10 chiffres pour qu'un analyste puisse vous rappeler. Exemple : 06 12 34 56 78. » |
| Nombre de postes manquant | « Le nombre de postes est vide. Nous en avons besoin pour préparer un diagnostic adapté. Une estimation suffit. » |
| Échec d'envoi (serveur) | « Votre demande n'est pas partie : la connexion a été interrompue. Vos réponses sont conservées. Réessayez, ou appelez-nous au 0X XX XX XX XX. » |

## 9. Contraintes

- **Marque** : bleu marine, blanc cassé, accent cyan. Le rouge est réservé à l'urgence. Typographie Manrope ou Plus Jakarta Sans. **Jamais** de hacker à capuche, de cadenas rouge ou de code défilant. Ton rassurant et pédagogique.
- **Réglementaire** :
  - RGPD : formulaires minimaux, consentement explicite pour le rapport du quiz, aucun traceur publicitaire avant consentement (CNIL).
  - Pas d'allégations non vérifiables (« 100 % sécurisé », « conformité NIS2 garantie »).
  - Les certifications et qualifications affichées doivent être justifiées.
  - Mentions légales LCEN.
- **Sécurité du site lui-même**, par cohérence : HTTPS, en-têtes de sécurité (CSP, HSTS), pas de CMS non maintenu, formulaire protégé contre le spam sans reCAPTCHA intrusif, hébergement dans l'UE.
- **Accessibilité** : RGAA / WCAG 2.1 AA. Contraste de 4,5:1 minimum : le cyan clair ne s'utilise pas pour du texte sur fond clair. Le quiz doit fonctionner au clavier et au lecteur d'écran. Le bouton d'urgence doit mesurer au moins 44 × 44 px.
- **SEO** : requêtes nationales (« SOC managé PME », « NIS2 PME », « surveillance informatique 24/7 »), données structurées Organization et FAQPage, page rapide (LCP inférieur à 2,5 s).
- **Langues** : français au lancement. Anglais en phase 2 (clients ETI à capitaux étrangers).

## 10. Livrables, planning, budget

**Livrables** : un atelier de cadrage, l'arborescence, des wireframes mobile et desktop, 2 pistes de maquette puis 1 maquette finale, un mini design system (couleurs, typographies, composants), l'intégration, le quiz et le simulateur de prix, le suivi analytics et appels, la recette accessibilité, la mise en ligne et une formation d'une heure.

| Semaine | Étape |
|---|---|
| S1 | Cadrage, atelier messages, collecte des contenus |
| S2 | Arborescence, wireframes, logique du quiz |
| S3–S4 | Design (2 pistes, puis itération) |
| S5–S7 | Intégration, quiz, simulateur, formulaires |
| S8 | Recette (contenus, accessibilité, performance), corrections |
| S9 | Mise en ligne, suivi des KPIs |

**Budget indicatif** (estimation du marché français, non sourcée) :
- Freelance confirmé (design et intégration, quiz compris) : **5 000 à 9 000 € HT**.
- Petite agence (stratégie, rédaction SEO, design sur mesure, quiz et simulateur) : **10 000 à 18 000 € HT**.
- Maintenance et évolutions : 80 à 250 € HT par mois.
- Rempart prévoit **12 000 € HT** hors photos.

## 11. Critères de réussite

- Le site est en ligne en 9 semaines, avec le score Lighthouse mobile suivant : Performance ≥ 90, Accessibilité ≥ 95.
- Au moins 30 demandes de diagnostic par mois au 6e mois, et un taux de complétion du quiz de 55 % ou plus.
- Le numéro d'urgence est joignable en 1 tap depuis n'importe quel écran mobile.
- Un dirigeant non technique comprend l'offre, le prix et le « suis-je concerné NIS2 » en moins de 3 minutes (test utilisateur sur 5 personnes).
- Aucune image ni formulation anxiogène ne passe la validation (relecture finale contre la charte).
