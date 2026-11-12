# Étude de cas : site vitrine industrie 4.0 / maintenance prédictive

> Document de travail de l'agence. **Vibra est une entreprise fictive.** Les entreprises analysées sont réelles. Leurs sites **n'ont pas pu être ouverts** (réseau de la session bloqué) : les critiques reposent sur les pages indexées, les documents publics (PDF, références) et la presse. Voir les notes de méthode en fin de document.

## Executive summary

La robotique et la « physical AI » battent des records de financement (27,6 Md$ en 2025 selon PitchBook). La maintenance prédictive, elle, se vend sur un argument simple : le coût d'un arrêt non planifié. Les 6 sites étudiés convergent : hero « uptime », capture de tableau de bord, études de cas souvent en PDF, CTA « démo ». Aucun ne met le téléphone ni un essai sur machine au premier plan, alors que les PME achètent ainsi. Pour Vibra, l'opportunité est un site « fiche technique » : français, sans buzzword, avec des photos réelles, des témoignages nommés en HTML, et trois actions (tester, appeler, télécharger).

## 1. Le marché en 5 lignes

- **Records de financement robotique** : PitchBook compte 27,6 Md$ sur 1 009 opérations en 2025, plus du double de 2024. Crunchbase, sur un périmètre plus étroit, donne 13,8 Md$ contre 7,8 Md$ ([synthèse](https://ai2.work/blog/robotics-startup-funding-doubles-to-27-6b-on-physical-ai-boom)).
- **La « physical AI » s'accélère** : 47,4 Md$ sur 521 opérations au S1 2026 ([Crunchbase News](https://news.crunchbase.com/venture/physical-ai-funding-startups-robotics-aerospace-h1-2026/)).
- **L'arrêt coûte cher** : 1 400 Md$ par an pour le Fortune Global 500, soit 11 % du chiffre d'affaires (contre 8 % en 2019-2020). Dans l'automobile, jusqu'à 2,3 M$ de l'heure ([Siemens TCOD 2024](https://assets.new.siemens.com/siemens/assets/api/uuid:1b43afb5-2d07-47f7-9eb7-893fe7d0bc59/TCOD-2024_original.pdf), synthèse [automation.com](https://www.automation.com/en-us/assets/white-papers/white-paper-true-costs-downtime-2024)).
- **La filière française se structure et se consolide** :
  - Wormsensing (CEA-Leti) a levé 9,5 M€ en série A ([Wormsensing](https://www.wormsensing.com/news/wormsensing-raises-9-5-million-series-a)).
  - I-care a racheté les actifs d'Amiral Technologies en septembre 2026 ([PR Newswire](https://www.prnewswire.com/fr/communiques-de-presse/i-care-group-acquiert-amiral-technologies-et-renforce-son-offre-de-maintenance-predictive-basee-sur-lia-notamment-dans-les-secteurs-du-nucleaire-et-de-la-defense-302881112.html)).
- **Pour une PME, l'argument est l'heure d'arrêt évitée.** Ordres de grandeur cités par les synthèses : environ 125 000 $ par heure en médiane selon ABB, environ 260 000 $ selon Aberdeen (sources primaires non consultées).

Le chiffre « +185 % sur un an » du README n'a pas été retrouvé : il faut le remplacer par les chiffres ci-dessus ou le sourcer.

## 2. Critique de 6 sites réels

Grille utilisée : première impression (2 s), usabilité, hiérarchie visuelle, accessibilité, ce qui marche, recommandations. « Non observé » signifie qu'une visite visuelle est nécessaire.

### 2.1 Wormsensing (France, Grenoble), capteur piézoélectrique Dragonfly®
- **URL** : https://www.wormsensing.com/
- **Positionnement** : un capteur ultrafin (environ 150 µm) et une plateforme, « born at CEA-Leti, made in Grenoble ».
- **Première impression** : non observée. Le titre de la home (« Dragonfly® piezoelectric vibration sensors ») annonce clairement l'objet, mais vise un lecteur technique.
- **Usabilité** : une navigation courte (Capteurs, Plateforme, cas d'usage, About, News), une gamme en 3 versions (Passive, IEPE, IO). Le CTA n'a pas été observé.
- **Hiérarchie** : les fiches sont denses en spécifications (IP67, M12, 150 °C, de 0,01 Hz à 100 kHz).
- **Accessibilité** : non observée.
- **Ce qui marche** :
  - L'ancrage scientifique et territorial dès les titres.
  - Un livre blanc co-signé avec ifm (un industriel connu).
- **Recommandations** :
  1. Ajouter une entrée « responsable maintenance », sans unités de R&D (nε, µdef).
  2. Publier un témoignage d'usine nommé.
  3. Proposer une version française.

### 2.2 I-care (Belgique, présent en France), service de maintenance prédictive et capteur Wi-care
- **URL** : https://www.icareweb.com/ppc/wireless-vibration-sensor ; [étude de cas Barry Callebaut, Louviers (PDF)](https://www.icareweb.com/wp-content/uploads/2022/06/FR-I-care-Barry-Callebaut-Success-Story.pdf.pdf)
- **Positionnement** : un service complet (capteurs, plateforme I-see, analystes), en abonnement « Wi-care as a Service ».
- **Première impression** : non observée. Ce sont des landing pages publicitaires par mot-clé (`/ppc/…`).
- **Usabilité** : le contenu est éclaté entre pages ppc, brochures PDF et sous-sites pays. La preuve est enfermée dans des PDF, ce qui est difficile sur mobile.
- **Hiérarchie** : non observée. Les brochures mettent en avant l'ATEX et l'abonnement.
- **Accessibilité** : les PDF ne sont probablement pas balisés. Non vérifié.
- **Ce qui marche** :
  - Une étude de cas qui nomme **le client et le site**.
  - L'abonnement qui supprime l'investissement initial.
  - Le produit est annoncé comme utilisable par du personnel non formé (Wi-care PURE).
- **Recommandations** :
  1. Passer les études de cas en HTML.
  2. Unifier le parcours sur une seule page produit.

### 2.3 Exotec (France, Lille), robots d'entrepôt Skypod
- **URL** : https://www.exotec.com/ (FR : https://www.exotec.com/fr/solution/)
- **Positionnement** : un intégrateur et constructeur qui combine robotique, logiciel (Deepsky) et expertise opérationnelle.
- **Première impression** : non observée.
- **Usabilité** : découpage par système, par secteur (alimentaire, santé, industrie) et par ressources. Le site est bilingue. Une visite virtuelle à 360° remplace la visite de site.
- **Hiérarchie** : fiches techniques franches (30 kg, 4 m/s) et preuves chiffrées et nommées (Renault Villeroy : 191 robots).
- **Accessibilité** : la visite à 360° nécessite une alternative. Non vérifié.
- **Ce qui marche** : la preuve nommée, le découpage sectoriel et l'immersion maîtrisée.
- **Recommandations pour notre usage** : un ton grand compte à adapter, avec des actions plus courtes (essai, téléphone).

### 2.4 Siemens Senseye (Royaume-Uni / Allemagne), logiciel de maintenance prédictive
- **URL** : https://www.siemens.com/en-us/products/industrial-digitalization-services/senseye-predictive-maintenance/ ; [référence usine de Cham](https://references.siemens.com/en/reference/44824?id=44824)
- **Positionnement** : la maintenance prédictive « at scale », avec un copilote IA générative.
- **Première impression** : non observée. Le produit est inclus dans la navigation du groupe Siemens.
- **Usabilité** : une bibliothèque de références par site (Cham, Sachsenmilch, BlueScope). Le chemin vers le produit est long, car le site est celui d'un groupe.
- **Hiérarchie** : chiffres en « jusqu'à » clairement attribués (jusqu'à −50 % d'arrêts non planifiés).
- **Accessibilité** : non observée.
- **Ce qui marche** : du contenu d'autorité (le rapport True Cost of Downtime) et des références nommées par usine.
- **Recommandations pour notre usage** : reprendre le format de la référence par site, pas l'architecture de groupe.

### 2.5 Augury (États-Unis / Israël), Machine Health : référence internationale
- **URL** : https://www.augury.com/ ; https://www.augury.com/machine-health/
- **Positionnement** : l'IA industrielle pour la disponibilité et la productivité.
- **Première impression** : d'après le titre de la home (« Industrial AI for Uptime & Productivity »), une promesse claire mais très orientée IA.
- **Usabilité** : 2 produits (Machine Health, Process Health), des landing pages publicitaires et un gros blog SEO.
- **Hiérarchie** : la preuve chiffrée est mise en avant (−75 % de fausses alertes ; ROI de 310 % selon une étude Forrester TEI commandée).
- **Accessibilité** : non observée.
- **Ce qui marche** : posséder une catégorie (« Machine Health ») et un abonnement par machine lisible.
- **Recommandations pour notre usage** :
  1. Garder la clarté, retirer le vocabulaire IA.
  2. Toujours signaler une étude commandée.

### 2.6 Tractian (Brésil / États-Unis), capteurs et GMAO : référence internationale
- **URL** : https://tractian.com/en/solutions/condition-monitoring
- **Positionnement** : un capteur multisignal (Smart Trac) et une GMAO, avec une installation rapide.
- **Première impression** : non observée.
- **Usabilité** : pages solutions, fiches capteur et comparatifs de blog.
- **Hiérarchie** : spécifications de terrain en avant (IP69K, zones dangereuses, batterie de 3 à 5 ans, passerelle 4G indépendante du Wi-Fi de l'usine, rapport initial en 5 jours).
- **Accessibilité** : non observée.
- **Ce qui marche** :
  - Lever l'objection de la DSI (pas de réseau usine).
  - Une promesse de délai.
- **Recommandations pour notre usage** : éviter les comparatifs « Top 5 » où l'auteur se classe premier. C'est efficace en SEO mais cela abîme la confiance.

Consulté en surface : Sereact (Allemagne, https://sereact.ai/product/pick-and-place), qui affiche ses chiffres de performance en tête de page produit.

## 3. Thèmes clés

### T1 : La promesse de disponibilité dans le hero
- **Prévalence** : 4 sites sur 6 (Augury « Uptime », Senseye « at scale », Tractian, I-care).
- **Observation** : les titres de pages tournent autour de l'uptime, de la prévention et de la disponibilité.
- **Interprétation** : la promesse est devenue générique. Il faut la rendre concrète (un délai : « 3 semaines avant »).

### T2 : La preuve nommée existe, mais elle est souvent enfermée
- **Prévalence** : 4 sur 6 citent des clients nommés (I-care, Exotec, Senseye, Augury via Forrester). Sur ces 4, au moins 1 publie l'étude de cas principalement en PDF (I-care).
- **Interprétation** : les témoignages nommés par site sont la norme attendue. Le format HTML, visible sur mobile, est un différenciant.

### T3 : La fiche technique comme argument de vente
- **Prévalence** : 4 sur 6 (Wormsensing, Tractian, Exotec, I-care pour l'ATEX).
- **Observation** : spécifications d'environnement (IP, température, ATEX) et d'autonomie en avant.
- **Interprétation** : ce public lit d'abord la fiche. Elle doit être accessible en un tap, sans formulaire.

### T4 : Le vocabulaire IA domine
- **Prévalence** : 3 sur 6 (Augury, Senseye avec un copilote d'IA générative, Sereact pour la robotique). Wormsensing et Tractian restent plus factuels.
- **Interprétation** : un directeur d'usine de PME y lit du buzzword. Un ton factuel est un différenciant à coût nul.

### T5 : Aucun canal téléphone ni essai sur machine mis en avant
- **Prévalence** : 0 sur 6 (d'après les pages indexées). Le CTA dominant semble être « démo » ou un contact. Non vérifié visuellement.
- **Interprétation** : c'est l'opportunité la plus nette pour une PME qui vend à des PME.

### T6 : Lever l'objection informatique
- **Prévalence** : 1 sur 6 explicitement (Tractian avec la passerelle 4G).
- **Interprétation** : les DSI bloquent souvent ces projets. Un encart d'architecture et d'hébergement UE est peu coûteux et lève le frein.

## 4. Insights → Opportunités

| Insight | Opportunité | Impact | Effort |
|---|---|---|---|
| Aucun site ne met le téléphone en avant | Barre « Appeler un technicien » fixe sur mobile, avec le nom et les horaires | H | B |
| « Démo » est le CTA par défaut | « Tester sur une machine » : pilote de 6 semaines avec un périmètre clair | H | M |
| Les études de cas sont souvent en PDF | 3 témoignages en HTML (photo, nom, site, machine, panne évitée) | H | M |
| La promesse « uptime » est générique | Une promesse chiffrée et datée (« jusqu'à 3 semaines avant », avec son périmètre) | H | B |
| La fiche technique est déterminante | Fiche technique en un tap, sans formulaire, plus un résumé HTML | H | B |
| Le jargon IA est omniprésent | Ton factuel, vocabulaire de maintenancier (roulement, balourd, GMAO) | M | B |
| L'objection de la DSI est rarement traitée | Encart « 4G autonome, hébergement UE », plus une fiche sécurité | M | B |
| Le coût d'arrêt est le premier argument | Mini calculateur (chiffre d'affaires horaire × heures d'arrêt) avec une source citée | M | M |
| Les photos de banque d'images sont rejetées par ce public | Une séance photo en atelier chez 2 clients | H | M |

## 5. Erreurs à éviter

- Les photos de banque d'images (ouvrier souriant et tablette, usine bleutée).
- Des promesses absolues (« 100 % des pannes »).
- Un ROI tiré d'une étude commandée sans le dire.
- Le jargon IA, « jumeau numérique », « révolution 4.0 ».
- Une fiche technique derrière un long formulaire.
- Du jaune en texte sur blanc (environ 1,6:1).
- Une certification (ATEX, IP) affichée sans être obtenue.

## 6. Conclusion pour Vibra (fictif)

- **Angle** : « On pose le capteur, vous voyez la panne arriver. »
- **Le README est pertinent.** Ajustements recommandés :
  - Section 2 : un calculateur sourcé.
  - Section 3 : une durée pour chaque étape et la passerelle 4G.
  - Section 6 : des témoignages en HTML.
  - Un encart « Hébergement UE et compatibilité GMAO ».
- **Ton** : les fiches de Wormsensing et Tractian, en français, sans le vocabulaire IA d'Augury.
- **Conversion** : 3 CTA : « Tester sur une machine », « Appeler un technicien », « Télécharger la fiche technique ».
- **Budget** : la séance photo en atelier passe avant toute animation.

## 7. Questions à valider en recherche utilisateur

1. Un responsable maintenance préfère-t-il appeler, remplir un formulaire de pilote ou télécharger d'abord la fiche technique ?
2. La promesse « 3 semaines avant la panne » est-elle crédible, ou suscite-t-elle la méfiance sans périmètre précis ?
3. Quel format de témoignage convainc le plus : un pair du même secteur, un site proche géographiquement ou un chiffre d'arrêt évité ?
4. Le calculateur de coût d'arrêt est-il utilisé, ou jugé gadget ?
5. Quelles objections informatiques remontent en premier (réseau, cloud, cybersécurité) ?
6. L'abonnement par point de mesure est-il compris, ou faut-il afficher un prix indicatif ?
7. Sur le terrain (gants, tablette, bruit), le bouton d'appel et la fiche technique sont-ils accessibles en un geste ?

## 8. Notes de méthode

- **Sources** :
  - Environ 45 recherches web (novembre 2026), partagées entre les deux catégories.
  - Pages officielles indexées (wormsensing.com, icareweb.com, exotec.com, siemens.com, augury.com, tractian.com, sereact.ai).
  - Documents publics (PDF I-care, rapport Siemens TCOD 2024 non ouvert), presse et agrégateurs (Crunchbase News, synthèses PitchBook).
- **Limites** :
  - **Aucun visuel vu.** WebFetch est bloqué (ENOTFOUND), donc les rubriques première impression, hiérarchie, CTA et accessibilité sont des déductions ou sont marquées « non observé ». Le thème T5 (absence de téléphone) est notamment à confirmer visuellement.
  - Les chiffres d'entreprise sont auto-déclarés.
  - Les ROI cités sont issus d'études commandées.
  - Les chiffres ABB et Aberdeen ont été repris de synthèses secondaires.
  - Le budget de recherche web de la session a été épuisé avant d'avoir pu vérifier le nom « Vibra » (antériorités) et la taille du marché de la maintenance prédictive.
- **À faire avant présentation** : visiter les 6 sites (desktop et mobile), relever les CTA et la présence d'un numéro de téléphone, mesurer les contrastes, et compléter les rubriques « non observé ».
