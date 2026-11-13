# Étude de cas : site vitrine d'un artisan RGE de la rénovation énergétique

> Entreprise fictive : **Arotz Rénovation** (Pays basque, nom réservé à la démo). Toutes les autres entreprises citées sont réelles. Aucun chiffre n'est inventé : chaque donnée de marché ou de concurrent a sa source, ouverte le 2026-11-13.
> Les visuels d'Aira, d'Effy, d'Hellio (cas d'Orléans) et de Final Touch Carpentry ont été vus et capturés dans le bench le 2026-11-12 (voir « Notes de méthode » en fin de document).

## Executive summary

En 2026, la rénovation énergétique des maisons ne croît pas grâce aux subventions : les dépôts MaPrimeRénov' de rénovation d'ampleur ont été divisés par 4 entre le premier semestre 2025 et le premier semestre 2026. Ce qui progresse, c'est le besoin de **confiance**, depuis que le démarchage pour ces travaux est interdit au téléphone, par SMS, par e-mail et sur les réseaux sociaux.

Les sites de référence (plateformes nationales, réseau, installateur britannique, artisan primé) partagent les mêmes codes : simulateur d'aides, mur de logos, avis, services en icônes. Les meilleurs incarnent l'équipe et chiffrent des cas réels.

Pour Arotz, l'opportunité est d'être l'artisan local vérifiable : un « Qui sommes-nous » direct, labels avec numéros, avant/après en classes DPE, estimateur honnête et posture « on ne vous démarchera jamais ». Le tout dans une identité basque artisanale qui tranche avec les plateformes.

---

## 1. Le marché en 5 lignes

1. **Budget public rationné** : le budget MaPrimeRénov' 2026 est de 3,6 milliards d'euros. Le guichet a été suspendu au 1er janvier 2026, faute de loi de finances votée, puis rouvert le 23 février 2026 ([Selectra](https://selectra.info/energie/renovation-energetique/aides/ma-prime-renov), vu le 2026-11-13).
2. **Demande globale en chute** : un peu plus de 20 000 dossiers de rénovation d'ampleur déposés au premier semestre 2026, contre 95 000 au premier semestre 2025, selon l'Anah ([Banque des Territoires, dépêche AFP du 27/07/2026](https://www.banquedesterritoires.fr/maprimerenov-les-nouvelles-demandes-divisees-par-quatre-apres-la-baisse-des-aides), vu le 2026-11-13). Rendez-vous France Rénov' obligatoire avant dépôt. Mon Accompagnateur Rénov' obligatoire pour le Parcours accompagné : « entre 2 000 et 2 800 € pour un accompagnement complet » ([Hellowatt](https://www.hellowatt.fr/renovation/globale/accompagnateur-renov), vu le 2026-11-13).
3. **La confiance devient le moteur** : la loi du 30 juin 2025 interdit de solliciter un particulier par téléphone, SMS, e-mail ou message privé sur les réseaux sociaux pour lui proposer des travaux de rénovation énergétique ([Aladom](https://www.aladom.fr/actualites/secteur-service/10807/loi-du-30-juin-2025-interdiction-du-demarchage-pour-les-aides-a-la-renovation/), [ANIL](https://www.anil.org/aj-loi-lutte-fraude-aides-publiqus-renovation-energetique/), vus le 2026-11-13). Le particulier doit chercher l'artisan, ce qui fait du site et de la fiche Google le canal principal.
4. **Bailleurs** : les logements classés G sont considérés comme non décents à compter de 2025, les F à compter de 2028, les E à compter de 2034 ([ministère de la Transition écologique](https://www.ecologie.gouv.fr/politiques-publiques/diagnostic-performance-energetique-dpe), vu le 2026-11-13). Ce calendrier soutient la demande des bailleurs.
5. **Concurrence locale en ligne** : au Pays basque, les recherches « artisan RGE pompe à chaleur » remontent surtout des annuaires (Effy, PagesJaunes, Hellowatt) et SOLIHA Pays Basque ([effy.fr, Ustaritz](https://www.effy.fr/artisans/travaux/pompe-a-chaleur/pyrenees-atlantiques/64547-ustaritz), [hellowatt.fr](https://www.hellowatt.fr/artisans/soliha-pays-basque/)), pas des sites d'artisans.

---

## 2. Critique de 5 sites réels

Grille utilisée pour chaque site : première impression (2 s), usabilité, hiérarchie visuelle, accessibilité, ce qui marche, recommandations. « Non observable » signifie que la page n'a pas été vue.

### 2.1 Effy (France, accompagnateur national) : https://www.effy.fr/nos-offres
- **Positionnement** : accompagnateur de la rénovation énergétique. Revendique « + de 100 000 familles accompagnées chaque année » et « plus de 5 000 artisans RGE partenaires » (page [nos offres](https://www.effy.fr/nos-offres), vue le 2026-11-13). Mandataire MaPrimeRénov', prime CEE « Prime Effy ».
- **Première impression** (accueil vu dans le bench, n° 19) : un salon mis en scène, une mascotte, du jaune vif et « Votre pompe à chaleur dès 49€/mois ». Aucun visage d'artisan. L'objectif est clair : obtenir des aides.
- **Usabilité** :
  - le [parcours d'estimation](https://www.effy.fr/parcours/1/accueil) est la porte d'entrée : une question par écran, deux grandes cartes à pictogramme, une barre de progression et « En 2 minutes ! » (bench, n° 5) ;
  - le numéro court 3456 est écrit dans l'en-tête, avec « du lundi au vendredi - 8h à 19h » (page nos offres, vue le 2026-11-13) ;
  - offres par type de travaux ([rénovation globale](https://www.effy.fr/nos-offres/renovation-globale-isolation-chauffage)), page [avis](https://www.effy.fr/avis-effy), [guide](https://www.effy.fr/guide).
- **Hiérarchie visuelle** : sur l'accueil, la mensualité et le bouton jaune passent avant les travaux et avant l'artisan (bench, n° 19).
- **Accessibilité** : en mobile, le bouton téléphone (54×48 px) n'a ni `aria-label` ni texte relevé (bench). Le reste n'a pas été audité.
- **Ce qui marche** :
  - le simulateur comme point d'entrée ;
  - des récits clients titrés par une citation (« [On sent la différence de confort !](https://www.effy.fr/magazine/sent-la-difference-de-confort-une-renovation-globale-dans-le-val-doise) ») ;
  - un SEO très fort sur les aides.
- **Recommandations** :
  1. Corriger les incohérences, relevées le 2026-11-13 : « Depuis plus de 15 ans » sur la page [rénovation globale](https://www.effy.fr/nos-offres/renovation-globale-isolation-chauffage), « Plus de 17 ans » sur [nos offres](https://www.effy.fr/nos-offres) et l'[accueil](https://www.effy.fr/) ; « jusqu'à 11 000 € de prime » sur nos offres, « jusqu'à 25 000€ de Prime Effy » sur la page rénovation globale.
  2. Rendre visible l'artisan qui réalise les travaux.
  3. Dater les montants d'aides affichés.

### 2.2 Hellio, offre particuliers (France) : https://particulier.hellio.com/solutions/renovation-globale
- **Positionnement** : « Rénovez votre maison en toute confiance après un audit ». Rénovation globale clé en main, avec Hellio Ingénierie comme Mon Accompagnateur Rénov'.
- **Première impression** : le mot « confiance » et l'audit comme première étape rassurent dès le titre.
- **Usabilité** :
  - une page solution par projet et une page [aides](https://www.hellio.com/aides-financements) ;
  - deux domaines (corporate et particulier) peuvent égarer le visiteur.
- **Hiérarchie visuelle** : non observable.
- **Accessibilité** : non observable.
- **Ce qui marche** :
  - des cas réels avec ville et % (« [76 % d'économies d'énergie pour une maison à Orléans](https://www.hellio.com/actualites/communiques/renovation-energetique-orleans-globale) ») ;
  - l'audit est présenté comme rassurant, pas comme une contrainte.
- **Recommandations** :
  1. Remonter les cas chiffrés des communiqués vers les pages de vente.
  2. Séparer clairement le parcours particulier du parcours B2B.
  3. Ajouter un repère DPE avant/après à chaque cas.

### 2.3 illiCO travaux (réseau français de courtage) : https://www.illico-travaux.com/
- Un article de l'[Observatoire de la Franchise](https://www.observatoiredelafranchise.fr/indiscretions-actualite/ILLICO-TRAVAUX-illico-travaux-renove-tout-50813.htm) annonce un site « plus intuitif », mais il date du 31 juillet 2015. Nouvelle identité graphique présentée le 02/10/2026 ([Toute la Franchise](https://www.toute-la-franchise.com/news-illico-travaux-nouvelle-identite-titre-meilleure-franchise), vu le 2026-11-13).
- **Positionnement** : « Un interlocuteur unique », « Artisans sélectionnés », « Plus de 200 agences locales à votre service » (accueil lu le 2026-11-13).
- **Première impression, usabilité, hiérarchie, accessibilité** : non observables. Seul le texte de l'accueil a été lu, sans capture.
- **Ce qui marche** (modèle) : « un seul interlocuteur » répond au premier frein (coordonner plusieurs corps de métier).
- **Recommandations** :
  1. Distinguer nettement le parcours client du recrutement de franchisés.
  2. Montrer les artisans réels derrière le courtier.

### 2.4 Aira (Royaume-Uni, installateur de pompes à chaleur) : référence internationale
- **URL** : https://www.airahome.com/en-gb/locations/england (l'ancienne adresse `heat-pump-installation-uk/england` y redirige) ; page ville https://www.airahome.com/en-gb/locations/england/london ; cas https://www.airahome.com/en-gb/case-studies/roger-sue-aira-heat-pump-installation
- **Positionnement** : PAC clé en main, évaluation gratuite, « 15-Year Aira Guarantee », subvention de 7 500 £ déduite du devis, « We're a Which? Trusted Trader » (pages [England](https://www.airahome.com/en-gb/locations/england) et [installation](https://www.airahome.com/en-gb/heat-pump-installation-2), vues le 2026-11-13).
- **Première impression** (capture du bench, n° 1) : **deux installateurs bras croisés devant la camionnette jaune Aira, une pastille « Which? Trusted Trader » posée sur la photo**. Humain et label de confiance sont réunis dans la même image.
- **Usabilité** :
  - déroulé clair : évaluation gratuite, paiement flexible, conception et pose, reprise de l'ancienne chaudière, garantie ;
  - pages par région et par ville ;
  - téléphone écrit en texte dans l'en-tête sur desktop, réduit à une icône en mobile (bench).
- **Hiérarchie visuelle** (bench, n° 1) : fond blanc, grand titre, un CTA « Get a quote » sombre sur orange. Côté contenu : humain, puis promesse, puis aide déduite, puis étapes.
- **Accessibilité** : textes alternatifs descriptifs présents. En mobile, l'icône téléphone fait 31×31 px, sous les 44 px des cibles tactiles WCAG 2.5.5 (bench).
- **Ce qui marche** :
  - l'aide déduite du devis, dite en une phrase ;
  - le SEO local par pages ville ;
  - des cas clients au prénom (« Roger & Sue »).
- **Recommandations** :
  1. Afficher des prix vérifiables : des comparateurs tiers les contestent ([theecoexperts.co.uk](https://www.theecoexperts.co.uk/heat-pumps/aira-review-best-heat-pump-installer)).
  2. Montrer tous les avis : le carrousel annonce « Showing our 4 & 5 star reviews » (bench, n° 1).
  3. Moins de marketing produit, plus de chantier réel.

### 2.5 Final Touch Carpentry (artisan, international) : https://www.awwwards.com/sites/final-touch-carpentry
- Nominé Awwwards (21/07/2021). La fiche résume : « fonction et conversion avant le design, entreprise locale qui vise à générer des leads ».
- **Première impression** (fiche capturée dans le bench, n° 2) : hero bleu nuit, accroche manuscrite dorée, **deux boutons fantômes de même poids** (« Request a quote », « Call us now »).
- **Usabilité** : le lien « Visit Site » mène aujourd'hui à FTCC Group, une entreprise de réparation de sinistres pour assureurs, hors secteur (bench).
- **Hiérarchie visuelle** : aucun CTA ne domine, ce qui contredit l'intention « conversion avant le design ».
- **Accessibilité** : non observable.
- **Ce qui marche** : des chiffres posés avec leur définition à côté (« <24 Hrs » d'intervention, par exemple).
- **Recommandations** : un seul CTA dominant ; ne pas citer ce site comme modèle de conversion, puisque son lien mène aujourd'hui à une autre activité.

---

## 3. Thèmes clés

### Thème 1 : l'argent comme porte d'entrée (prévalence : 3 sites sur 5)
- **Observations** : le simulateur de prime d'Effy, la page aides d'Hellio, la subvention déduite du devis chez Aira.
- **Interprétation** : l'aide est le déclencheur, mais si elle est l'unique message, le site ressemble à une plateforme de primes et rappelle le démarchage. Pour un artisan, l'aide doit accompagner les travaux, pas les remplacer.

### Thème 2 : l'incarnation humaine rassure (prévalence : 2 sites sur 5 de façon nette)
- **Observations** : Aira montre ses installateurs en hero et ses clients au prénom ; Effy titre ses témoignages par une citation.
- **Interprétation** : c'est l'avantage naturel d'un artisan face aux plateformes. Il est sous-exploité par les grands acteurs.

### Thème 3 : des cas chiffrés réels, mais mal placés (prévalence : 2 sites sur 5)
- **Observations** : le cas Hellio d'Orléans (76 %) est dans un communiqué, les cas Aira dans une section dédiée.
- **Interprétation** : le format « ville + travaux + gain » est le plus crédible. Il doit être sur la page principale.

### Thème 4 : la preuve de confiance par des tiers (prévalence : 3 sites sur 5)
- **Observations** : Which? Trusted Trader, Gas Safe et NAPIT chez Aira ; la page avis d'Effy ; le réseau d'artisans « sélectionnés » chez illiCO.
- **Interprétation** : les labels ne rassurent que s'ils sont vérifiables. En France, il faut RGE et Qualibat **avec numéro et lien vers l'annuaire**, plus l'assureur décennale.

### Thème 5 : incohérences et contenus non datés (prévalence : 1 site sur 5 observé, mais flagrant)
- **Observations** : deux contradictions chez Effy, relevées le 2026-11-13 (ancienneté de 15 ou 17 ans, prime jusqu'à 11 000 ou 25 000 €).
- **Interprétation** : pour un public méfiant, une incohérence suffit à faire douter de tout le reste.

### Thème 6 : le SEO local est décisif (prévalence : 1 site sur 5, plus le constat sur les résultats locaux)
- **Observations** : les pages ville d'Aira ; au Pays basque, les annuaires occupent les résultats.
- **Interprétation** : la fiche Google Business Profile et des sections par commune sont le levier le plus rentable pour Arotz.

---

## 4. Insights → Opportunités

| Insight | Opportunité pour Arotz | Impact | Effort |
|---|---|---|---|
| Démarchage interdit, défiance généralisée | Engagement visible « Nous ne vous appellerons jamais sans votre demande », avec lien vers France Rénov' | H | B |
| Les labels ne rassurent que vérifiables | Bloc labels avec numéro RGE et Qualibat, lien vers l'annuaire officiel, assureur décennale et zone couverte | H | B |
| Humain = avantage naturel de l'artisan | Bloc « Qui sommes-nous » court, sans photo (qui, quoi, d'où), chef de chantier référent nommé dans le déroulé | H | B |
| Format le plus crédible : ville + travaux + gain | Avant/après avec classe DPE (F → B), commune, travaux, gain estimé, avis du client | H | M |
| Les aides sont le déclencheur, mais incertaines en 2026 | Estimateur en fourchette, barème daté, « sous réserve d'éligibilité », résultat sans obligation de laisser son téléphone | H | M |
| Annuaires dominants sur le local | Fiche Google soignée, avis réguliers, sections par commune, données structurées LocalBusiness | H | M |
| Coordonner plusieurs corps de métier fait peur | « Un seul interlocuteur, de la visite à la réception », avec le déroulé en 5 étapes | M | B |
| Incohérences chez les plateformes | Chiffres et barèmes centralisés dans le CMS, avec la date de mise à jour visible | M | B |
| Plateformes visuellement interchangeables (bleu, vert, illustrations plates) | Identité basque artisanale : chaux, rouge, sapin, bois, Fraunces | M | B |

---

## 5. Erreurs à éviter

- **Codes du démarchage** :
  - compte à rebours, « PAC à 1 € », pop-up de rappel ;
  - téléphone exigé avant le résultat ;
  - photos de banque d'images.
- **Montants d'aides promis** (« jusqu'à 11 000 € pour vous ») : les barèmes changent, et le guichet a été suspendu en 2026.
- **Logos RGE sans numéro**, ou une qualification non détenue.
- **Greenwashing** (« maison écologique », « zéro carbone », feuilles vertes) : parler de confort, de facture et de DPE.
- **L'oubli du bandeau France Rénov'** : obligatoire depuis le 1er octobre 2026 sur tout support de promotion de travaux de rénovation énergétique, amende jusqu'à 75 000 € pour une personne morale ([France Rénov'](https://france-renov.gouv.fr/actualites/publicite-pour-la-renovation-energetique-obligation-desormais-de-faire-reference-au), vu le 2026-11-13).
- **Pas de numéro cliquable sur mobile.**

## 6. Conclusion appliquée à Arotz Rénovation

- **Positionnement** : « l'artisan RGE du coin qui fait les travaux, monte les dossiers et ne démarche pas ».
- **Hero** : photo réelle de chantier, la promesse du README, le CTA « Visite gratuite » et le numéro cliquable.
- **Preuves** : labels numérotés et vérifiables, avant/après DPE, avis Google liés, déroulé en 5 étapes, « Qui sommes-nous » court, bandeau France Rénov'.
- **Estimateur** honnête qui qualifie la visite, sans piéger un numéro.
- **Identité** basque et artisanale, à l'opposé des plateformes.
- **SEO local** : fiche Google et sections Bayonne, Anglet, Biarritz, Ustaritz, Hasparren, Saint-Jean-Pied-de-Port…

---

## 7. Questions à tester en recherche utilisateur

1. Qu'est-ce qui distingue, aux yeux d'un propriétaire, un artisan sérieux d'un démarcheur sur un site ? Les numéros de labels suffisent-ils ?
2. L'engagement « on ne vous appellera jamais sans demande » rassure-t-il, ou rappelle-t-il le problème ?
3. Quelles informations les gens acceptent-ils de donner dans l'estimateur (revenus, commune, travaux) ? Le revenu fiscal est-il un point d'abandon ?
4. Une fourchette d'aides est-elle comprise et jugée honnête, ou décevante ?
5. Les classes DPE (F → B) parlent-elles autant que des euros économisés par an ?
6. Le basque dans les titres est-il perçu comme un gage de proximité, ou comme une barrière pour les néo-résidents ?

## 8. Notes de méthode

- **Sources** : recherche web en novembre 2026 (pages officielles, presse, annuaires, sources publiques). Chaque chiffre a été revérifié le 2026-11-13 en ouvrant la page citée. Les chiffres qui n'y figuraient pas ont été retirés : la répartition du budget MaPrimeRénov' entre rénovations d'ampleur et par geste, et le bilan des contrôles de la DGCCRF en 2025. La page info.gouv.fr sur la réouverture de MaPrimeRénov' affiche une vérification anti-robots : elle n'est plus citée.
- **Visuels** : Aira, Effy, Hellio (cas d'Orléans) et Final Touch Carpentry ont été ouverts et capturés dans le bench le 2026-11-12. Les sections ci-dessus reprennent ces observations.
- **Limites** :
  - le site d'illiCO travaux n'a été lu qu'en texte, sans capture ; les pages Hellio autres que le cas d'Orléans n'ont pas été vues ;
  - aucun site d'artisan RGE indépendant du Pays basque avec un site remarquable n'a été identifié : la recherche n'a remonté que des annuaires (voir la fiche Effy d'un artisan du 64, bench n° 22).
- **Obligations légales appliquées** : bandeau France Rénov' (France Rénov', ANIL), interdiction du démarchage (loi du 30 juin 2025), allégations environnementales (directive (UE) 2024/825). Sources dans le brief, section 7.
- **Prévalences** : calculées sur 5 sites.
