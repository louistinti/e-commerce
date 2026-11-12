# Étude de cas : site vitrine d'une PME de nettoyage B2B locale

Entreprise du projet : **Brillance Pro**, entreprise **fictive** (nettoyage de bureaux, commerces et fins de chantier à Bordeaux et en Gironde, équipe salariée, contrats sans engagement). Les entreprises analysées sont réelles.

## Executive summary

La propreté pèse environ 21 Md€, mais 55 % du chiffre d'affaires est fait par moins de 5 % des entreprises. Derrière, des milliers de TPE se battent sur Google localement, et les créations d'entreprises sont au record (1,17 million en 2025). Les 5 sites analysés (Lebontri, Onet, Coverall, Stratus, Office Pride) ont tous une logique de pages locales et de devis gratuit. Mais seuls 2 sur 5 donnent un prix indicatif, et aucun ne met en avant l'équipe comme preuve. Brillance Pro peut gagner avec une estimation immédiate suivie d'un devis sous 24 h, de vraies photos de l'équipe salariée et des avis Google datés, sur un gabarit léger et déclinable.

---

## 1. Le marché en 5 lignes

- **Un gros marché très fragmenté** : environ 21 Md€ de chiffre d'affaires en 2024, 15 500 entreprises d'au moins 1 salarié, 600 000 salariés ([Bpifrance Création](https://bpifrance-creation.fr/entrepreneur/actualites/proprete-avenir-eclatant), [Xerfi d'après Le Monde de la Propreté](https://www.xerfi.com/presentationetude/le-marche-des-services-de-nettoyage_SAE11)). 55 % du chiffre d'affaires est fait par les entreprises de plus de 250 salariés, soit moins de 5 % d'entre elles.
- **Les créations d'entreprises sont au record** : 1 165 800 en 2025 (+4,9 %). Le commerce est le premier contributeur, avec une « forte hausse » dans les services administratifs, dont le nettoyage fait partie ([Insee Première n° 2092](https://insee.fr/fr/statistiques/8721354)).
- **À corriger dans le README** : « premier moteur des créations en 2026 selon l'INSEE » n'est **pas confirmé**. En 2026, le soutien aux entreprises oscille : +13,5 % en mai, −4,3 % en juillet ([Insee mai 2026](https://www.insee.fr/fr/statistiques/fichier/version-html/9007871/IR144_CreaE_mai26.pdf), [Insee juillet 2026](https://www.insee.fr/fr/statistiques/fichier/version-html/9037671/IR206_CreaE_juil26.pdf)). Formulation sûre : « l'un des secteurs les plus dynamiques en créations ».
- **Les prix sont lisibles** : 2 à 3,50 € HT par m² pour une PME, 3 à 5 € HT par m² pour un petit bureau ([Companeo](https://www.companeo.com/nettoyage-de-locaux/FAQ/prix-prestation-nettoyage-bureaux-ou-locaux-professionnels)). La croissance annoncée varie de 2,5 à 5 % par an selon les sources.
- **La demande locale est visible** : Bordeaux Métropole a lancé un appel d'offres pour le nettoyage récurrent de ses bâtiments ([BOAMP](https://www.boamp.fr/telechargements/FILES/PDF/2026/04/26-35990.pdf)), et les offres d'emploi d'agents sont nombreuses à Mérignac, Pessac et Bordeaux.

## 2. Analyse de 5 sites réels (framework « design critique »)

> Les pages n'ont **pas** pu être affichées : le réseau de la session bloquait l'accès direct. La première impression, la hiérarchie et l'accessibilité sont évaluées **d'après la description** des résultats de recherche. Contraste et taille de texte : **non observables**.

### 2.1 Lebontri (FR, multi-villes) : https://lebontri.fr/nettoyage-bureau/bordeaux
- **Positionnement** : débarras et nettoyage, avec une page par ville et par prestation.
- **Première impression (2 s)** : la ville et le délai sont dans le title (« Nettoyage de bureau Tours : devis sous 24h », [Tours](https://lebontri.fr/nettoyage-bureau/tours)). L'objectif est clair.
- **Usabilité** : un **simulateur** (surface, nombre de bureaux, fréquence) donne un prix par passage et par mois HT (exemple : 180 € et 720 €, sur la [page Valenciennes](https://lebontri.fr/nettoyage-bureau/valenciennes)). Le devis gratuit suit, après un audit.
- **Hiérarchie visuelle** : promesse locale, puis simulateur, puis inclusions (produits, matériel, hors heures de bureau).
- **Accessibilité** : non observable. **Défaut de contenu relevé** : un texte non rempli (« {city} ») apparaît d'après le résultat de recherche.
- **Ce qui marche** : un prix immédiat, le délai promis, un SEO local ciblé.
- **Recommandations** : 1) relire chaque page générée et supprimer les variables visibles ; 2) préciser si le délai de 24 h vaut partout ; 3) ajouter des preuves locales (avis, chantiers).

### 2.2 Onet Propreté et Services (FR, grand groupe) : https://www.onet.fr/en/agencies/onet-proprete-et-services-lyon/
- **Positionnement** : le leader national, avec des pages par agence.
- **Première impression (2 s)** : une page institutionnelle locale (nom de l'agence, adresse). L'objectif « contacter l'agence » est clair, pas celui d'obtenir un prix.
- **Usabilité** : adresse, téléphone, horaires en semaine, prestations par secteur (bureaux, industrie, commerce, santé). Il n'y a pas de devis immédiat.
- **Hiérarchie visuelle** : agence, puis secteurs, puis certifications (Qualipropre, par exemple au [Mans](https://www.onet.fr/en/agencies/onet-proprete-et-services-le-mans/)).
- **Accessibilité** : non observable. Des pages françaises servies sous `/en/` peuvent fausser l'attribut de langue (à vérifier).
- **Ce qui marche** : le standard nom, adresse, téléphone et horaires, un label sectoriel affiché.
- **Recommandations** : 1) un CTA de devis par agence ; 2) une URL et un attribut `lang` cohérents ; 3) des preuves locales (photos, avis).

### 2.3 Coverall (US, franchise) : https://www.coverall.com/commercial-cleaning-services/janitorial/
- **Positionnement** : un réseau de franchisés de nettoyage commercial.
- **Première impression (2 s)** : un estimateur instantané. L'objectif « savoir combien ça coûte » est clair.
- **Usabilité** : la surface et la fréquence donnent une fourchette mensuelle, avec le périmètre précisé (sols, poussière, poubelles). Un formulaire séparé sert aux besoins ponctuels ([get-a-quote](https://www.coverall.com/get-a-quote/)).
- **Hiérarchie visuelle** : estimation, puis périmètre, puis visite sur place présentée comme l'étape suivante.
- **Accessibilité** : non observable.
- **Ce qui marche** : un prix tout de suite, une [page de pédagogie du prix](https://www.coverall.com/commercial-cleaning-services/pricing-commercial-cleaning-services-for-your-business/), des avis Google exploités ([Fresno, plus de 100 avis 5 étoiles](https://www.coverall.com/in-the-news/coverall-of-fresno-reinforces-role-as-the-best-commercial-cleaning-provider-with-5-star-rating-and-over-100-google-reviews/)).
- **Recommandations** : 1) fusionner les deux parcours (récurrent et ponctuel) en un seul formulaire à embranchement ; 2) remplacer les communiqués « best in X » par des avis intégrés.

### 2.4 Stratus Building Solutions (US, franchise) : https://www.stratusclean.com/
- **Positionnement** : nettoyage commercial, avec des pages devis par ville ([Miami](https://www.stratusclean.com/locations/miami/get-quote/)).
- **Première impression (2 s)** : le message « la plupart des devis sont bâtis sur des hypothèses, les nôtres sur vos locaux » justifie la visite.
- **Usabilité** : un [formulaire](https://www.stratusclean.com/get-quote/) court (nom, société, téléphone, e-mail, code postal, service). Il ne demande ni la surface ni la fréquence.
- **Hiérarchie visuelle** : message, formulaire, visite.
- **Accessibilité** : non observable.
- **Ce qui marche** : un argument qui transforme l'absence de prix en gage de sérieux, une page devis par ville.
- **Recommandations** : 1) demander la surface et la fréquence pour qualifier ; 2) donner au moins un ordre de prix.

### 2.5 Office Pride (US, franchise) : https://officepride.com/
- **Positionnement** : nettoyage de bureaux et de locaux commerciaux, avec des équipes locales ([Colorado Springs](https://officepride.com/colorado-springs-downtown/)).
- **Première impression (2 s)** : le CTA « Request a Quote ».
- **Usabilité** : des pages par implantation et une consultation sur place « free, no-obligation ».
- **Hiérarchie visuelle** : CTA, implantation, consultation.
- **Accessibilité** : non observable.
- **Ce qui marche** : la proximité et l'absence d'engagement formulée clairement.
- **Recommandations** : 1) un prix indicatif ; 2) un élément différenciant (équipe, méthode) face aux autres franchises.

Référence complémentaire : le [devis express de Companeo](https://www.companeo.com/nettoyage-de-locaux/devis-express), une plateforme qui envoie plusieurs devis sous 48 h. C'est le concurrent indirect sur les mêmes recherches.

## 3. Thèmes clés

| Thème | Prévalence | Observations | Interprétation |
|---|---|---|---|
| Pages locales (ville, agence, quartier) | **5 sur 5** | Lebontri par ville, Onet par agence, Coverall, Stratus et Office Pride par implantation | Le SEO local est l'enjeu n° 1. Pour une seule ville, la profondeur (communes, chantiers locaux) compte plus que le nombre de pages. |
| Devis gratuit suivi d'une visite | **5 sur 5** | Lebontri (audit), Coverall (walkthrough), Stratus, Office Pride (consultation), Onet (contact agence) | La visite est la norme acceptée. Il ne faut pas la supprimer, mais la rendre légère (« 20 min, sans engagement »). |
| Prix indicatif immédiat | **2 sur 5** | Lebontri (simulateur), Coverall (fourchette) | Un avantage net, encore rare. |
| Avis exploités | **1 sur 5** confirmé | Coverall (communiqués avis Google) | Les avis sont sous-exploités sur les sites alors qu'ils pèsent dans le pack local. |
| Labels sectoriels | **1 sur 5** confirmé | Onet (Qualipropre) | Un signal de sérieux, à n'afficher que s'il est obtenu. |
| Équipe montrée | **0 sur 5** (d'après les recherches) | Aucun site ne met en avant les agents nommés ou le statut salarié dans les extraits | Le différenciateur le plus disponible pour Brillance Pro. |
| Défauts des pages générées | **1 sur 5** | Lebontri (« {city} ») | Le principal risque du SEO local à grande échelle. |

## 4. Insights → Opportunités

| Insight | Opportunité | Impact | Effort |
|---|---|---|---|
| Seuls 2 sites sur 5 donnent un prix | Fourchette indicative à l'étape 2 du devis, avant les coordonnées | H | M |
| Visite systématique, mais vécue comme une friction | « Visite de 20 min offerte, devis écrit sous 24 h » en microcopie | M | B |
| L'équipe n'est jamais montrée | Photos réelles et prénoms, mention « salariés, déclarés, assurés » | H | M |
| Avis sous-exploités | Note Google dans le hero et 3 verbatims datés, objectif de 30 avis | H | B |
| Pages générées fautives | Pas de pages-villes en masse : une liste des communes en HTML et 3 pages SEO rédigées | M | B |
| Les plateformes captent les recherches (devis sous 48 h) | Promesse de 24 h et interlocuteur direct | M | B |
| Besoin de déclinaison pour d'autres métiers | Gabarit à blocs paramétrables (prestations, communes, accent couleur) | M | M |

## 5. Erreurs à éviter

- **Le site générique** : banque d'images, « solutions sur mesure », aucune ville.
- **Les pages locales générées avec des variables visibles** ou des textes dupliqués.
- **Le formulaire à 15 champs**, ou au contraire sans surface ni fréquence.
- **Les labels non obtenus** (Qualipropre, Ecolabel, ISO 14001).
- **Les avis inventés ou copiés** : c'est une pratique commerciale trompeuse.
- **Un téléphone non cliquable.**

## 6. Conclusion appliquée à Brillance Pro

- Brillance Pro se positionne comme **« l'équipe de ménage de vos bureaux, salariée, locale, sans engagement »**.
- Le hero porte la ville et le délai. Le CTA principal est « Obtenir mon estimation » et le téléphone est cliquable.
- Le devis se fait en 3 étapes : type de local, surface et fréquence (la fourchette s'affiche), puis coordonnées.
- Pour le SEO local : la ville dans le title et le H1, une fiche Google Business Profile, les données structurées `LocalBusiness`, la liste des communes en HTML.
- Le gabarit est déclinable pour la sécurité, la maintenance ou les espaces verts.
- Le nom est provisoire et fictif : il faut vérifier l'INPI, car il est probablement déjà utilisé.

## 7. Questions à valider en recherche utilisateur

1. Une office manager connaît-elle la surface de ses locaux ? Faut-il proposer des tranches (moins de 100 m², 100 à 300 m², etc.) ou un nombre de postes ?
2. Une fourchette indicative rassure-t-elle, ou crée-t-elle une ancre de prix qui gêne la négociation ?
3. Qu'est-ce qui prouve le mieux le sérieux : la mention « salariés et assurés », la note Google, une photo de l'équipe, ou un label ?
4. « Sans engagement » est-il crédible tel quel, ou faut-il préciser le préavis ?
5. Sur mobile, préfère-t-on appeler ou remplir le devis ? Cela varie-t-il selon le persona (commerçant ou conductrice de travaux) ?
6. Les avant/après sont-ils regardés, et sont-ils jugés authentiques ?

## 8. Notes de méthode

- **Sources** : recherches web (novembre 2026) sur les sites des entreprises, les études de marché (Xerfi, Bpifrance Création), l'Insee et les plateformes (Companeo).
- **Limites** :
  - **les visuels n'ont pas été vus** : l'accès direct est bloqué par le réseau de la session, donc le critique est fondé sur les textes et la structure décrits ;
  - l'accessibilité et le mobile ne sont pas évalués ;
  - **aucun concurrent bordelais n'a pu être analysé** en profondeur : les recherches locales renvoyaient surtout vers des annuaires et des offres d'emploi, et le budget de recherche a été épuisé ;
  - l'échantillon compte 2 sites français et 3 américains, ce qui surreprésente les franchises américaines ;
  - les chiffres de croissance du secteur divergent selon les sources.
