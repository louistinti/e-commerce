# Benchmark visuel : Vibra (entreprise fictive)

Ce bench suit le brief client bloc par bloc : chaque inspiration est rattachée à un bloc de l'arborescence (section 6 du brief) ou à une exigence transverse, et les autres références sont rangées à part.

## Limites, à lire en premier

Vérification du 2026-11-12, faite avec un vrai navigateur (Chrome piloté par Playwright).

- **Ce qui a été vu** : 14 des 19 références d'origine ont été ouvertes et capturées (n° 1 à 14). Pour le n° 2, la fiche Lapa Ninja est bloquée : c'est le site réel d'Intrepid Automation qui a été vu. Pour le n° 12, le PDF est mort : c'est la version HTML de la même étude de cas qui a été vue. Les captures sont en 1440 × 900 px, au-dessus de la ligne de flottaison, avec une seconde capture ciblée pour 3 éléments clés (n° 2, 7 et 11). Les couleurs et les polices citées ont été relevées dans la page (`getComputedStyle`). Les chiffres cités sont ceux affichés le 2026-11-12.
- **Ce qui reste bloqué** (5 références, marquées « non vérifié », rangées à côté) :
  - n° 15 et 16 (Behance) : « HTTP ERROR 400 » renvoyé au navigateur automatisé ;
  - n° 17 et 18 (Pinterest) : fenêtre de connexion sur toute la page, aucune URL d'épingle exposée ;
  - n° 19 (Lapa Ninja) : challenge Cloudflare, « Sorry, you have been blocked ». Le site réel de Vibor n'a pas été retrouvé.
- **Références ajoutées lors de la vérification** : 4 (n° 20 à 23, Dribbble et One Page Love). La partie mobile repose sur 3 sites réels vus en 390 × 844 px.
- **Corrections importantes** (faites lors de la vérification, toujours valables) :
  - n° 7, Tractian : la page ne parle ni de passerelle (c'est le capteur lui-même qui émet en 4G/LTE) ni de « rapport initial en 5 jours ». La fiche technique est **bloquée derrière un formulaire de 5 champs**, l'exact contre-exemple du brief.
  - n° 10, Siemens : il n'y a **aucun pourcentage** sur les arrêts non planifiés, seulement « Significant reduction ». Les seuls chiffres sont « plus de 90 machines » et « des coûts 3 à 5 fois plus élevés ».
  - n° 1, 2, 6, 14 : les phrases citées dans une version antérieure (« Industrial AI for Uptime & Productivity », « from signal to measured gains », « Born at CEA-Leti, made in Grenoble ») sont les **titres d'onglet**, pas les titres affichés. Le n° 2 n'a pas « weeks, not months » en titre de hero : c'est le titre de la 2e section.
  - n° 5 : ce n'est pas une illustration 3D ombrée, c'est un dessin au trait noir (rendu « Sketch and Toon » de Cinema 4D).
  - n° 9 : rien ne permet de dire que c'est « le shot le plus vu du tag ». Il n'y a ni score de santé ni courbe de tendance.
  - n° 11 : les chiffres de Sereact ne sont pas en tête de page, ils forment la 2e section.
  - Contraste du jaune : texte `#111418` sur `#FFC20E` = **11,4:1**, pas 13:1.
- **URL mortes ou redirigées** : n° 12, le PDF I-care renvoie une erreur 404 (avec ou sans le double `.pdf`). n° 10, l'URL redirige vers `references.siemens.com/en/reference/siemens-cham?id=44824`. n° 2, `intrepidautomation.com` redirige vers `www.`.
- **Bannières cookies** : refusées partout où un refus existait (« Reject all », « Tout rejeter », « Deny »). Sur Augury, refus par « Use necessary cookies only ». Les fenêtres promotionnelles (webinaire Augury, visite d'usine Tractian) ont été fermées.
- **Données personnelles** : les avatars des auteurs Dribbble et One Page Love sont floutés sur les captures. Aucun formulaire n'a été rempli.
- **Refonte du 2026-11-12 (tri selon le brief)** :
  - Les 23 références sont triées : **10 inspirations** (n° 4, 5, 6, 7, 9, 11, 12, 14, 20, 22) et **13 à côté** (n° 1, 2, 3, 8, 10, 13, 15 à 19, 21, 23). Rien n'est supprimé : chaque référence à côté garde sa ligne et sa raison.
  - Les captures sont rangées dans [`captures/inspis/`](captures/inspis/) et [`captures/a-cote/`](captures/a-cote/), sans renommage. Les captures mobiles suivent le même tri, chacune selon ce qu'elle montre : Wormsensing en inspiration, Tractian et I-care à côté (contre-exemples sur l'appel et les chiffres).
  - Le bench est réorganisé par bloc du brief. Les numéros ne changent pas.
  - Aucune nouvelle référence : chaque bloc a au moins une inspiration. Les manques à l'intérieur des blocs (calculateur, formulaire court, tableau de bord annoté) sont signalés dans la couverture.
  - La direction B « Atelier de nuit » est retirée (raison dans « Directions »). La direction C est gardée avec une correction typographique.
  - Tokens corrigés pour suivre le brief : `type.h3` passe en Barlow Condensed (le brief réserve Barlow Condensed aux titres) ; `type.data` passe d'IBM Plex Mono à Barlow en chiffres tabulaires (le brief fixe deux familles) ; ajout de `color.focus-inverse` `#FFFFFF`, car l'anneau `#1F6FEB` sur le pied de page `#2B3036` ne fait que 2,87:1 (WCAG demande 3:1) ; ajout d'un `scroll-padding-bottom` sous la barre d'appel fixe (WCAG 2.2, critère 2.4.11, focus non masqué). Tous les autres contrastes ont été recalculés et sont conformes.

- **Passe du 2026-11-13 (aucun client, aucun chiffre inventé)** :
  - Les questions ouvertes de fin de bench deviennent des **Arbitrages** (fin du document) : chaque question reçoit une décision.
  - Les chiffres propres à Vibra (anticipation « 19 jours », « 34 défauts », « 20 pilotes ») sont retirés. Les chiffres relevés sur les pages du bench restent, avec leur URL.
  - Le coût d'un arrêt a maintenant sa source ouverte : le rapport Siemens *The True Cost of Downtime 2024* (PDF ouvert le 2026-11-13).
  - Photos d'équipe : Unsplash (« Access Denied ») et Pexels (vérification Cloudflare) bloquent le navigateur automatisé. On n'a rien contourné : le site aura un « Qui sommes-nous » court, sans photo, et les exigences de photo réelle d'équipe sont retirées du bench.

Répartition : sites réels 10 · Awwwards 1 · Dribbble 6 · One Page Love 2 · Behance 2 (non vérifiés) · Pinterest 2 (non vérifiés) · Lapa Ninja 1 (non vérifié). **Total : 23, dont 18 vus. Inspirations : 10. À côté : 13.**

---

## Couverture du brief

| Exigence du brief | Inspirations | Manque |
|---|---|---|
| 1. Hero (photo d'atelier serrée sur le capteur, « Zéro arrêt surprise », 2 CTA) | 6, 4, 20 | Aucun hero vu n'est à la fois clair, cadré sur un capteur posé et doté d'un bouton d'appel. Le n° 6 a le bon cadrage mais un fond `#06060F`. |
| 2. Le coût d'un arrêt (grand chiffre sourcé, calculateur à 2 champs) | 11, 12 | Aucun calculateur vu. La source du chiffre est le rapport Siemens TCOD 2024, ouvert le 2026-11-13 (voir « Arbitrages »). |
| 3. Installation en 3 étapes (3 dessins au trait, sans durée) | 5, 7 | Aucune référence ne montre 3 étapes de pose d'un capteur. Les dessins sont à produire dans le style du n° 5. |
| 4. Ce que voit le responsable maintenance (capture annotée : score, tendance, alerte avec action) | 9 | Ni score de santé, ni courbe de tendance, ni annotation en 3 points sur les références vues. La phrase d'Augury (n° 1, à côté) donne le texte de l'alerte. |
| 5. Secteurs (agroalimentaire, plasturgie, métallurgie : machines et défaut typiques) | 22 | Aucune référence n'associe un secteur, ses machines et son défaut. Le trait épais du n° 8 (à côté) peut servir aux pictos. |
| 6. Retours d'usine (3 témoignages : nom, fonction, site, machine, sans portrait) | 12 | Seulement des études longues : aucune grille de 3 cartes courtes vue. |
| 7. Fiche technique (PDF sans formulaire, résumé HTML) | 7 | Aucun site vu ne propose le PDF sans formulaire (le n° 7 est le contre-exemple). |
| 8. Qui sommes-nous, contact et pilote (« Qui sommes-nous » sans photo, formulaire court, numéro direct, technicien par région) | 22, 14 | Aucun formulaire court vu. |
| Mobile : appel fixe en 1 tap, fiche technique en 1 tap | 6 (mobile) | Aucun des 3 sites vus en 390 px n'a de lien `tel:`. |
| Marque : gris acier, blanc, jaune en accent, Barlow Condensed et Barlow | 20, 4 | Aucune référence en Barlow, aucune en gris acier et jaune. Le n° 20 montre la condensée noire et le jaune, mais en trop grande dose. |
| Photos d'atelier, aucune banque d'images (critère de réussite) | 6, 12, 4 | Le n° 10 (à côté) montre le défaut à éviter. |
| Accessibilité : contrastes AA, cibles de 48 px, statut jamais par la couleur seule | 6 (mobile), 7 | Aucun tableau de bord vu ne double la couleur d'une icône et d'un libellé. |
| Preuve « Zéro arrêt surprise » : tendance, alerte et intervention planifiée sur une capture | 9, 11 | Aucune référence ne montre la tendance qui précède l'alerte. Pas de délai d'anticipation chiffré : Vibra n'a pas de mesure. |
| Preuve « Vos données restent en Europe et hors de votre réseau » (schéma pour P3) | 6, 7 | Aucune référence ne montre l'hébergement UE ni une fiche sécurité téléchargeable. |

Les autres preuves de la section « Messages clés » sont couvertes par leur bloc : installation (bloc 3), alerte (bloc 4), témoignages (bloc 6), coût d'un arrêt (bloc 2).

---

## Inspirations, bloc par bloc

### 1. Hero

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 6 | Wormsensing : Plateforme, https://www.wormsensing.com/platform (site réel, FR) | [capture](captures/inspis/06-wormsensing-platform.jpg) | **La référence la plus proche du hero voulu** : photo serrée, réelle, du capteur Dragonfly collé sur un carter, avec sa plaque signalétique et son câble. On reprend le cadrage seulement. À éviter : le fond `#06060F`, les capitales espacées et les boutons à contour, signature d'un fabricant de capteurs existant. | « Une photo d'atelier réelle avec un cadrage serré sur le capteur posé » ; P1 veut « une vraie photo de capteur posé sur un moteur » ; ne pas imiter la signalétique d'un fabricant. |
| 4 | Path Robotics, https://www.awwwards.com/sites/path-robotics (Awwwards, site du jour le 23 septembre 2021, 7,34/10) | [capture](captures/inspis/04-awwwards-path-robotics.jpg) | Cellule de soudage photographiée seule, titre géant et **grille de colonnes visible** (filets verticaux qui découpent l'en-tête et l'image). On reprend la machine seule et la grille, en version claire. À noter : la fiche montre la version primée (fond `#000`), le site actuel a changé (« Physical AI for Manufacturing », `#151515`). | Hero en photo réelle de machine ; registre « document de travail » pour des acheteurs qui se méfient du marketing. |
| 20 | Sterial (Pxcraftt), https://dribbble.com/shots/27613985-Worker-in-Hazmat-Suit-Spraying-Disinfectant-Website-Design (Dribbble) | [capture](captures/inspis/20-dribbble-pxcraftt-disinfection.jpg) | Titre en capitales condensées très grasses, noir sur blanc, dernier mot surligné de jaune ; **téléphone et bouton jaune à texte noir dans l'en-tête**. À éviter : la moitié de page en aplat jaune et les hachures noir et jaune (code chantier). | Titre « Zéro arrêt surprise » en Barlow Condensed ; CTA secondaire « Appeler un technicien » visible dès l'arrivée ; jaune en fond de bouton avec texte foncé. |

Renvois à côté : la rangée de logos clients sous le hero du n° 3 n'est pas reprise, car Vibra est fictive et des logos réels laisseraient croire à des clients. La formule « en semaines, pas en mois » du n° 2 n'est pas reprise non plus : Vibra n'a pas de délai mesuré à promettre.

### 2. Le coût d'un arrêt

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 11 | Sereact : Pick and Place, https://sereact.ai/product/pick-and-place (site réel, DE) | [hero](captures/inspis/11-sereact-pick-and-place.jpg), [KPI](captures/inspis/11-sereact-kpis.jpg) | Section « Key Production KPIs » : 8,000+ prises par jour, 600+ unités par heure en pointe, > 99 % de prises réussies. Chaque chiffre a une étiquette en petites capitales (monospace 12 px bleu `#0284C7`), un grand chiffre (Montserrat 300, 60 px) et une phrase de contexte (« When your system can feed fast enough. »). On reprend la structure : étiquette, grand chiffre, phrase de périmètre, filets fins. Étiquette en Barlow Condensed, pas en monospace. | « Un grand chiffre sourcé » ; règle « chaque chiffre a un périmètre ». |
| 12 | I-care : Barry Callebaut, https://www.icareweb.com/knowledge/predictive-maintenance/success-story-barry-callebaut/ (site réel, BE) | [capture](captures/inspis/12-icare-barry-callebaut.jpg) | Le chiffre d'arrêt évité mis en regard du coût horaire : 30 h d'arrêt évitées sur les broyeurs, 1 h d'arrêt = 5 000 $. C'est exactement le calcul que fait le calculateur. | Calculateur (chiffre d'affaires horaire × heures d'arrêt) ; P2 veut « le chiffre du coût d'arrêt ». |

### 3. Installation en 3 étapes

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 5 | Sensor installation (Franco Bertoncini Andrade, pour Nordsense), https://dribbble.com/shots/8762795-Sensor-installation (Dribbble) | [capture](captures/inspis/05-dribbble-sensor-installation.jpg) | Illustration de notice d'installation : dessin isométrique au trait noir sur blanc, une pièce, ses vis en vue éclatée, un seul aplat de couleur (vert `#BFDCBF`, à remplacer par le jaune ou le gris acier). Un objet, le geste, aucun décor. | « 3 étapes illustrées » ; style retenu pour les 3 dessins (voir « Arbitrages »). |
| 7 | Tractian : Condition Monitoring, https://tractian.com/en/solutions/condition-monitoring (site réel, US) | [capture](captures/inspis/07-tractian-condition-monitoring.jpg) | La FAQ « combien de temps pour installer ? » et la promesse « No IT setup, no Wi-Fi needed ». | Message « Installé sans câble, sans arrêter la ligne » ; frein de P1 « encore un outil à surveiller ». |

### 4. Ce que voit le responsable maintenance

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 9 | Preventive Maintenance Dashboard (Jagath Selvan), https://dribbble.com/shots/9109597-Preventive-Maintenance-Dashboard (Dribbble) | [capture](captures/inspis/09-dribbble-maintenance-dashboard.jpg) | Une grille « une carte = une machine » avec 4 valeurs et leur unité, des compteurs par type d'alerte en tête, l'horodatage « Last Updated ». À éviter : l'alerte signalée surtout par la couleur rouge, et la vibration en « hz » au lieu de mm/s. Il manque le score de santé et la tendance, à ajouter sur la capture de Vibra. | « Une alerte = une machine, un défaut, une action » ; capture annotée en 3 points ; statuts doublés d'une icône et d'un libellé (WCAG). |

Renvoi à côté : la phrase d'Augury (n° 1) « Predictive intelligence alerts your team to exactly what's failing, how urgent it is, and what to do » donne l'ordre des 3 annotations : quelle machine, quelle urgence, quelle action.

### 5. Secteurs

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 22 | Plastics Unlimited (Nerdwerx), https://onepagelove.com/plastics-unlimited (One Page Love, publié le 15 février 2016, site hors ligne) | [capture](captures/inspis/22-onepagelove-plastics-unlimited.jpg) | « Capabilities » en accordéon : un intitulé en capitales par savoir-faire, un « + » pour déplier. Pour Vibra : un accordéon par secteur, avec ses machines typiques et son défaut typique. À éviter : les aplats rouge et bleu saturés. | « Pour chacun : les machines typiques et le défaut typique » ; P2 cherche « des références dans son secteur ». |

Renvoi à côté : le trait épais des icônes du n° 8, lisible en petit, pour des pictos qui montrent les vrais objets (moteur, pompe, extrudeuse, broyeur).

### 6. Retours d'usine

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 12 | I-care : Barry Callebaut (Louviers), même URL qu'au bloc 2 | [capture](captures/inspis/12-icare-barry-callebaut.jpg) | Photo réelle d'un opérateur sur la ligne, site nommé, secteur et taille en icônes, citation du responsable fiabilité, puis « Challenges », « Solutions », « Benefits ». Faits : site de 350 salariés, environ 4 000 équipements, moteur suivi jusqu'à l'arrêt programmé. À éviter : les chiffres enfouis en fin de page et le bouton orange `#F7941D` à texte blanc (2,3:1). Sur la carte Vibra, la machine et le défaut détecté remontent en tête, sans portrait et sans chiffre de résultat. | « 3 témoignages avec nom, fonction, site et machine » ; P2 veut « un témoignage d'une usine comparable avec le nom du site » ; CTA « Lire le retour complet ». |

Renvoi à côté : la page Siemens (n° 10) confirme la structure en 3 rubriques (objectifs, solution, bénéfices) et le site nommé, mais sans chiffre et avec une photo d'ambiance.

### 7. Fiche technique

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 7 | Tractian : Condition Monitoring (même URL qu'au bloc 3) | [spécifications](captures/inspis/07-tractian-specs.jpg) | Bloc « Technical Specifications » : 6 tuiles avec icône (batterie 3 à 5 ans, -40 °F à 250 °F, Class 1 Div 1 ATEX/IECEx, IP69K, 4G/LTE, échantillonnage jusqu'à 64 kHz). Chaque certification est nommée avec sa classe. À éviter : « Download Spec Sheet » ouvre un formulaire de 5 champs (nom, e-mail pro, téléphone, fonction, secteur), et le fond `#1E293B` du bloc. | Résumé HTML (IP, autonomie, plage de fréquence, température, certification) ; certification citée seulement si obtenue, avec sa référence ; PDF **sans** formulaire (contre-exemple). |

Renvoi à côté : la description du n° 21 pose le même problème que ce bloc, éviter de faire « soit une fiche technique, soit un site vague ». Le résumé HTML sert la directrice, le PDF sert le maintenancier et l'informaticien.

### 8. Qui sommes-nous, contact et pilote

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 22 | Plastics Unlimited (même fiche qu'au bloc 5) | [capture](captures/inspis/22-onepagelove-plastics-unlimited.jpg) | Bandeau noir fixe avec **le numéro de téléphone en premier**, et « Sales representatives as well as technical advisors are available ». One Page Love signale une galerie d'équipe avec e-mail et poste téléphonique ; Vibra garde les noms et les numéros, sans portrait. | « Numéro direct, nom du technicien par région » ; P1 attend « un interlocuteur technique joignable ». |
| 14 | Wormsensing : About us, https://www.wormsensing.com/about-us (site réel, FR) | [capture](captures/inspis/14-wormsensing-about.jpg) | L'ancrage territorial en une ligne (« Engineered in Grenoble », fondée en 2020 par deux ingénieurs de recherche du CEA). Pour Vibra : Saint-Étienne et les techniciens par région, dans un « Qui sommes-nous » de 3 phrases, sans photo. On ne reprend pas la photo aérienne de ville. | Bloc « Qui sommes-nous » ; campagne régionale (Auvergne-Rhône-Alpes, Grand Est) et requêtes SEO régionales ; nom du technicien par région. |

### Exigences transverses

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 6 | Wormsensing : Plateforme | [capture](captures/inspis/06-wormsensing-platform.jpg) | La chaîne en 5 verbes (Sense, Connect, Acquire, Interpret, Decide) avec des chiffres d'unité (10 µm, 150 µm, 100 kHz, 1000×). Pour Vibra : capteur, passerelle 4G, hébergement UE, alerte. À éviter : les gains en fourchettes sans périmètre (« Up to 280% », « −50 to −99% »). | Schéma d'architecture pour P3 ; preuve « Vos données restent en Europe et hors de votre réseau ». |
| 7 | Tractian | [capture](captures/inspis/07-tractian-condition-monitoring.jpg) | « No IT setup, no Wi-Fi needed » : l'argument « rien sur le réseau usine » dit en une ligne. Boutons bleu `#2563EB` à texte blanc (5,2:1), rayon de 2 px. | P3 veut lire « aucune connexion au réseau usine » ; contrastes AA. |
| 11 | Sereact | [KPI](captures/inspis/11-sereact-kpis.jpg) | La phrase de contexte sous chaque chiffre. | Le chiffre de référence du bloc 2 (Siemens TCOD 2024) avec sa phrase de périmètre : « grande usine de biens de grande consommation ». |
| 20 | Sterial | [capture](captures/inspis/20-dribbble-pxcraftt-disinfection.jpg) | La condensée noire en grand et le jaune en surlignage ou en fond de bouton seulement. | Marque : Barlow Condensed, jaune jamais en texte sur blanc. |

---

## Mobile

Trois sites vus en 390 × 844 px le 2026-11-12. Le brief demande un bouton « Appeler un technicien » fixe sur mobile, la fiche technique en 1 tap, des cibles de 48 px et un test « appeler et trouver la fiche en moins de 10 s ».

| Site | Capture | Ce qu'on observe | Exigence du brief |
|---|---|---|---|
| Wormsensing : Plateforme (n° 6, inspiration) | [capture](captures/inspis/mobile-wormsensing.jpg) | La photo est recadrée sur le capteur, qui reste lisible au-dessus du titre. Les 2 boutons passent l'un sous l'autre en pleine largeur, 48 px de haut. En-tête fixe réduit à « Menu ». Aucun lien `tel:`. | Hero cadré sur le capteur posé ; cibles de 48 px. |
| Tractian : Condition Monitoring (n° 7, à côté en mobile) | [capture](captures/a-cote/mobile-tractian.jpg) | Le texte passe au-dessus de la photo, les 2 boutons « See Pricing » et « Book a Demo » restent côte à côte. Seule la barre de navigation est collante. « Contact us », visible avec une icône de téléphone sur desktop, disparaît dans le menu burger. Aucun lien `tel:`. | Contre-exemple : l'appel ne doit jamais passer dans le menu. |
| I-care : Barry Callebaut (n° 12, à côté en mobile) | [capture](captures/a-cote/mobile-icare.jpg) | La photo passe au-dessus du titre, puis secteur et taille en icônes. Le seul élément fixe est une bulle de chat orange en bas à droite (plus le bouton de consentement). Aucun lien `tel:` ; les chiffres clés (30 h, 5 000 $ de l'heure) sont tout en bas de la page. | Contre-exemple : l'information clé d'un témoignage (machine, défaut) doit être en tête de carte. |

Ce que ces observations donnent pour Vibra :
- **aucun des 3 sites ne propose d'appel en 1 tap**. La barre fixe « Appeler un technicien » avec un vrai lien `tel:` est un point de différence. Elle ne se cache jamais dans le menu. Parmi les sites réels vus, seul Plastics Unlimited (n° 22, desktop, 2016) mettait le téléphone en premier ;
- recadrer la photo du hero sur le capteur posé, comme Wormsensing, pour qu'il reste visible en 390 px ;
- boutons empilés en pleine largeur, 48 px minimum (Wormsensing est exactement à 48 px) ;
- la machine et le défaut d'un témoignage remontent en tête de carte, au lieu d'être en fin d'article comme chez I-care ;
- la fiche technique en 1 tap, sans formulaire : c'est l'inverse de Tractian (n° 7).

---

## Directions

Constat du panel : les heros du secteur sont sombres (Augury, Intrepid, Path Robotics, Wormsensing, Sereact, Siemens). Seuls Tractian et I-care ont un hero clair. Aucun site vu ne propose d'appel en 1 tap, et Tractian bloque sa fiche technique. Les trois actions de Vibra (tester, appeler, télécharger sans formulaire) sont donc des arguments de différence. Le brief ne fixe pas de nombre de pistes : deux directions restent.

**Direction A : « Fiche technique »** (recommandée)
- Fond blanc et gris acier, grille visible, grands chiffres en Barlow Condensed, photos serrées sur le capteur posé.
- Le jaune est réservé au CTA et aux repères d'étapes.
- Rassure le maintenancier : on dirait un document de travail, pas une pub.
- Inspirations : n° 6 (cadrage du hero), n° 4 (grille visible, machine seule), n° 20 (condensée noire, téléphone dans l'en-tête), n° 11 (chiffres et étiquettes), n° 7 (bloc de spécifications), n° 5 (dessin au trait pour les étapes), n° 9 (cartes machine).

**Direction C : « Carnet de terrain »**
- Photos documentaires du capteur et des gestes d'installation, légendes courtes, témoignages en avant.
- Correction : les légendes sont en Barlow Condensed (`type.label`), pas en écriture manuscrite ni en monospace, car le brief fixe deux familles.
- Très crédible, mais dépend entièrement de la séance photo (prévue au brief, S3). Pas de portraits d'équipe : le « Qui sommes-nous » reste sans photo.
- Inspirations : n° 12 (photo réelle d'opérateur, citation nommée), n° 22 (interlocuteurs nommés), n° 14 (ancrage territorial), n° 6 en mobile (photo recadrée sur le capteur).

**Direction B « Atelier de nuit » : retirée.** Elle mettait un fond graphite et le jaune en bandes de balisage, ce qui sort du trio « gris acier, blanc, jaune » du brief et pousse vers la signalétique de chantier ; elle visait aussi « l'impact au salon », alors que le brief dit que les acheteurs se méfient du marketing.

---

## Palette, polices, design tokens, composants

Chaque valeur a été vérifiée le 2026-11-12 contre les contraintes du brief (gris acier, blanc, jaune sécurité ; Barlow Condensed et Barlow ; pas de jaune en texte sur blanc ; WCAG 2.2 AA ; cibles de 48 px). Contrastes calculés avec la formule WCAG.

### Palette recommandée

| Rôle | Hex | Note |
|---|---|---|
| Acier foncé (titres, pied de page) | `#2B3036` | 13,3:1 sur blanc |
| Acier | `#4A525B` | texte secondaire : 7,9:1 sur blanc, 6,8:1 sur `#ECEEF0` |
| Gris moyen (filets) | `#8A939C` | décor uniquement, pas de texte |
| Gris clair (fonds de section) | `#ECEEF0` | |
| Blanc | `#FFFFFF` | |
| Jaune sécurité | `#FFC20E` | proche des RAL 1003 et 1023 (valeur RVB indicative). **Fond de bouton avec texte `#111418`** (11,4:1) ; **jamais en texte sur blanc** (1,6:1) |

### Polices (Google Fonts)

- **Barlow Condensed** : 600 et 700 pour tous les titres, les chiffres-clés et les étiquettes.
- **Barlow** : 400 et 500 pour le texte, 600 pour les boutons. Les valeurs de capteurs (mm/s, °C) sont en Barlow 500 avec chiffres tabulaires (`font-variant-numeric: tabular-nums`).
- **Correction** : l'option IBM Plex Mono est retirée, car le brief fixe deux familles. Les étiquettes monospace vues chez Sereact (n° 11) et Sterial (n° 20) sont reprises en Barlow Condensed en capitales.

### 3 « à ne pas faire »

1. Pas de photo de banque d'images (ouvrier souriant avec tablette, usine teintée en bleu) : le brief l'exclut, et ce public la repère immédiatement.
2. Pas de jaune en aplat sur toute la page ni de rayures noir et jaune partout : on bascule dans le code BTP et signalétique (voir n° 20).
3. Pas de vocabulaire IA ni de tableau de bord « futuriste » (néon, 3D) : le brief interdit le jargon IA, et la capture doit ressembler au vrai logiciel.

### Couleurs

| Token | Hex | Usage |
|---|---|---|
| `color.brand.primary` | `#FFC20E` | fond du CTA principal, repères d'étapes |
| `color.brand.primary-hover` | `#E5AC00` | survol du CTA (texte `#111418` : 9,0:1) |
| `color.brand.ink` | `#111418` | texte sur jaune, titres |
| `color.neutral.900` | `#2B3036` | titres, pied de page |
| `color.neutral.700` | `#4A525B` | texte courant secondaire |
| `color.neutral.400` | `#8A939C` | filets, icônes inactives |
| `color.neutral.100` | `#ECEEF0` | fonds de section |
| `color.neutral.0` | `#FFFFFF` | fond principal |
| `color.semantic.success` | `#1E7F4F` | machine OK, envoi réussi (texte blanc, 5,0:1) |
| `color.semantic.warning` | `#B45309` | dégradation à surveiller (5,0:1 sur blanc ; le jaune de marque n'est pas utilisé pour l'alerte, pour éviter la confusion) |
| `color.semantic.error` | `#C62828` | défaut critique, erreur de formulaire (5,6:1 sur blanc) |
| `color.focus` | `#1F6FEB` | anneau de focus clavier sur fonds clairs (4,6:1 sur blanc, 4,0:1 sur `#ECEEF0`), distinct du jaune |
| `color.focus-inverse` | `#FFFFFF` | **ajouté** : anneau de focus sur fonds foncés (pied de page, barre d'appel). `#1F6FEB` sur `#2B3036` ne fait que 2,87:1 ; le blanc fait 13,3:1 |

Les statuts sont toujours doublés d'une icône et d'un libellé, jamais signalés par la couleur seule.

### Typographie

| Token | Police | Taille (desktop / mobile) | Graisse | Interlignage |
|---|---|---|---|---|
| `type.display` | Barlow Condensed | 72 / 44 px | 700 | 1,0 |
| `type.h1` | Barlow Condensed | 48 / 34 px | 700 | 1,05 |
| `type.h2` | Barlow Condensed | 36 / 28 px | 600 | 1,1 |
| `type.h3` | Barlow Condensed (**corrigé**, était Barlow) | 24 / 22 px | 600 | 1,2 |
| `type.body` | Barlow | 18 / 17 px | 400 | 1,55 |
| `type.small` | Barlow | 15 / 15 px | 500 | 1,45 |
| `type.label` | Barlow Condensed | 14 px, majuscules, interlettrage 0,04 em | 600 | 1,2 |
| `type.data` | Barlow (**corrigé**, était IBM Plex Mono), chiffres tabulaires | 16 px | 500 | 1,4 |

`type.h3` passe de 22 / 20 px à 24 / 22 px pour compenser la chasse plus étroite de la condensée.

### Espacement (base 4 px)

`space.1` 4 · `space.2` 8 · `space.3` 12 · `space.4` 16 · `space.6` 24 · `space.8` 32 · `space.12` 48 · `space.16` 64 · `space.24` 96 (marge verticale entre sections sur desktop ; 64 sur mobile).

### Rayons

`radius.none` 0 (photos, sections) · `radius.sm` 2 px (boutons, champs) · `radius.md` 4 px (cartes). Des angles presque vifs, pour un registre industriel.

### Ombres

`shadow.none` par défaut (on préfère les filets) · `shadow.sm` `0 1px 2px rgba(17,20,24,.08)` pour les cartes au survol · `shadow.sticky` `0 -2px 8px rgba(17,20,24,.12)` pour la barre d'appel fixe sur mobile.

### Motion

| Token | Valeur | Usage |
|---|---|---|
| `motion.duration.fast` | 120 ms | survol, focus |
| `motion.duration.base` | 200 ms | ouverture d'accordéon, changement d'onglet |
| `motion.duration.slow` | 400 ms | apparition des 3 étapes au défilement (une fois) |
| `motion.easing.standard` | `cubic-bezier(.2,0,0,1)` | |
| `motion.easing.exit` | `cubic-bezier(.4,0,1,1)` | |

`prefers-reduced-motion` : toutes les durées passent à 0, sans apparition au défilement.

### Composants clés

**Bouton primaire** (« Tester sur une machine »)
- Fond `brand.primary`, texte `brand.ink`, Barlow 600 en 17 px, hauteur 48 px minimum, `radius.sm`.
- États :
  - survol : `primary-hover` ;
  - focus : anneau `color.focus` de 3 px, décalé de 2 px (`color.focus-inverse` sur fond foncé) ;
  - actif : enfoncé de 1 px ;
  - désactivé : `neutral.100` avec texte `neutral.400` et `aria-disabled` ;
  - chargement : spinner avec le libellé « Envoi… ».

**Bouton secondaire** (« Appeler un technicien », « Télécharger la fiche technique (PDF, 2 pages) »)
- Contour de 2 px `neutral.900`, texte `neutral.900`, fond transparent.
- États :
  - survol : fond `neutral.100` ;
  - focus : identique au primaire ;
  - désactivé : contour `neutral.400`.
- Sur mobile, « Appeler » devient une barre fixe en bas d'écran (`tel:`), 48 px minimum.
- **Ajouté** : la page reçoit un `scroll-padding-bottom` égal à la hauteur de la barre, pour qu'un élément qui reçoit le focus ne passe jamais dessous (WCAG 2.2, critère 2.4.11).

**Carte témoignage**
- Sans portrait. En tête, la machine et le défaut détecté (`type.h2`), puis la citation en Barlow 500 au corps `type.body` (**corrigé** : une citation est du texte, pas un titre), puis nom, fonction, site et ville en `type.small`.
- Une mention « Témoignage fictif (démonstration) » en `type.label`.
- Filet `neutral.100` et `radius.md`.

**Formulaire pilote**
- 5 champs maximum (nom, société, site, nombre de machines, téléphone), un libellé au-dessus de chaque champ (jamais seulement un placeholder), champs de 48 px de haut.
- Erreurs sous le champ en `semantic.error` avec une icône, et `aria-describedby`.
- Le téléphone est obligatoire, l'e-mail facultatif.

### À faire / À ne pas faire

| À faire | À ne pas faire |
|---|---|
| Jaune en fond de bouton avec texte foncé | Jaune en texte ou en icône sur fond blanc |
| Statuts couleur, plus icône, plus libellé | Statut indiqué seulement par du rouge ou du vert |
| Photos réelles, cadrage serré sur la machine | Images de banque ou rendus 3D génériques d'usine |
| Un seul CTA primaire par écran | Trois boutons jaunes côte à côte |
| Cibles tactiles de 48 px minimum (usage avec des gants) | Liens texte de 14 px comme seul moyen d'action |
| Fiche technique téléchargeable sans formulaire | Fiche technique bloquée derrière un formulaire (5 champs chez Tractian, n° 7) |
| Chiffres avec unité, périmètre et source (« 30 h d'arrêt évitées sur les broyeurs », I-care, n° 12) | « Jusqu'à 100 % de pannes évitées » |

---

## À côté

| # | Référence | Capture | Pourquoi à côté |
|---|---|---|---|
| 1 | Augury : accueil, https://www.augury.com/ (site réel, US) | [capture](captures/a-cote/01-augury.jpg) | Le titre affiché parle d'« Industrial AI Agents » : le brief interdit le jargon IA. Bouton orange `#EB7633` à texte blanc à 2,9:1 (WCAG AA non atteint), fenêtre de webinaire à l'arrivée, photo d'usine sous voile bleu nuit. Seul détail utile, la phrase sur l'alerte, cité au bloc 4. |
| 2 | Intrepid Automation, https://www.intrepidautomation.com/ (vu à la place de la fiche Lapa Ninja, bloquée) | [hero](captures/a-cote/02-intrepid-automation.jpg), [section « weeks »](captures/a-cote/02-intrepid-automation-weeks.jpg) | Hero quasi noir en rendu 3D de 4 machines : le brief demande une photo d'atelier réelle. Seule la formule « Manufacturing measured in weeks, not months » (2e section) est utile, citée au bloc 1. |
| 3 | Manufacturing Business Website Landing Page (Modall), https://dribbble.com/shots/24381180-Manufacturing-Business-Website-Landing-Page | [capture](captures/a-cote/03-dribbble-modall.jpg) | Hero en photo d'équipe sous un filtre bleu uniforme : c'est l'« usine teintée en bleu » à proscrire, et le brief veut un cadrage serré sur le capteur. Seule la rangée de logos clients est utile, citée au bloc 1. |
| 8 | Industrial Internet of Things, icônes (Katie Collins), https://dribbble.com/shots/22710707-Industrial-Internet-of-Things-IIoT-icons | [capture](captures/a-cote/08-dribbble-iiot-icons.jpg) | Répertoire générique (engrenages, globe, nuage « IIoT », bras robot), aucun capteur ni moteur, monochrome bleu hors de la palette du brief. Seul le trait épais est utile, cité au bloc 5. |
| 10 | Siemens Senseye : usine de Cham, https://references.siemens.com/en/reference/44824?id=44824 | [capture](captures/a-cote/10-siemens-senseye-cham.jpg) | Photo de banque d'images (bokeh) : le brief exige « aucune photo de banque d'images ». Résultat sans chiffre (« Significant reduction ») : le brief veut un chiffre avec périmètre. Référence interne (Siemens chez Siemens). Structure en 3 rubriques citée au bloc 6. |
| 13 | Exotec : Ressources, https://www.exotec.com/fr/ressources/ | [capture](captures/a-cote/13-exotec-ressources.jpg) | Contexte sectoriel seulement : aucun bloc du brief ne prévoit de page ressources ni de visite à 360°. Boutons turquoise `#28AFB9` à texte blanc (2,7:1, WCAG AA non atteint). La visite à 360° reste une idée de phase 2. |
| 15 | Industrial Internet of Things Corporate Website (Zajno pour KONUX), https://www.behance.net/gallery/53536049/Industrial-Internet-of-Things-Corporate-Website | non capturé | **Non vérifié** : Behance renvoie « HTTP ERROR 400 ». La page du projet sur zajno.com n'existe plus (404) et konux.com parle aujourd'hui de ferroviaire. |
| 16 | Speak Up Africa, identité (Éditions Pépé), https://www.behance.net/gallery/71073479/Speak-Up-Africa-Visual-identity-for-Social-Media | non capturé | **Non vérifié** : Behance renvoie « HTTP ERROR 400 ». Le test « condensée et jaune en grand » est fait avec le n° 20. |
| 17 | Industrial Company Website Inspiration, https://www.pinterest.com/ideas/industrial-company-website-inspiration/897062612591/ | non capturé | **Non vérifié** : fenêtre de connexion sur toute la page, aucune URL d'épingle exposée. Derrière la fenêtre (non capturé), les vignettes sont surtout anthracite et orange. |
| 18 | 34 Website Design – Industrial ideas, https://www.pinterest.com/jclewis33/website-design-industrial/ | non capturé | **Non vérifié** : même fenêtre de connexion. Derrière, des templates génériques (rouge, orange, jaune et marine). |
| 19 | Vibor (capteurs industriels), https://www.lapa.ninja/post/vibor/ | non capturé | **Non vérifié** : challenge Cloudflare. Le site réel de Vibor n'a pas été retrouvé. |
| 21 | AI Infrastructure Website (UX MIND agency, NIXTA Power Fabric), https://dribbble.com/shots/27803560-AI-Infrastructure-Website-Energy-Tech-UI-UX | [capture](captures/a-cote/21-dribbble-uxmind-nixta.jpg) | Hors secteur et hors ton : infrastructure IA (le brief interdit le jargon IA), maquette mobile sur béton, chiffres en monospace pointillé (le brief fixe deux familles). Le bloc « The numbers » est mieux montré par le n° 11. L'idée utile (valeur d'abord, détail ensuite) est citée au bloc 7. |
| 23 | B-Metal, https://onepagelove.com/b-metal (One Page Love, publié le 17 décembre 2019) | [capture](captures/a-cote/23-onepagelove-b-metal.jpg) | Le visuel principal est une photo plein cadre de meulage avec étincelles, cliché du secteur métal, au lieu du cadrage serré sur la machine demandé par le brief. Le grand titre noir sur blanc (Acumin, non condensée) est déjà mieux montré par les n° 4 et 20. |
| 7 (mobile) | Tractian en 390 × 844 px | [capture](captures/a-cote/mobile-tractian.jpg) | Contre-exemple de l'exigence mobile du brief : « Contact us » passe dans le menu, aucun lien `tel:`. Détail dans « Mobile ». |
| 12 (mobile) | I-care en 390 × 844 px | [capture](captures/a-cote/mobile-icare.jpg) | Contre-exemple : aucun lien `tel:`, chiffres clés en bas de page, seule une bulle de chat est fixe. Détail dans « Mobile ». |

---

## Galeries : requêtes lancées

| Plateforme | Requêtes ou pages | Résultat |
|---|---|---|
| Behance | n° 15 et 16 | Inaccessible : « HTTP ERROR 400 » au navigateur automatisé. |
| Pinterest | n° 17 et 18 | Inaccessible sans compte : fenêtre de connexion, aucune URL d'épingle exposée. Pas de capture (page de connexion). |
| Lapa Ninja | n° 2 et 19 | Inaccessible : challenge Cloudflare. |
| Dribbble | n° 3, 5, 8, 9 ; recherche « industrial yellow website » | 2 retenues (n° 20, 21). Sur la première page de résultats, la grande majorité des sites jaunes sont du BTP, de la toiture ou des engins : le jaune vif dit « chantier ». |
| Awwwards | n° 4 | Fiche vue. Pas de nouvelle recherche. |
| One Page Love | tag « industrial » (8 fiches) | 2 retenues (n° 22, 23). Les autres sont hors sujet (blog, restauration écologique), hors ligne depuis 2012-2013, ou au style « futuriste 3D » (Aevion, drone). |
| Land-book, Godly | non relancés | Bloqués sur ce projet (Cloudflare, redirection vers recent.design). |

Refonte du 2026-11-12 : aucune nouvelle recherche, car chaque bloc du brief a au moins une inspiration.

---

## Arbitrages

- **Installation : photos ou dessins ?** On dessine les 3 étapes au trait, dans le style du n° 5, parce que le capteur est fictif et qu'aucune photo de pose minutée ne peut exister. Le dessin montre le geste sans décor, et la séance photo se concentre sur le hero.
- **Source du coût d'un arrêt** : on affiche 36 000 $ pour une heure d'arrêt dans une grande usine de biens de grande consommation, avec le lien vers [Siemens, *The True Cost of Downtime 2024*](https://assets.new.siemens.com/siemens/assets/api/uuid:1b43afb5-2d07-47f7-9eb7-893fe7d0bc59/TCOD-2024_original.pdf) (PDF ouvert le 2026-11-13). C'est le secteur du rapport le plus proche de l'agroalimentaire de P1. Pas de chiffre ABB, faute de source ouverte ; le calculateur ramène le repère à l'échelle du visiteur.
- **Troisième police** : on reste sur Barlow Condensed et Barlow, avec chiffres tabulaires pour les valeurs de capteurs. Le brief fixe deux familles, et les chiffres tabulaires suffisent à aligner les données.
- **Photos d'équipe** : un « Qui sommes-nous » de 3 phrases, sans photo, avec le logo. Unsplash et Pexels bloquent le navigateur automatisé, et le brief exclut de toute façon la banque d'images.
- **Témoignages** : 3 cartes sans portrait ni chiffre de résultat, marquées « fictif ». Un visage ou un résultat sur un témoignage inventé le ferait passer pour vrai.
