# Brief client : site vitrine Sobra

> Document fictif, rédigé comme s'il était remis par l'entreprise à l'agence. **Sobra** est une entreprise imaginaire : personne ne valide ce brief, l'agence décide de tout. Aucun chiffre n'est inventé. Les valeurs de conception (px, semaines, nombre de champs ou d'étapes) sont des spécifications. Toute donnée chiffrée sur le secteur ou la loi a sa source, vue le 2026-11-13. Sobra n'a ni prix, ni effectif, ni résultat chiffré.

---

## 1. Présentation de l'entreprise

- **Sobra** : pilotage énergétique des bâtiments tertiaires.
- **Offre** :
  1. des **capteurs** sans fil (sous-comptage par usage, températures, CO₂) posés sans travaux ;
  2. une **plateforme** qui croise ces données avec les factures et la météo, détecte les dérives et prépare la déclaration OPERAT ;
  3. un **accompagnement** par un ingénieur énergie référent (plan d'action, réglages CVC, suivi mensuel).
- **Promesse** : réduire la consommation et tenir la trajectoire du décret tertiaire (-40 % en 2030, décret n° 2019-771).
- **Profil** : une PME basée à Lyon. Pas d'effectif ni de nombre de bâtiments suivis : ce serait inventé.

## 2. Contexte et déclencheur

- Le site actuel est une page unique produite au lancement. Il ne génère quasiment pas de demandes entrantes : presque tous les contrats viennent du réseau des fondateurs.
- **Déclencheurs** :
  - le bilan OPERAT 2024-2025 (-26 % de consommation corrigée du climat pour le parc déclaré) a relancé la demande. Les clients veulent maintenant savoir **comment gagner les 14 points restants** d'ici 2030 (source : [economiematin.fr](https://www.economiematin.fr/batiments-tertiaires-a-26-le-parc-francais-a-fait-la-moitie-du-chemin-vers-2030), qui cite le communiqué ADEME et ministère de la Transition écologique du 20/07/2026, vu le 2026-11-13) ;
  - le report de l'échéance BACS (2027 → 1er janvier 2030 pour les systèmes de 70 à 290 kW, décret n° 2025-1343 du 26/12/2025) a créé de la confusion, et Sobra veut se positionner comme la source claire (source : [projetcelsius.com](https://projetcelsius.com/en/blog/france-tertiary-decree-bacs-obligations/), vu le 2026-11-13) ;
  - Sobra prépare une levée de fonds : le site doit aussi rassurer investisseurs et partenaires.

## 3. Objectifs business et indicateurs

Les indicateurs sont suivis dès la mise en ligne. Pas de cible chiffrée : Sobra n'a pas d'historique, toute cible serait inventée.

| Objectif | Indicateur suivi |
|---|---|
| Générer des demandes d'audit qualifiées | Formulaires « Audit gratuit » remplis pour des bâtiments de 1 000 m² ou plus (seuil du décret tertiaire, article R174-22 du code de la construction et de l'habitation) |
| Faire du simulateur le point d'entrée | Part des visites qui lancent une simulation |
| Convertir après simulation | Taux de passage simulateur → formulaire |
| Crédibiliser auprès des grands comptes | Temps passé sur les sections Cas clients et Méthode |
| Être trouvé sur les requêtes réglementaires | Position Google (Search Console) sur « logiciel décret tertiaire » et « pilotage énergétique bâtiment tertiaire » |
| Performance | Core Web Vitals sur mobile, sous les seuils « bon » de Google (web.dev) : LCP ≤ 2,5 s, CLS ≤ 0,1, INP ≤ 200 ms |

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
- **Ce qu'elle doit trouver** : la méthode de mesure (IPMVP), la compatibilité GTB/BACS, des cas de foncières, la sécurité (hébergement en UE).

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
- **Ce qu'il doit trouver** : des cas de collectivités, l'éligibilité aux CEE, les modalités d'achat public, qui est derrière Sobra.

### Persona 3 : Sophie, 38 ans, responsable des services généraux d'une enseigne de 25 magasins
- **Job to be done** : « Quand je reçois les factures trimestrielles, je veux repérer en un coup d'œil les magasins qui gaspillent (chauffage la nuit, clim l'hiver), pour corriger vite sans immobiliser les équipes. »
- **Attentes** :
  - des résultats rapides et visibles ;
  - des alertes simples (chauffage allumé la nuit) ;
  - zéro travaux lourds.
- **Freins** :
  - le budget OPEX ;
  - l'installation dans des sites ouverts au public.
- **Ce qu'elle doit trouver** : le déroulé de l'installation, le simulateur, le mode de tarification (sans prix : Sobra n'a pas de grille réelle).

## 5. Messages clés et preuves

| Message | Preuve sur le site |
|---|---|
| « Vous avez fait la moitié du chemin vers 2030. On vous aide à faire l'autre. » | Le « -26 % » du bilan OPERAT 2024-2025 et les objectifs -40/-50/-60 % (décret n° 2019-771), chacun avec sa source et sa date |
| « Des économies mesurées, pas promises. » | Page Méthode : protocole IPMVP, correction climatique, période de référence. Aucun pourcentage de résultat : Sobra n'en a pas |
| « Installé sans travaux » | Déroulé en 3 étapes. À produire : une photo de capteur posé (banque d'images ou prise de vue), désaturée. Pas de vidéo, pour tenir le poids mobile |
| « Un ingénieur référent, pas un ticket de support » | Bloc « Qui sommes-nous » court, sans photo (bloc 7), et rythme du suivi (mensuel) |
| « Des économies finançables » | Mention des CEE avec les conditions, sans promesse de montant |
| « Impact mesuré » | Les deux indicateurs suivis (MWh et tCO₂ évités) et leur méthode, avec le facteur d'émission de la Base Empreinte ADEME. Aucune valeur inventée |

## 6. Arborescence et contenus attendus (one-page + pages légales)

1. **Hero** : le chiffre public « -26 % » en grand, sa source juste dessous, le titre de l'option A (section 9), le CTA « Audit gratuit » et le CTA secondaire « Estimer mes économies » (ancre vers le simulateur).
2. **Le problème** en 3 chiffres : l'objectif de -40 % en 2030 (décret n° 2019-771), les 14 points qui restent après le bilan OPERAT 2024-2025, l'échéance BACS du 1er janvier 2030 pour les systèmes de 70 à 290 kW (décret n° 2025-1343). Chaque chiffre a sa source et sa date (sources en section 2).
3. **La solution** : capteurs, plateforme, accompagnement, en 3 colonnes. À produire : les écrans de la plateforme, dessinés par l'agence, sans valeur chiffrée (axes et libellés seuls), légendés « illustration ».
4. **Simulateur** : type de bâtiment (bureaux, enseignement, commerce, santé, logistique) + surface + (option) facture annuelle → fourchette d'économies en kWh/an et en €/an, et position sur la trajectoire 2030. Les formules reposent sur des références publiques, chacune citée sur la page Méthode. Les hypothèses sont affichées et le résultat peut être envoyé dans le formulaire.
5. **Cas clients** : carte à points d'exemple (aucune adresse, aucun total affiché) et 3 fiches de démonstration : type de bâtiment, ville, leviers activés, indicateur suivi (consommation corrigée du climat sur 12 mois). Aucun gain chiffré. La courbe avant/après est une forme sans valeurs, légendée « illustration ».
6. **Impact cumulé** : les indicateurs MWh et tCO₂ évités, leur méthode et le facteur d'émission utilisé. Pas de compteur chiffré dans la démo : le cumul serait inventé.
7. **Qui sommes-nous et cadres suivis** :
   - « Qui sommes-nous » en 3 phrases, sans photo, avec le logo : « Sobra est une équipe d'ingénieurs énergie basée à Lyon. Chaque bâtiment suivi a un ingénieur référent, qui lit les données, propose les réglages et fait le bilan avec vous chaque mois. Les capteurs, la plateforme et l'ingénieur forment un seul service. » ;
   - les textes servis, cités en clair avec leur source : décret tertiaire, décret BACS, CEE « sous réserve d'éligibilité » ;
   - aucun logo de label ni de partenaire : Sobra n'en a obtenu aucun. Pas de logo ADEME : l'ADEME encadre l'usage de son logo, et un programme financé ou une étude ne donne pas droit au logo.
8. **Contact / demande d'audit** : formulaire court (nom, organisation, e-mail, surface totale, nombre de sites, résultat du simulateur prérempli) et prise de rendez-vous.
- **Pied de page** : mentions légales, politique de confidentialité, gestion des cookies, accessibilité (déclaration), page Méthode (calculs du simulateur et des indicateurs d'impact).

## 7. Contraintes

### Marque
- **Palette** : vert profond, sable, jaune soleil.
- **À proscrire** : feuilles, planète et éoliennes en clip-art, bleu « tech ».
- **Typo** : une grotesque large pour les chiffres (Archivo en largeur étendue ou Space Grotesk).
- **Ton** : concret, sourcé, sans superlatif.
- **Nom provisoire** : prévoir un remplacement facile (texte, logo, favicon).

### Réglementaire
- **Allégations environnementales** : chaque chiffre a une source, une date et un périmètre.
  - Interdits : « neutre en carbone », « vert », « éco-responsable » sans preuve.
  - On applique la loi Climat et Résilience et la directive (UE) 2024/825, que les États membres appliquent à partir du 27 septembre 2026 (article 4, [EUR-Lex](https://eur-lex.europa.eu/eli/dir/2024/825/oj/fra), vu le 2026-11-13).
- **Dates réglementaires** : citer les textes en vigueur (décret n° 2019-771, décret n° 2025-1343 du 26/12/2025 qui modifie le calendrier BACS) et dater chaque mention.
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
- Chiffres sourcés et fiches cas éditables sans développeur.
- Poids de page inférieur à 1,5 Mo sur mobile.

## 8. Mini plan de recherche utilisateur

- **Objectif** : vérifier que les trois personas comprennent la promesse en 5 s, lisent le « -26 % » comme un repère du secteur et non comme un résultat de Sobra, et terminent le simulateur jusqu'au formulaire.
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
   - Quand un prestataire vous annonce un pourcentage d'économies, qu'est-ce qui vous fait le croire ou non ?
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

### Titre du hero retenu
**« Vous avez fait la moitié du chemin vers 2030. On vous aide à faire l'autre. »** (option A)
Chiffre en grand au-dessus du titre : « -26 % ».
Source sous le chiffre : « Consommation du parc tertiaire déclaré sur OPERAT, corrigée du climat, par rapport à l'année de référence. Bilan OPERAT 2024-2025, ADEME et ministère de la Transition écologique, 20/07/2026. Objectif 2030 : -40 %. »
Sous-titre : « Capteurs, plateforme et un ingénieur référent pour tenir l'objectif 2030 du décret tertiaire. »

| Option | Texte | Ton | Idéal pour |
|---|---|---|---|
| A. Échéance (retenue) | « Vous avez fait la moitié du chemin vers 2030. On vous aide à faire l'autre. » | Complice, réglementaire | Foncières et collectivités déjà engagées sur OPERAT |
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
| Impact | « Comprendre le calcul » |
| Formulaire | « Envoyer ma demande d'audit » |

### Messages du formulaire
- **Succès** : « Demande envoyée. Un ingénieur Sobra vous rappelle pour fixer l'audit. Le résumé de votre simulation vous a été envoyé par e-mail. »
- **Erreur de champ** (ce qui s'est passé, pourquoi, comment corriger) : « Surface non reconnue : le champ attend un nombre en m². Saisissez par exemple 2400. »
- **Erreur d'envoi** : « Votre demande n'est pas partie : la connexion a été interrompue. Vos informations sont conservées. Réessayez, ou écrivez-nous à contact@… »
- **Simulateur hors périmètre** : « Moins de 1 000 m² : votre bâtiment n'est pas soumis au décret tertiaire. Sobra peut quand même réduire sa consommation. Laissez-nous vos coordonnées pour une estimation. »

## 10. Livrables

- Benchmark et moodboard (3 pistes) ; choix d'une piste.
- Wireframes desktop et mobile de la one-page.
- Maquettes UI desktop et mobile, avec les états du simulateur (vide, saisie, résultat, erreur).
- Mini design system : couleurs, typos, composants chiffres, cartes, courbes.
- Développement, intégration CMS, formulaire connecté au CRM (HubSpot ou Pipedrive).
- Simulateur : spécification des formules, écrite par l'agence à partir de références publiques citées sur la page Méthode, puis développement.
- Rédaction des contenus et de la page Méthode.
- Recette (navigateurs, mobile, accessibilité), mise en ligne, formation d'une heure.

## 11. Planning indicatif

| Semaine | Étape |
|---|---|
| S1 | Cadrage, relevé des sources publiques (décret tertiaire, OPERAT, BACS, CEE) |
| S2 | Benchmark, moodboard, choix de la piste |
| S3 | Wireframes, spécification du simulateur |
| S4-S5 | Maquettes UI desktop et mobile, 2 allers-retours |
| S6-S8 | Développement, simulateur, CMS, intégration CRM |
| S9 | Contenus finaux, recette, accessibilité |
| S10 | Mise en ligne, suivi des indicateurs |
| Phase 2 (M+2/M+3) | Version anglaise, pages ville, fiches supplémentaires |

## 12. Budget

Non chiffré. Les fourchettes de la première version n'avaient pas de source : elles sont retirées. Aucune grille tarifaire publique n'a été ouverte pour les remplacer.

## 13. Critères de réussite

- Un responsable technique comprend en 5 secondes ce que fait Sobra et pourquoi c'est urgent (test sur 5 personnes).
- Tous les chiffres publiés ont une source et une date ; aucune allégation non prouvée.
- Le simulateur fonctionne au clavier et sur mobile, et son résultat préremplit le formulaire.
- Les indicateurs de la section 3 sont mesurés dès la mise en ligne.
- Les scores Lighthouse mobile sont d'au moins 90 en performance et en accessibilité.
- Sobra met à jour seule les chiffres sourcés et les fiches cas.
