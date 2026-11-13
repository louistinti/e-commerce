# Étude de cas : site vitrine d'une PME de nettoyage B2B locale

Entreprise du projet : **Brillance Pro**, entreprise **fictive** (nettoyage de bureaux, commerces et fins de chantier à Bordeaux et en Gironde, équipe salariée, contrats sans engagement). Les entreprises analysées sont réelles. Aucun chiffre n'est inventé : chaque donnée chiffrée porte sa source et sa date de consultation.

## Executive summary

La propreté pèse 21 Md€ de chiffre d'affaires en 2024, pour 15 500 entreprises d'au moins 1 salarié, en majorité des TPE et des PME ([Bpifrance Création](https://bpifrance-creation.fr/entrepreneur/actualites/proprete-avenir-eclatant), vu le 2026-11-13). Les créations d'entreprises atteignent un record en 2025, et elles progressent de 12 % dans les services administratifs et de soutien, dont relève le nettoyage ([Insee Première n° 2092](https://insee.fr/fr/statistiques/8721354), vu le 2026-11-13). Les 5 sites analysés (Lebontri, Onet, Coverall, Stratus, Office Pride) misent tous sur des pages locales et un devis gratuit. Parmi les 4 sites vérifiés dans le bench, aucun n'affiche un prix avant les coordonnées ou la création d'un compte, et aucun ne nomme ses agents. Brillance Pro peut se distinguer avec un repère de prix affiché avant les coordonnées, un bloc « Qui sommes-nous » direct et un bloc avis daté, sur un gabarit léger et déclinable.

---

## 1. Le marché en 4 lignes

- **Un gros marché de TPE et de PME** : 21 Md€ de chiffre d'affaires en 2024, 15 500 entreprises d'au moins 1 salarié, 600 000 personnes employées ([Bpifrance Création](https://bpifrance-creation.fr/entrepreneur/actualites/proprete-avenir-eclatant), vu le 2026-11-13). Xerfi, d'après Le Monde de la Propreté, donne le même ordre de grandeur pour 2024 et décrit un secteur fait surtout de TPE et de micro-entreprises, face à quelques grands groupes ([Xerfi](https://www.xerfi.com/presentationetude/le-marche-des-services-de-nettoyage_SAE11), vu le 2026-11-13).
- **Les créations d'entreprises sont au record** : 1 165 800 en 2025 (+5 %). Elles progressent de 12 % dans les activités de services administratifs et de soutien, dont relève le nettoyage ([Insee Première n° 2092](https://insee.fr/fr/statistiques/8721354), vu le 2026-11-13). Bpifrance Création range la propreté parmi les services aux entreprises les plus dynamiques (même page que ci-dessus).
- **Les prix sont publiés** : 3 à 5 € HT par m² pour de petits bureaux ou commerces, 2 à 3,50 € HT par m² pour une PME ou une surface intermédiaire ([Companeo](https://www.companeo.com/nettoyage-de-locaux/FAQ/prix-prestation-nettoyage-bureaux-ou-locaux-professionnels), page mise à jour le 25/05/2026, vue le 2026-11-13).
- **La demande locale est visible** : Bordeaux Métropole a lancé un appel d'offres pour le nettoyage récurrent de ses bâtiments ([BOAMP](https://www.boamp.fr/telechargements/FILES/PDF/2026/04/26-35990.pdf)), et les offres d'emploi d'agents sont nombreuses à Mérignac, Pessac et Bordeaux.

## 2. Analyse de 5 sites réels (framework « design critique »)

> Les pages ont été ouvertes et capturées le 2026-11-12 (détail et captures dans le [bench](BENCH.md)), sauf les pages Stratus, bloquées par une protection anti-robots. Les constats ci-dessous suivent le bench. Les couleurs et contrastes viennent des styles calculés de la page.

### 2.1 Lebontri (FR, plateforme multi-villes) : https://lebontri.fr/nettoyage-bureau/bordeaux
- **Positionnement** : une plateforme d'annonces. Des intervenants vérifiés répondent aux demandes, avec un acompte de 10 %. Ce n'est pas une entreprise de nettoyage.
- **Première impression (2 s)** : le H1 « Nettoyage de bureaux à Bordeaux – Service sur mesure pour entreprises », une pastille « Bordeaux et alentours · intervenants vérifiés ». L'objectif est clair. La promesse « devis sous 24h » a disparu du title ([Tours](https://lebontri.fr/nettoyage-bureau/tours)).
- **Usabilité** : le « simulateur » n'a ni champ ni prix. L'estimation est floutée (« ••• € ») et demande un compte ([page Valenciennes](https://lebontri.fr/nettoyage-bureau/valenciennes)).
- **Hiérarchie visuelle** : promesse locale, puis CTA d'estimation, puis 4 cartes de facteurs de prix (surface, fréquence, prestations, horaires).
- **Accessibilité** : CTA vert clair `#D1ED92`, texte `#12372A`, 10,1:1.
- **Défaut de contenu relevé** : aucune variable « {city} » visible. Le vrai défaut est la duplication : d'une ville à l'autre, seuls la ville, la fin du H1 et le département changent.
- **Ce qui marche** : la pastille locale, la micro-ligne « Gratuit · 3 minutes · une photo suffit », les facteurs de prix expliqués.
- **Recommandations** : 1) rédiger chaque page-ville au lieu de la dupliquer ; 2) montrer l'estimation sans compte ; 3) ajouter des preuves locales (avis, chantiers).

### 2.2 Onet Propreté et Services (FR, grand groupe) : https://www.onet.fr/en/agencies/onet-proprete-et-services-lyon/
- **Positionnement** : le leader national, avec des pages par agence.
- **Première impression (2 s)** : une vraie photo d'agent en tenue, de dos, logo visible, sur tout le hero. L'objectif « contacter l'agence » est clair, pas celui d'obtenir un prix.
- **Usabilité** : adresse, téléphone, horaires (lundi au vendredi, 8 h-12 h et 14 h-17 h), prestations par secteur. Il n'y a pas de devis immédiat.
- **Hiérarchie visuelle** : agence, puis secteurs, puis certifications (Qualipropre, par exemple au [Mans](https://www.onet.fr/en/agencies/onet-proprete-et-services-le-mans/)).
- **Accessibilité** : du blanc sur `#F34028` (3,8:1) et sur `#41C5E7` (2,0:1), sous le seuil AA. La page `/en/` est bien la version anglaise : title en anglais et attribut `lang="en"` (vu le 2026-11-13). Il n'y a donc pas d'incohérence de langue.
- **Ce qui marche** : le standard nom, adresse, téléphone et horaires, les données `LocalBusiness`, un label sectoriel expliqué.
- **Recommandations** : 1) un CTA de devis par agence ; 2) un seul CTA primaire et des contrastes AA ; 3) des preuves locales (avis).

### 2.3 Coverall (US, franchise) : https://www.coverall.com/commercial-cleaning-services/janitorial/
- **Positionnement** : un réseau de franchisés de nettoyage commercial.
- **Première impression (2 s)** : un H1 en capitales condensées et un estimateur annoncé comme « instantané ».
- **Usabilité** : l'estimateur compte 10 champs et exige les coordonnées avant la fourchette. Un formulaire séparé sert aux besoins ponctuels ([get-a-quote](https://www.coverall.com/get-a-quote/)), avec 6 champs obligatoires dont les coordonnées.
- **Hiérarchie visuelle** : estimation, puis périmètre en 5 tâches (sols, déchets, aspirateur, poussière, surfaces), puis visite sur place.
- **Accessibilité** : CTA blanc sur `#00AB48`, 3,0:1, sous le seuil AA.
- **Ce qui marche** : le périmètre court, le paragraphe « How we determine your quote », une [page de pédagogie du prix](https://www.coverall.com/commercial-cleaning-services/pricing-commercial-cleaning-services-for-your-business/), des avis Google mis en avant par communiqué ([Fresno, plus de 100 avis 5 étoiles](https://www.coverall.com/in-the-news/coverall-of-fresno-reinforces-role-as-the-best-commercial-cleaning-provider-with-5-star-rating-and-over-100-google-reviews/)).
- **Recommandations** : 1) afficher la fourchette avant les coordonnées ; 2) fusionner les deux parcours (récurrent et ponctuel) en un seul formulaire à embranchement ; 3) remplacer les communiqués par des avis intégrés et datés.

### 2.4 Stratus Building Solutions (US, franchise) : https://www.stratusclean.com/
> **Non vérifié** : le 2026-11-12, les pages affichaient un challenge Cloudflare, non contourné. Les constats viennent des résultats de recherche.
- **Positionnement** : nettoyage commercial, avec des pages devis par ville ([Miami](https://www.stratusclean.com/locations/miami/get-quote/)).
- **Première impression (2 s)** : le message « la plupart des devis sont bâtis sur des hypothèses, les nôtres sur vos locaux » justifie la visite.
- **Usabilité** : un [formulaire](https://www.stratusclean.com/get-quote/) court (nom, société, téléphone, e-mail, code postal, service). Il ne demande ni la surface ni la fréquence.
- **Hiérarchie visuelle** : message, formulaire, visite.
- **Accessibilité** : non observable.
- **Ce qui marche** : un argument qui transforme l'absence de prix en gage de sérieux.
- **Recommandations** : 1) demander la surface et la fréquence pour qualifier ; 2) donner au moins un ordre de prix.

### 2.5 Office Pride (US, franchise) : https://officepride.com/
- **Positionnement** : nettoyage de bureaux et de locaux commerciaux, avec des équipes locales ([Colorado Springs](https://officepride.com/colorado-springs-downtown/)).
- **Première impression (2 s)** : une photo d'équipe en polos sous un dégradé bleu, la ville sous le H1, le téléphone en bouton blanc à côté du CTA « Request a Quote ».
- **Usabilité** : un formulaire « Step 1 of 3 » avec barre de progression, visible dès le hero, mais qui demande les coordonnées dès l'étape 1. La mention « free, no-obligation » n'existe plus sur la page.
- **Hiérarchie visuelle** : CTA, formulaire, 3 réassurances (« Highly reviewed · Locally owned · Professional crews »).
- **Accessibilité** : « Request a Quote » blanc sur `#00964D`, 3,8:1, sous le seuil AA.
- **Ce qui marche** : la proximité, le formulaire découpé en étapes, les réassurances courtes.
- **Recommandations** : 1) un prix indicatif ; 2) les coordonnées en dernière étape ; 3) un CTA au contraste AA.

Référence complémentaire : le [devis express de Companeo](https://www.companeo.com/nettoyage-de-locaux/devis-express), un comparateur qui met en relation avec 4 sociétés et promet une demande en « 60 secondes chrono ». C'est le concurrent indirect sur les mêmes recherches.

## 3. Thèmes clés

| Thème | Prévalence | Observations | Interprétation |
|---|---|---|---|
| Pages locales (ville, agence, quartier) | **5 sur 5** (Stratus non vérifié) | Lebontri par ville, Onet par agence, Coverall, Stratus et Office Pride par implantation | Le SEO local est l'enjeu n° 1. Pour une seule ville, la profondeur (communes, contenus rédigés) compte plus que le nombre de pages. |
| Devis gratuit suivi d'une visite | **5 sur 5** | Lebontri (audit), Coverall (visite sur place), Stratus, Office Pride, Onet (contact agence) | La visite est la norme acceptée. Il ne faut pas la supprimer, mais la présenter comme légère et sans engagement. |
| Prix avant les coordonnées | **0 sur 4** vérifiés | Lebontri floute l'estimation et demande un compte, Coverall exige les coordonnées | La place est libre : personne ne montre un ordre de prix d'emblée. |
| Avis exploités | **1 sur 5** | Coverall (communiqués sur ses avis Google) | Les avis sont sous-exploités sur les sites. |
| Labels sectoriels | **1 sur 5** | Onet (Qualipropre) | Un signal de sérieux. Brillance Pro, fictive, n'affiche aucun logo de label. |
| Équipe montrée | **2 sur 4** vérifiés en photo, **0** qui nomme ses agents | Onet (un agent en tenue), Office Pride (une équipe en polos). Aucun prénom, aucune mention du statut salarié | Le statut salarié et un interlocuteur nommé restent libres. |
| Pages dupliquées | **1 sur 5** | Lebontri (Tours et Bordeaux ne diffèrent que par la ville) | Le principal risque du SEO local à grande échelle. |

## 4. Insights → Opportunités

| Insight | Opportunité | Impact | Effort |
|---|---|---|---|
| Aucun site vérifié ne montre un prix avant les coordonnées | Repère de prix au m² à l'étape 2 du devis, avant les coordonnées, avec sa source | H | M |
| Visite systématique, mais vécue comme une friction | « Visite offerte, sans engagement » en microcopie | M | B |
| Aucun site ne nomme ses agents ni leur statut | Bloc « Qui sommes-nous » court : équipe salariée et assurée, responsable d'exploitation, sans photo | H | B |
| Avis sous-exploités | Bloc avis avec note, nombre, 3 verbatims datés et lien vers la fiche ; dans la démo, gabarit marqué « Exemple de mise en page » | H | B |
| Pages dupliquées d'une ville à l'autre | Pas de pages-villes en masse : une liste des communes en HTML et 3 pages SEO rédigées | M | B |
| Les plateformes captent les recherches | Estimation immédiate et interlocuteur direct | M | B |
| Besoin de déclinaison pour d'autres métiers | Gabarit à blocs paramétrables (prestations, communes, accent couleur) | M | M |

## 5. Erreurs à éviter

- **Le site générique** : banque d'images, « solutions sur mesure », aucune ville.
- **Les pages locales dupliquées** d'une ville à l'autre.
- **Le formulaire à 15 champs**, ou au contraire sans surface ni fréquence.
- **Les labels non obtenus** (Qualipropre, Ecolabel, ISO 14001).
- **Les avis inventés ou copiés** : c'est une pratique commerciale trompeuse.
- **Un téléphone non cliquable.**

## 6. Conclusion appliquée à Brillance Pro

- Brillance Pro se positionne comme **« l'équipe de ménage de vos bureaux, salariée, locale, sans engagement »**.
- Le hero porte la ville et l'estimation en ligne : « Nettoyage de bureaux à Bordeaux, estimation en ligne immédiate ». Le CTA principal est « Obtenir mon estimation » et le téléphone est cliquable.
- Le devis se fait en 3 étapes : type de local, surface et fréquence (le repère de prix au m² s'affiche), puis coordonnées.
- Pour le SEO local : la ville dans le title et le H1, les données structurées `LocalBusiness`, la liste des communes en HTML.
- Le gabarit est déclinable pour la sécurité, la maintenance ou les espaces verts.
- Le nom est fictif et réservé à la démo : on ne le dépose pas et on ne le réutilise pas pour une entreprise réelle.

## 7. Questions pour la recherche utilisateur

1. Une office manager connaît-elle la surface de ses locaux ? Faut-il proposer des tranches (moins de 100 m², 100 à 300 m², etc.) ou un nombre de postes ?
2. Un repère de prix rassure-t-il, ou crée-t-il une ancre qui gêne la négociation ?
3. Qu'est-ce qui prouve le mieux le sérieux : la mention « salariés et assurés », la note Google, le bloc « Qui sommes-nous », ou un label ?
4. « Sans engagement » est-il crédible tel quel, ou faut-il préciser le préavis ?
5. Sur mobile, préfère-t-on appeler ou remplir le devis ? Cela varie-t-il selon le persona (commerçant ou conductrice de travaux) ?
6. Les avant/après sont-ils regardés, même légendés « photo d'illustration » ?

## 8. Notes de méthode

- **Sources** : recherches web (novembre 2026) sur les sites des entreprises, les études de marché (Xerfi, Bpifrance Création), l'Insee et les plateformes (Companeo). Les sources chiffrées ont été rouvertes le 2026-11-13. Les chiffres qu'aucune page ouverte n'affichait ont été retirés : la part de 55 % du chiffre d'affaires faite par les grandes entreprises, les taux de croissance annuelle du secteur, les évolutions mensuelles des créations en 2026.
- **Limites** :
  - les visuels ont été vus et capturés le 2026-11-12 (bench), sauf Stratus ;
  - les contrastes et le mobile sont relevés dans le bench, sans audit d'accessibilité complet ;
  - **aucun concurrent bordelais n'a pu être analysé** en profondeur : les recherches locales renvoyaient surtout vers des annuaires et des offres d'emploi, et le budget de recherche a été épuisé ;
  - l'échantillon compte 2 sites français et 3 américains, ce qui surreprésente les franchises américaines.
