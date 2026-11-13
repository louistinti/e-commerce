# Étude de cas : site vitrine industrie 4.0 / maintenance prédictive

> Document de travail de l'agence. **Vibra est une entreprise fictive.** Les entreprises analysées sont réelles. Leurs sites **n'ont pas pu être ouverts** (réseau de la session bloqué) : les critiques reposent sur les pages indexées, les documents publics (PDF, références) et la presse. Voir les notes de méthode en fin de document. **Mise à jour du 2026-11-12** : les pages citées ont depuis été ouvertes et capturées (voir les limites du [bench](BENCH.md)). Les erreurs factuelles relevées sont corrigées ci-dessous (I-care, Augury, Tractian, Sereact) ; le reste de l'analyse n'a pas été réécrit. **Passe du 2026-11-13** : chaque chiffre de marché et d'entreprise a été rouvert à sa source. Les chiffres sans source ouverte sont retirés, et quatre affirmations sont corrigées (Wormsensing, Exotec, Siemens, Augury).

## Executive summary

La robotique et la « physical AI » battent des records de financement (27,6 Md$ en 2025 selon PitchBook, voir section 1). La maintenance prédictive, elle, se vend sur un argument simple : le coût d'un arrêt non planifié. Les 6 sites étudiés convergent : hero « uptime », capture de tableau de bord, études de cas souvent en PDF, CTA « démo ». Aucun ne met le téléphone ni un essai sur machine au premier plan, alors que les PME achètent ainsi. Pour Vibra, l'opportunité est un site « fiche technique » : français, sans buzzword, avec des photos d'atelier, des témoignages nommés en HTML, et trois actions (tester, appeler, télécharger).

## 1. Le marché en 5 lignes

- **Records de financement robotique** : environ 27,6 Md$ levés sur 1 009 opérations en 2025 par les startups de la robotique et de la physical AI, selon [PitchBook, « Q4 2025 Robotics & Physical AI VC Trends », aperçu, p. 4](https://pitchbook.brightspotcdn.com/8b/51/2ba28f134d58b6bc6055b8f16c1e/q4-2025-robotics-physical-ai-vc-trends-preview.pdf), vu le 2026-11-13.
- **La « physical AI » s'accélère** : 47,4 Md$ sur 521 opérations au S1 2026, selon les données Crunchbase ([Crunchbase News](https://news.crunchbase.com/venture/physical-ai-funding-startups-robotics-aerospace-h1-2026/), vu le 2026-11-13).
- **L'arrêt coûte cher** : près de 1 400 Md$ par an pour les 500 plus grandes entreprises mondiales, soit 11 % de leur chiffre d'affaires. Une heure d'arrêt dans une grande usine coûte 36 000 $ dans les biens de grande consommation et 2,3 M$ dans l'automobile ([Siemens, *The True Cost of Downtime 2024*](https://assets.new.siemens.com/siemens/assets/api/uuid:1b43afb5-2d07-47f7-9eb7-893fe7d0bc59/TCOD-2024_original.pdf), PDF ouvert le 2026-11-13).
- **La filière française se structure et se consolide** :
  - Wormsensing (essaimage du CEA-Leti) a levé 9,5 M€ en série A ([Wormsensing](https://www.wormsensing.com/news/wormsensing-raises-9-5-million-series-a), vu le 2026-11-13).
  - I-care a racheté les actifs d'Amiral Technologies en septembre 2026 ([PR Newswire](https://www.prnewswire.com/fr/communiques-de-presse/i-care-group-acquiert-amiral-technologies-et-renforce-son-offre-de-maintenance-predictive-basee-sur-lia-notamment-dans-les-secteurs-du-nucleaire-et-de-la-defense-302881112.html), correctif du 18 septembre 2026, vu le 2026-11-13).
- **Pour une PME, l'argument est l'heure d'arrêt évitée.** Le chiffre Siemens porte sur de grandes usines : sur le site, il sert de repère, et le calculateur fait le reste avec les chiffres du visiteur.

Retirés lors de la passe du 2026-11-13, faute de source ouverte : le chiffre Crunchbase « 13,8 Md$ contre 7,8 Md$ » (absent de la synthèse citée), le « 8 % en 2019-2020 » (absent du rapport Siemens), les ordres de grandeur ABB et Aberdeen (sources primaires non ouvertes), et le « +185 % sur un an » qui figurait au README.

## 2. Critique de 6 sites réels

Grille utilisée : première impression (2 s), usabilité, hiérarchie visuelle, accessibilité, ce qui marche, recommandations. « Non observé » signifie qu'une visite visuelle est nécessaire.

### 2.1 Wormsensing (France, Grenoble), capteur piézoélectrique Dragonfly®
- **URL** : https://www.wormsensing.com/
- **Positionnement** : un capteur ultrafin (150 µm) et une plateforme, « Born in the Alps. Forged at CEA-Leti. » ([accueil](https://www.wormsensing.com/), vu le 2026-11-13).
- **Première impression** : non observée. Le titre de la home (« Dragonfly® piezoelectric vibration sensors ») annonce clairement l'objet, mais vise un lecteur technique.
- **Usabilité** : une navigation courte (Capteurs, Plateforme, cas d'usage, About, News), une gamme en 3 versions (Passive, IEPE, IO). Le CTA n'a pas été observé.
- **Hiérarchie** : les fiches sont denses en spécifications : connecteur M12 et IP67 pour la version IO, bande de 0,01 Hz à 100 kHz ([capteurs](https://www.wormsensing.com/sensors)), 150 °C maximum en exposition de 4 h pour la version IEPE ([IEPE](https://www.wormsensing.com/sensors/iepe)), vus le 2026-11-13.
- **Accessibilité** : non observée.
- **Ce qui marche** :
  - L'ancrage scientifique et territorial dès les titres.
  - Un livre blanc co-signé avec ifm (un industriel connu).
- **Recommandations** :
  1. Ajouter une entrée « responsable maintenance », sans unités de R&D (nε, µdef).
  2. Publier un témoignage d'usine nommé.
  - Correction du 2026-11-13 : la recommandation « proposer une version française » est retirée. Le site a un sélecteur de langue avec le français, et une page FR existe ([capteur de vibrations piézoélectrique](https://www.wormsensing.com/fr/capteur-de-vibrations-piezoelectrique)).

### 2.2 I-care (Belgique, présent en France), service de maintenance prédictive et capteur Wi-care
- **URL** : https://www.icareweb.com/ppc/wireless-vibration-sensor ; [étude de cas Barry Callebaut, Louviers](https://www.icareweb.com/knowledge/predictive-maintenance/success-story-barry-callebaut/) (le PDF cité auparavant renvoie une erreur 404 ; l'étude existe en HTML, en anglais)
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
- **Hiérarchie** : fiches techniques franches (capacité de 30 kg, jusqu'à 4 m/s, [robots](https://www.exotec.com/fr/solutions/robots/)) et preuves chiffrées et nommées (Renault Group à Villeroy : 167 robots, [cas client](https://www.exotec.com/fr/cas-clients/renault-group-une-logistique-plus-efficace-des-pieces-detachees-automobiles/)), vus le 2026-11-13. Correction : la version précédente donnait 191 robots.
- **Accessibilité** : la visite à 360° nécessite une alternative. Non vérifié.
- **Ce qui marche** : la preuve nommée, le découpage sectoriel et l'immersion maîtrisée.
- **Recommandations pour notre usage** : un ton grand compte à adapter, avec des actions plus courtes (essai, téléphone).

### 2.4 Siemens Senseye (Royaume-Uni / Allemagne), logiciel de maintenance prédictive
- **URL** : https://www.siemens.com/en-us/products/industrial-digitalization-services/senseye-predictive-maintenance/ ; [référence usine de Cham](https://references.siemens.com/en/reference/44824?id=44824)
- **Positionnement** : la maintenance prédictive « at scale », avec un copilote IA générative.
- **Première impression** : non observée. Le produit est inclus dans la navigation du groupe Siemens.
- **Usabilité** : une bibliothèque de références par site (Cham, Sachsenmilch, BlueScope). Le chemin vers le produit est long, car le site est celui d'un groupe.
- **Hiérarchie** : correction du 2026-11-13, le « jusqu'à −50 % d'arrêts non planifiés » est retiré. La référence de Cham n'affiche aucun pourcentage, seulement « Significant reduction » (vu le 2026-11-12, [bench](BENCH.md) n° 10), et la page produit renvoie une vérification anti-robots.
- **Accessibilité** : non observée.
- **Ce qui marche** : du contenu d'autorité (le rapport True Cost of Downtime) et des références nommées par usine.
- **Recommandations pour notre usage** : reprendre le format de la référence par site, pas l'architecture de groupe.

### 2.5 Augury (États-Unis / Israël), Machine Health : référence internationale
- **URL** : https://www.augury.com/ ; https://www.augury.com/machine-health/
- **Positionnement** : l'IA industrielle pour la disponibilité et la productivité.
- **Première impression** : vue le 2026-11-12. « Industrial AI for Uptime & Productivity » n'est que le titre d'onglet ; le hero affiche « Industrial AI Agents That Work for You. From Uptime to Unstoppable. », encore plus orienté IA.
- **Usabilité** : 2 produits (Machine Health, Process Health), des landing pages publicitaires et un gros blog SEO.
- **Hiérarchie** : la preuve chiffrée est mise en avant : ROI de 310 % selon une étude Forrester Total Economic Impact commandée ([Machine Health](https://www.augury.com/machine-health/), vu le 2026-11-13). Correction : le « −75 % de fausses alertes » cité auparavant n'apparaît ni sur l'accueil ni sur la page Machine Health ; il est retiré.
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
- **Hiérarchie** : spécifications de terrain en avant (IP69K, zones dangereuses, batterie de 3 à 5 ans, capteur en 4G/LTE sans Wi-Fi de l'usine). Vu le 2026-11-12 : la page ne mentionne ni passerelle ni « rapport initial en 5 jours », et la fiche technique est derrière un formulaire de 5 champs.
- **Accessibilité** : non observée.
- **Ce qui marche** :
  - Lever l'objection de la DSI (pas de réseau usine).
  - Une FAQ sur le temps d'installation.
- **Recommandations pour notre usage** : éviter les comparatifs « Top 5 » où l'auteur se classe premier. C'est efficace en SEO mais cela abîme la confiance.

Consulté en surface : Sereact (Allemagne, https://sereact.ai/product/pick-and-place), qui affiche ses chiffres de performance dans la 2e section de la page produit (8,000+ prises par jour, 600+ unités par heure en pointe, > 99 % de réussite).

## 3. Thèmes clés

### T1 : La promesse de disponibilité dans le hero
- **Prévalence** : 4 sites sur 6 (Augury « Uptime », Senseye « at scale », Tractian, I-care).
- **Observation** : les titres de pages tournent autour de l'uptime, de la prévention et de la disponibilité.
- **Interprétation** : la promesse est devenue générique. Il faut la rendre concrète : montrer l'alerte qui arrive avant la panne, sur une capture du logiciel.

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
- **Prévalence** : 0 sur 6. Vérifié le 2026-11-12 sur mobile pour Tractian, Wormsensing et I-care : aucun lien `tel:`, le CTA dominant est « démo » ou un contact.
- **Interprétation** : c'est l'opportunité la plus nette pour une PME qui vend à des PME.

### T6 : Lever l'objection informatique
- **Prévalence** : 1 sur 6 explicitement (Tractian, avec des capteurs en 4G/LTE qui n'utilisent pas le Wi-Fi de l'usine).
- **Interprétation** : les DSI bloquent souvent ces projets. Un encart d'architecture et d'hébergement UE est peu coûteux et lève le frein.

## 4. Insights → Opportunités

| Insight | Opportunité | Impact | Effort |
|---|---|---|---|
| Aucun site ne met le téléphone en avant | Barre « Appeler un technicien » fixe sur mobile, avec le nom et les horaires | H | B |
| « Démo » est le CTA par défaut | « Tester sur une machine » : pilote court avec un périmètre clair | H | M |
| Les études de cas sont souvent en PDF | 3 témoignages en HTML (nom, site, machine, défaut détecté), sans portrait | H | M |
| La promesse « uptime » est générique | Une promesse concrète : la tendance, l'alerte et l'intervention planifiée, montrées sur une capture | H | B |
| La fiche technique est déterminante | Fiche technique en un tap, sans formulaire, plus un résumé HTML | H | B |
| Le jargon IA est omniprésent | Ton factuel, vocabulaire de maintenancier (roulement, balourd, GMAO) | M | B |
| L'objection de la DSI est rarement traitée | Encart « 4G autonome, hébergement UE », plus une fiche sécurité | M | B |
| Le coût d'arrêt est le premier argument | Mini calculateur (chiffre d'affaires horaire × heures d'arrêt) avec une source citée | M | M |
| Les photos de banque d'images sont rejetées par ce public | Une séance photo en atelier cadrée sur le capteur, et un « Qui sommes-nous » sans photo | H | M |

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
  - Section 3 : 3 étapes dessinées au trait, et la passerelle 4G.
  - Section 6 : des témoignages en HTML, sans portrait.
  - Un encart « Hébergement UE et compatibilité GMAO ».
  - Un « Qui sommes-nous » court, sans photo, près du contact.
- **Ton** : les fiches de Wormsensing et Tractian, en français, sans le vocabulaire IA d'Augury.
- **Conversion** : 3 CTA : « Tester sur une machine », « Appeler un technicien », « Télécharger la fiche technique ».
- **Budget** : la séance photo en atelier passe avant toute animation.

## 7. Questions pour la recherche utilisateur

1. Un responsable maintenance préfère-t-il appeler, remplir un formulaire de pilote ou télécharger d'abord la fiche technique ?
2. La promesse « Zéro arrêt surprise » est-elle crédible sans délai chiffré, ou suscite-t-elle la méfiance ?
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
  - **Aucun visuel vu lors de la rédaction.** WebFetch était bloqué (ENOTFOUND), donc les rubriques première impression, hiérarchie, CTA et accessibilité sont des déductions ou sont marquées « non observé ». Le thème T5 (absence de téléphone) a été vérifié sur mobile le 2026-11-12.
  - Les chiffres d'entreprise sont auto-déclarés.
  - Les ROI cités sont issus d'études commandées.
  - Le nom « Vibra » sert uniquement à la démonstration : pas de recherche d'antériorité. La taille du marché de la maintenance prédictive n'est pas citée, faute de source ouverte.
- **Visites** : les sites ont été ouverts et capturés le 2026-11-12 (desktop et mobile), avec relevé des CTA, des liens `tel:` et des contrastes. Le détail est dans le [bench](BENCH.md) ; les rubriques « non observé » ci-dessus n'ont pas été réécrites.
