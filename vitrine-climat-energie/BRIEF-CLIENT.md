# Brief client : site vitrine Sobra

> Document fictif rédigé comme s'il était remis par le client à l'agence. **Sobra** est une entreprise imaginaire (nom provisoire, à vérifier à l'INPI). Les chiffres internes de Sobra ci-dessous sont des hypothèses de travail, à remplacer par des données réelles.

---

## 1. Présentation de l'entreprise

- **Sobra** : pilotage énergétique des bâtiments tertiaires.
- **Offre** :
  1. des **capteurs** sans fil (sous-comptage par usage, températures, CO₂) posés en une journée ;
  2. une **plateforme** qui croise ces données avec les factures et la météo, détecte les dérives et prépare la déclaration OPERAT ;
  3. un **accompagnement** par un ingénieur énergie référent (plan d'action, réglages CVC, suivi mensuel).
- **Promesse** : réduire la consommation dès la première année et tenir la trajectoire du décret tertiaire (-40 % en 2030).
- **Profil (hypothèse)** : une PME de 25 personnes basée à Lyon, avec environ 180 bâtiments suivis.

## 2. Contexte et déclencheur

- Le site actuel est une page unique produite au lancement. Il ne génère quasiment pas de demandes entrantes : 90 % des contrats viennent du réseau des fondateurs.
- **Déclencheurs** :
  - le bilan OPERAT 2024-2025 (-26 %, à mi-chemin de 2030) a relancé la demande. Les clients veulent maintenant savoir **comment gagner les 14 points restants** ;
  - le report de l'échéance BACS (2027 → 2030 pour les 70-290 kW) a créé de la confusion, et Sobra veut se positionner comme la source claire ;
  - Sobra prépare une levée de fonds : le site doit aussi rassurer investisseurs et partenaires.

## 3. Objectifs business et KPIs

| Objectif | KPI | Cible à 6 mois après la mise en ligne |
|---|---|---|
| Générer des demandes d'audit qualifiées | Formulaires « Audit gratuit » remplis par des bâtiments de plus de 1 000 m² | ≥ 10 par mois |
| Faire du simulateur le point d'entrée | Taux d'usage du simulateur (visites ayant lancé une simulation) | ≥ 25 % des visites |
| Convertir après simulation | Taux de passage simulateur → formulaire | ≥ 12 % |
| Crédibiliser auprès des grands comptes | Temps moyen sur les sections Cas clients et Méthode | ≥ 45 s |
| Être trouvé sur les requêtes réglementaires | Top 10 Google sur « logiciel décret tertiaire », « pilotage énergétique bâtiment tertiaire » | 2 requêtes sur 3 |
| Performance | LCP mobile, CLS, INP | < 2,5 s ; < 0,1 ; < 200 ms |

## 4. Cibles et personas

### Persona 1 : Claire, 44 ans, responsable technique et énergie d'une foncière de bureaux (30 actifs)
- **Job to be done** : « Quand je prépare la déclaration OPERAT et le comité d'investissement, je veux savoir quels actifs dérivent et quoi corriger, pour tenir -40 % en 2030 sans lancer de gros travaux. »
- **Attentes** :
  - tenir la trajectoire OPERAT sur tout le parc ;
  - avoir des données fiables par actif ;
  - disposer d'un reporting exportable (CSRD, comité d'investissement).
- **Freins** :
  - un projet IT de plus, la crainte de l'intégration avec la GTB existante ;
  - des « économies » non prouvées ;
  - la sécurité des données.
- **Ce qu'elle doit trouver** : la méthode de mesure (IPMVP), la compatibilité GTB/BACS, les références de foncières, la sécurité (hébergement en UE).

### Persona 2 : Marc, 52 ans, directeur des services techniques d'une ville de 40 000 habitants
- **Job to be done** : « Quand le budget énergie dérape et que les élus me demandent des résultats, je veux identifier les bâtiments qui coûtent le plus et un moyen finançable de les corriger, pour présenter un plan crédible au prochain conseil. »
- **Attentes** :
  - baisser la facture d'énergie (sous contrainte budgétaire) ;
  - prioriser les bâtiments (écoles, gymnases) ;
  - financer via les CEE.
- **Freins** :
  - la commande publique (il lui faut un marché ou une centrale d'achat) ;
  - peu de temps, des équipes réduites ;
  - la méfiance envers les « start-up » qui pourraient disparaître.
- **Ce qu'il doit trouver** : des cas de collectivités, l'éligibilité aux CEE, les modalités d'achat public, la pérennité (partenaires, ADEME).

### Persona 3 : Sophie, 38 ans, responsable des services généraux d'une enseigne de 25 magasins
- **Job to be done** : « Quand je reçois les factures trimestrielles, je veux repérer en un coup d'œil les magasins qui gaspillent (chauffage la nuit, clim l'hiver), pour corriger vite sans immobiliser les équipes. »
- **Attentes** :
  - des résultats rapides et visibles ;
  - des alertes simples (chauffage allumé la nuit) ;
  - zéro travaux lourds.
- **Freins** :
  - le budget OPEX ;
  - l'installation dans des sites ouverts au public.
- **Ce qu'elle doit trouver** : la durée d'installation, le retour sur investissement en mois, le simulateur, le prix indicatif ou le mode de tarification.

## 5. Messages clés et preuves

| Message | Preuve attendue sur le site |
|---|---|
| « -27 % de consommation la première année » | Note de méthode sous le chiffre : nombre de bâtiments, période, correction climatique, protocole IPMVP. **Sans cette preuve, le chiffre n'est pas publié.** |
| « Vous êtes à mi-chemin de 2030. Nous vous aidons à faire l'autre moitié. » | Rappel daté et sourcé des objectifs (-40/-50/-60 %) et du bilan OPERAT |
| « Installé en un jour, sans travaux » | Photo réelle d'un capteur posé, vidéo de 30 s, déroulé en 3 étapes |
| « Un ingénieur référent, pas un ticket de support » | Portraits de l'équipe, rythme du suivi (mensuel) |
| « Des économies finançables » | Mention des CEE avec les conditions, sans promesse de montant |
| « Impact mesuré » | Compteur MWh et tCO₂ évités, avec un lien vers le facteur d'émission utilisé (base Empreinte ADEME) |

## 6. Arborescence et contenus attendus (one-page + pages légales)

1. **Hero** : le chiffre d'impact en grand, une phrase de méthode, le CTA « Audit gratuit » et le CTA secondaire « Estimer mes économies » (ancre vers le simulateur).
2. **Le problème** en 3 chiffres : l'objectif de -40 % en 2030, la part déjà faite (-26 %), le coût de l'énergie pour le client type. Chaque chiffre a sa source.
3. **La solution** : capteurs, plateforme, accompagnement, en 3 colonnes. Captures réelles de la plateforme (pas de maquette fictive).
4. **Simulateur** : type de bâtiment (bureaux, enseignement, commerce, santé, logistique) + surface + (option) facture annuelle → fourchette d'économies en kWh/an et en €/an, et position sur la trajectoire 2030. Les hypothèses sont affichées et le résultat peut être envoyé dans le formulaire.
5. **Cas clients** : carte des bâtiments équipés (points agrégés, pas d'adresse exacte sans accord) et 3 fiches cas (type, surface, ville, gain sur 12 mois, courbe avant/après).
6. **Impact cumulé** : compteur MWh et tCO₂ évités, date de mise à jour, méthode.
7. **Certifications et partenaires** : uniquement des labels réellement obtenus. Pas de logo ADEME sans autorisation : l'ADEME encadre l'usage de son logo, et un programme financé ou une étude ne donne pas droit au logo. Mention CEE si Sobra est partenaire d'un obligé.
8. **Contact / demande d'audit** : formulaire court (nom, organisation, e-mail, surface totale, nombre de sites, résultat du simulateur prérempli) et prise de rendez-vous.
- **Pied de page** : mentions légales, politique de confidentialité, gestion des cookies, accessibilité (déclaration), page Méthode (calculs du simulateur et du compteur).

## 7. Contraintes

### Marque
- **Palette** : vert profond, sable, jaune soleil.
- **À proscrire** : feuilles, planète et éoliennes en clip-art, bleu « tech ».
- **Typo** : une grotesque large pour les chiffres (Archivo en largeur étendue ou Space Grotesk).
- **Ton** : concret, chiffré, sans superlatif.
- **Nom provisoire** : prévoir un remplacement facile (texte, logo, favicon).

### Réglementaire
- **Allégations environnementales** : chaque chiffre a une source, une date et un périmètre.
  - Interdits : « neutre en carbone », « vert », « éco-responsable » sans preuve.
  - Respecter la loi Climat et Résilience et la directive UE 2024/825 (à faire valider par un juriste).
- **Dates réglementaires** : citer les textes en vigueur (décret tertiaire, décret BACS modifié en décembre 2025) et dater chaque mention.
- **CEE** : pas de montant promis, mention « sous réserve d'éligibilité ».
- **RGPD** :
  - formulaire minimal et consentement explicite ;
  - données de simulation non conservées sans envoi du formulaire ;
  - mesure d'audience exemptée de consentement (Matomo configuré selon la CNIL) ou bandeau conforme.

### Accessibilité
- WCAG 2.2 AA visé : contrastes (attention au jaune sur sable), navigation au clavier dans le simulateur, alternative textuelle aux graphiques (tableau de données).

### SEO
- National sur les requêtes réglementaires, plus des pages ville en phase 2 (Lyon, Paris, Marseille).
- Données structurées Organization, FAQ et SoftwareApplication.

### Langues
- Français au lancement, anglais en phase 2 (investisseurs, foncières internationales). Prévoir l'i18n dès le départ.

### Technique
- Site statique ou CMS headless.
- Chiffres (compteur, cas) éditables sans développeur.
- Poids de page inférieur à 1,5 Mo sur mobile.

## 8. Mini plan de recherche utilisateur

- **Objectif** : vérifier que les trois personas comprennent la promesse en 5 s, croient le chiffre d'impact, et terminent le simulateur jusqu'au formulaire.
- **Méthode** :
  - 5 entretiens semi-directifs de 45 min (2 responsables techniques de foncière, 2 services techniques de collectivité, 1 services généraux retail), en visio ;
  - en fin d'entretien, un test d'usabilité de 10 min sur la maquette cliquable (hero, simulateur, formulaire) ;
  - recrutement via le réseau des fondateurs et LinkedIn, avec une incitation (carte cadeau ou rapport de benchmark).
- **Livrable** : synthèse des freins, verbatims, liste de corrections priorisées (impact × effort), avant la phase de maquettes finales (S4).

### Guide d'entretien en 5 temps

1. **Mise en route (5 min)**
   - Pouvez-vous décrire votre poste et le parc dont vous avez la charge ?
   - Combien de temps par mois consacrez-vous aux sujets d'énergie ?
2. **Contexte (10 min)**
   - Racontez-moi votre dernière déclaration OPERAT : qu'est-ce qui a été difficile ?
   - Comment suivez-vous aujourd'hui les consommations, et avec quels outils ?
   - Qui décide d'un achat de ce type chez vous, et sur quels critères ?
3. **Approfondissement (10 min)**
   - Quand un prestataire vous annonce « -30 % », qu'est-ce qui vous fait le croire ou non ?
   - Avez-vous déjà été déçu par un outil ou une promesse d'économies ? Que s'est-il passé ?
   - Qu'est-ce qui vous ferait demander un audit plutôt qu'attendre ?
4. **Réaction à la maquette (15 min)**
   - En 5 secondes : que propose cette entreprise, et pour qui ?
   - Lancez une simulation pour l'un de vos bâtiments. Pensez à voix haute.
   - Le résultat vous paraît-il crédible ? Que manque-t-il pour que vous remplissiez le formulaire ?
5. **Conclusion (5 min)**
   - Si vous deviez décrire ce site à un collègue, que diriez-vous ?
   - Y a-t-il une question que vous auriez aimé voir traitée sur la page ?

## 9. UX copy

### Titre du hero recommandé
**« -27 % de consommation dès la première année. »**
Sous-titre : « Capteurs, plateforme et un ingénieur dédié pour tenir l'objectif 2030 du décret tertiaire. »
Note de méthode sous le chiffre : « Moyenne de N bâtiments suivis sur 12 mois, corrigée du climat (protocole IPMVP). Voir la méthode. »

| Option | Texte | Ton | Idéal pour |
|---|---|---|---|
| A. Échéance | « Vous avez fait la moitié du chemin vers 2030. On vous aide à faire l'autre. » | Complice, réglementaire | Foncières et collectivités déjà engagées sur OPERAT |
| B. Facture | « Vos bâtiments consomment la nuit. Pas votre budget. » | Direct, un peu provocant | PME multisite et retail, campagnes payantes |
| C. Preuve | « Des économies mesurées, pas promises. » | Sobre, ingénieur | Grands comptes méfiants, page Méthode, LinkedIn |

### Libellés des CTA
| Contexte | Libellé |
|---|---|
| CTA principal du hero | « Demander mon audit gratuit » |
| CTA secondaire du hero | « Estimer mes économies » |
| Bouton du simulateur | « Calculer l'économie de mon bâtiment » |
| Après le résultat | « Recevoir l'analyse détaillée » |
| Cas clients | « Voir la courbe complète » |
| Compteur d'impact | « Comprendre le calcul » |
| Formulaire | « Envoyer ma demande d'audit » |

### Messages du formulaire
- **Succès** : « Demande envoyée. Un ingénieur Sobra vous rappelle sous 2 jours ouvrés pour fixer l'audit. Le résumé de votre simulation vous a été envoyé par e-mail. »
- **Erreur de champ** (ce qui s'est passé, pourquoi, comment corriger) : « Surface non reconnue : le champ attend un nombre en m². Saisissez par exemple 2400. »
- **Erreur d'envoi** : « Votre demande n'est pas partie : la connexion a été interrompue. Vos informations sont conservées. Réessayez, ou écrivez-nous à contact@… »
- **Simulateur hors périmètre** : « Moins de 1 000 m² : votre bâtiment n'est pas soumis au décret tertiaire. Sobra peut quand même réduire sa consommation. Laissez-nous vos coordonnées pour une estimation. »

## 10. Livrables

- Benchmark et moodboard (3 pistes) ; choix d'une piste.
- Wireframes desktop et mobile de la one-page.
- Maquettes UI desktop et mobile, avec les états du simulateur (vide, saisie, résultat, erreur).
- Mini design system : couleurs, typos, composants chiffres, cartes, courbes.
- Développement, intégration CMS, formulaire connecté au CRM (HubSpot ou Pipedrive).
- Simulateur : spécification des formules validée par Sobra, puis développement.
- Rédaction ou réécriture des contenus et de la page Méthode.
- Recette (navigateurs, mobile, accessibilité), mise en ligne, formation d'une heure.

## 11. Planning indicatif

| Semaine | Étape |
|---|---|
| S1 | Atelier de lancement, collecte des données (cas, chiffres, photos) |
| S2 | Benchmark, moodboard, choix de la piste |
| S3 | Wireframes, spécification du simulateur |
| S4-S5 | Maquettes UI desktop et mobile, 2 allers-retours |
| S6-S8 | Développement, simulateur, CMS, intégration CRM |
| S9 | Contenus finaux, recette, accessibilité |
| S10 | Mise en ligne, suivi des KPIs |
| Phase 2 (M+2/M+3) | Version anglaise, pages ville, cas supplémentaires |

## 12. Budget indicatif (France, HT)

Estimations de marché, non sourcées : à confronter aux devis.

| Prestataire | Fourchette | Commentaire |
|---|---|---|
| Freelance designer + développeur | 6 000 à 12 000 € | Simulateur simple, CMS léger |
| Studio ou agence (2 à 10 personnes) | 15 000 à 30 000 € | Design system, data-viz sur mesure, rédaction, SEO |
| Options | 1 000 à 2 500 € par jour de tournage photo ou vidéo ; 1 500 à 4 000 € pour l'anglais ; maintenance 80 à 250 € par mois | |

## 13. Critères de réussite

- Un responsable technique comprend en 5 secondes ce que fait Sobra et pourquoi c'est urgent (test sur 5 personnes).
- Tous les chiffres publiés ont une source et une date ; aucune allégation non prouvée.
- Le simulateur fonctionne au clavier et sur mobile, et son résultat préremplit le formulaire.
- Les KPIs à 6 mois sont atteints (section 3).
- Les scores Lighthouse mobile sont d'au moins 90 en performance et en accessibilité.
- Sobra met à jour seule le compteur et les cas clients.
