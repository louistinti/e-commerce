# Benchmark visuel : Sobra (climat / énergie, B2B tertiaire)

Ce bench suit le brief client bloc par bloc : chaque référence retenue sert un bloc de l'arborescence ou une exigence précise du brief.

## Limites, à lire en premier

- **Vérification** : faite le 2026-11-12 avec un vrai navigateur (Chrome piloté par Playwright). La première version avait été écrite sans accès réseau, « d'après la description » des résultats de recherche. 17 des 22 références d'origine ont une capture, en 1440 × 900 px, au-dessus de la ligne de flottaison (plus une capture ciblée quand un élément clé est plus bas). Pour 2 d'entre elles, l'URL d'origine est bloquée et la capture vient d'une page équivalente : le site réel de carbonplan (n° 15) et les shots Dribbble du même projet Manatee Energy (n° 19). Les couleurs et les polices citées ont été relevées dans la page (`getComputedStyle`). Les chiffres cités sont ceux affichés le 2026-11-12.
- **Bloqué, non vérifié** :
  - Land-book (n° 4) et Lapa Ninja (n° 14, 15, 20) : challenge Cloudflare, non contourné.
  - Behance (n° 19) : erreur HTTP 400 renvoyée au navigateur automatisé.
  - Pinterest (n° 7, 21, 22) : mur de connexion.
  - Le site réel d'Energy Park (n° 20) : certificat HTTPS invalide, avertissement non contourné. Seule la fiche Awwwards a été vue.
  - Ubigreen (n° 17) : erreurs 429 sur les feuilles de style. Le texte est lisible et cité, mais la capture ne montre pas le vrai design.
- **URL morte** : eTactica (n° 14), `etactica.com` redirige vers une page de nom de domaine à vendre.
- **Corrections de la vérification** (gardées) : le H1 de BrainBox AI (n° 1) est « AI Control », pas le chiffre. Deepki (n° 5) ne cite pas l'IPMVP sur l'accueil. Le tag Dribbble « impact » (n° 6) montre des logos. Fuselab (n° 11) n'est pas une carte comparative de sites. Breakthrough Energy (n° 2) est un site clair. Les titres « Automatisez… » de Citron (n° 16) et la fourchette « 10 à 40 % » d'Advizeo (n° 18) ne sont pas sur l'accueil. Les calculateurs n° 8 et 9 sont des projets immobiliers.
- **Refonte du 2026-11-12** :
  - Chaque référence est triée : **10 inspirations** (n° 1, 3, 5, 6, 10, 13, 15, 17, 24, 25) et **15 références à côté** (n° 2, 4, 7, 8, 9, 11, 12, 14, 16, 18, 19, 20, 21, 22, 23). Le n° 6 regroupe deux pages : le shot Cambium est une inspiration, le tag « impact » est rangé à côté. Rien n'est supprimé.
  - Les captures sont rangées dans [`captures/inspis/`](captures/inspis/) et [`captures/a-cote/`](captures/a-cote/), noms et numéros inchangés. Les captures mobiles suivent le même tri.
  - Le bench est réorganisé selon l'arborescence du brief (section 6), avec un tableau de couverture.
  - **Aucune nouvelle référence** : la recherche Dribbble renvoie maintenant une page « Let's confirm you are human », non contournée. Une recherche Awwwards n'a rien donné d'utile pour les blocs 7 et 8 (voir « Galeries : requêtes lancées »).
  - **Tokens corrigés** contre l'accessibilité et la marque du brief : `color.semantic.success`, `color.semantic.warning` et l'anneau de focus échouaient aux contrastes WCAG, `color.semantic.info` était un bleu (« bleu tech » proscrit). Détail dans « Palette, polices, design tokens, composants ».
- **Passe du 2026-11-13** : Sobra est fictive, aucun chiffre ne lui est attribué. Le hero passe sur un chiffre public sourcé (« -26 % », bilan OPERAT 2024-2025), les fiches cas et l'impact cumulé n'ont plus de valeur, et les portraits d'équipe sont remplacés par un « Qui sommes-nous » sans photo : Unsplash (« Access Denied ») et Pexels (vérification Cloudflare) ont bloqué la recherche de photos de banque d'images. Détail dans « Arbitrages ».
- **Bannières cookies** : refusées partout où un refus existait. **Données personnelles** : sur Dribbble, avatars et noms des designers masqués avant capture.

**Répartition** : 25 références. Sites réels du secteur 5 · Dribbble 10 · Awwwards 3 · Pinterest 3 · Lapa Ninja 2 · Land-book 1 · Behance 1. Energy Park est cité sur Awwwards et sur Lapa Ninja.

---

## Couverture du brief

| Exigence du brief | Inspirations | Manque |
|---|---|---|
| 1. Hero : chiffre public « -26 % » en grand, sa source dessous, CTA « Audit gratuit » et « Estimer mes économies » | 1, 6, 3 | Aucune référence ne pose un chiffre avec sa source juste dessous. BrainBox (n° 1) écrit « up to ». |
| 2. Le problème en 3 chiffres sourcés | 1, 5, 15 | Aucune référence ne pose une source sous chacun de ses chiffres. Seul Citron (n° 16, à côté) cite une allégation réglementaire chiffrée. |
| 3. La solution en 3 colonnes, écrans de la plateforme dessinés sans valeurs | 5, 3, 13 | Pas de mise en page « capteurs / plateforme / accompagnement » en 3 colonnes vue. |
| 4. Simulateur : type, surface, facture → fourchette kWh/an et €/an, position 2030, hypothèses, envoi au formulaire | 24, 10, 13, 5 | L'envoi du résultat dans un formulaire n'est montré par aucune référence. |
| 5. Cas clients : carte à points d'exemple et 3 fiches sans gain chiffré (type, ville, leviers, courbe d'illustration) | 25, 17, 5 | Aucune fiche cas avec courbe avant/après vue. |
| 6. Impact cumulé : indicateurs MWh et tCO₂, méthode, facteur d'émission, sans valeur | 6, 25 | Aucune référence ne lie un chiffre d'impact à sa méthode ou à son facteur d'émission. |
| 7. Qui sommes-nous et cadres suivis (pas de logo de label) | aucune | Aucune référence vue ne montre un bloc équipe sans photo ni une liste de textes réglementaires servis. Recherche d'ajout bloquée sur Dribbble. Voir « Arbitrages ». |
| 8. Contact / demande d'audit : formulaire court, résultat prérempli, prise de rendez-vous | aucune | Aucun formulaire capturé : les références vues s'arrêtent au bouton (« Get a demo », « Get in touch »). Les champs et les messages sont déjà fixés par le brief (sections 6 et 9). |
| Pied de page : page Méthode | 15 | Une vraie page de méthode (formules, facteur d'émission) n'a pas été vue. |
| Mobile : CTA, simulateur au clavier et sur mobile, poids < 1,5 Mo, LCP ≤ 2,5 s (seuil « bon » des Core Web Vitals) | 5 (mobile), 3 (mobile) | Aucun simulateur mobile observé sur un site réel. Poids et LCP non mesurés. |
| Marque : vert profond, sable, jaune soleil, un seul accent | 3 | Aucune référence vue en vert profond et sable. Le jaune unique d'ON Energy (n° 3) est le repère le plus proche. |
| Marque : grotesque large pour les chiffres | 1, 6 | Les chiffres vus sont fins (n° 1) ou en serif (n° 6). Aucune grotesque large vue. |
| Accessibilité : clavier dans le simulateur, alternative en tableau aux graphiques, contraste du jaune | aucune | Non observable sur des captures. Les contrastes sont calculés dans les tokens. |
| Preuve « Des économies mesurées, pas promises » : page Méthode (IPMVP, période, correction climatique) | 17, 5 | Le n° 17 donne la période et la correction, le n° 5 le client. Aucune référence ne réunit les trois éléments. |
| Preuve « mi-chemin de 2030 » : « -26 % » et objectifs datés et sourcés | 5, 15 | Pas de rappel réglementaire daté vu. |
| Preuve « Installé sans travaux » : déroulé en 3 étapes, photo de capteur posé à produire | 3 | Photo d'équipement réel vue, mais pas de capteur posé ni de déroulé en étapes. |
| Preuve « Un ingénieur référent » : « Qui sommes-nous » court sans photo, rythme du suivi | aucune | Aucun bloc équipe sans photo vu. |
| Preuve « Des économies finançables » : CEE sous réserve d'éligibilité | aucune | Aucune mention CEE vue sur les références capturées. |
| Preuve « Impact mesuré » : indicateurs et facteur d'émission ADEME | 25 | Unité et période vues, lien vers le facteur non vu. |

---

## Inspirations, bloc par bloc

### 1. Hero

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 1 | BrainBox AI : AI Control (site réel, Canada), https://brainboxai.com/en/solutions/ai-control | [capture](captures/inspis/01-brainboxai-ai-control.jpg) · [chiffres](captures/inspis/01-brainboxai-chiffres.jpg) | Le chiffre très grand et fin, l'unité collée (« -40% », « -25% »), une légende courte dessous. Fond blanc, texte `#17171B`, Atlas Grotesk graisse 300. À éviter : le « by up to » de la légende, et le H1 « AI Control » qui relègue le chiffre (il n'est que dans la balise `<title>`). | « Le chiffre en grand » : pour Sobra, c'est le « -26 % » public du bilan OPERAT, et la légende devient sa source. |
| 6 | Cambium : Impact (Exo Ape, Dribbble), https://dribbble.com/shots/24767351-Cambium-Impact | [capture](captures/inspis/06-dribbble-cambium-impact.jpg) | Un seul chiffre géant sur fond crème, « 3.5 Gigaton CO2e », « / Year » en petit, une phrase de comparaison, un bouton « More impact ». À éviter : le globe 3D (planète proscrite). | Un chiffre, une phrase, un CTA : la structure du hero. |
| 3 | ON Energy (Awwwards SOTD 09/03/2026, Studio 28K), https://www.on.energy/ | [site](captures/inspis/03-on-energy-site.jpg) · [fiche](captures/inspis/03-on-energy-awwwards.jpg) | Un seul accent jaune `#FFF313`, porté par le logo et le bouton « Get in touch » à texte noir. Photo d'équipement réel en niveaux de gris. Fond noir `#000`, H1 64 px graisse 300. À éviter : le noir intégral et la 3D. | CTA « Demander mon audit gratuit » en accent unique, photo réelle plutôt qu'illustration. |

### 2. Le problème en 3 chiffres

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 1 | BrainBox AI | [chiffres](captures/inspis/01-brainboxai-chiffres.jpg) | Deux grandes cartes blanches sur fond gris, un chiffre par carte, flèche vers le bas, légende courte. | Les 3 chiffres en cartes. Pour Sobra, une ligne de source et de date sous chaque chiffre. |
| 5 | Deepki (site réel, FR), https://www.deepki.com/ | [capture](captures/inspis/05-deepki.jpg) | Une courbe de trajectoire carbone 2020-2050, avec une infobulle « 2033 » qui compare objectif, actions et scénario tendanciel. | Situer -26 % (fait) et -40 % (2030) sur une même courbe datée. |
| 15 | carbonplan (site réel), https://carbonplan.org/ | [site](captures/inspis/15-carbonplan.jpg) | Des dates visibles en capitales (« MAY 07 2026 »), des chiffres en mono dans la marge. | « Chaque chiffre a sa source » : la source et la date en mono sous le chiffre. |

Détail repris d'une référence à côté : Citron (n° 16) affiche « Citron® répond à 3 des 7 obligations liées au décret BACS ». C'est le format d'une allégation réglementaire chiffrée, à dater et à sourcer pour Sobra.

### 3. La solution

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 5 | Deepki | [capture](captures/inspis/05-deepki.jpg) | Le hero montre l'écran de la plateforme en grand, recadré sur la donnée. À éviter : le superlatif « Most trusted » du H1. | Écrans de la plateforme, dessinés sans valeurs et légendés « illustration ». |
| 3 | ON Energy | [site](captures/inspis/03-on-energy-site.jpg) | Photo d'un équipement réel (une armoire électrique) désaturée, sans décor. | Colonne « capteurs » et photo de capteur posé (à produire). |
| 13 | Smart Energy Dashboard Concept (Zajno, Dribbble), https://dribbble.com/shots/25108413-Smart-Energy-Dashboard-Concept | [capture](captures/inspis/13-dribbble-zajno-smart-energy.jpg) | La consommation découpée par usage (éclairage, réfrigérateur, climatisation) en barres. À éviter : le fond noir et le contexte domestique. | Le sous-comptage par usage des capteurs Sobra, montré dans la colonne « plateforme ». |

Détails repris de références à côté : Breakthrough Energy (n° 2) pose un grand titre sur une photo réelle de personnes au travail, un repère pour la colonne « accompagnement ». Pas de portrait pour Sobra : le brief retient un « Qui sommes-nous » sans photo (voir « Arbitrages »). BatteryLoop (n° 12) chiffre le gain levier par levier.

### 4. Simulateur

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 24 | Solar energy saver calculator (Dribbble), https://dribbble.com/shots/24936784-Solar-energy-saver-calculator | [capture](captures/inspis/24-dribbble-solar-saver-calculator.jpg) | Le modèle le plus direct. Entrées à gauche : un curseur de facture doublé d'un champ « €23 Euro », des boutons segmentés. Résultat à droite, mis à jour en direct : « Estimated annual savings (EUR) €324 », bascule « 1 year / 25 years », réduction de CO₂ en kg par an. Une phrase dit que le calcul est indicatif. À éviter : l'équivalence en arbres plantés. | Type de bâtiment en boutons segmentés, surface en curseur doublé d'un champ (utilisable au clavier), hypothèses affichées. |
| 10 | Mobile Energy Savings Calculator (Dribbble), https://dribbble.com/shots/787436-Mobile-Energy-Savings-Calculator | [capture](captures/inspis/10-dribbble-mobile-energy-calculator.jpg) | « 38% Saved per year* » avec un astérisque relié à une note « *Based on US national… » sous le résultat. Gains à 5, 10 et 15 ans. À éviter : l'écran bleu ardoise (bleu proscrit). | « Les hypothèses sont affichées » : l'astérisque et la note collée au résultat. |
| 13 | Zajno | [capture](captures/inspis/13-dribbble-zajno-smart-energy.jpg) | Le résultat en fourchette, l'unité en petit : « 52–71 kWh per month ». | « Fourchette d'économies en kWh/an et en €/an ». |
| 5 | Deepki | [capture](captures/inspis/05-deepki.jpg) | La courbe de trajectoire annotée, avec une infobulle datée. | « Position sur la trajectoire 2030 » du bâtiment simulé. |

Détails repris de références à côté : Sunora AI (n° 23) détaille le résultat en un tableau de 3 lignes, le format des 3 sorties du brief (kWh/an, €/an, trajectoire). Opendoor (n° 8) place le résultat en bas de la carte, sous les entrées, l'ordre à garder en mobile.

### 5. Cas clients

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 25 | MapMortar : Decarbonisation Platform Design (Lumi studio, Dribbble), https://dribbble.com/shots/26536376-MapMortar-Decarbonisation-Platform-Design | [capture](captures/inspis/25-dribbble-mapmortar-decarbonisation.jpg) | Interface claire, carte de quartier en gris, repères colorés par statut de trajectoire : « On track » (noir), « Off track » (orange), « No plan » (gris). | « Carte des bâtiments équipés (points agrégés) » : des points colorés selon la trajectoire 2030, légende chiffrée sous la carte. |
| 17 | Ubigreen (site réel, FR), https://www.ubigreen.com/en/ | [témoignage](captures/inspis/17-ubigreen-cas.jpg) · [accueil](captures/inspis/17-ubigreen.jpg) (sans mise en forme) | Une citation datée : de 2018 à 2021, gaz corrigé -5,3 % et électricité -13 %, attribuée au responsable énergie du Conseil départemental de la Haute-Garonne, avec les leviers. Design non vu. | Les fiches cas (type, ville, gain, période) et un cas de collectivité pour le persona Marc. |
| 5 | Deepki | [chiffres](captures/inspis/05-deepki-chiffres.jpg) | 3 cartes chiffres signées chacune d'un logo client : « 6,500+ buildings monitored » (CBRE), « 40% time saved on reporting campaigns » (Icade), « 32% reduction in energy consumption » (Heppner). À éviter : le « 32 % » sans période ni périmètre. | La carte signée d'un nom de client, pour le persona Claire (cas de foncières). Pour Sobra, la carte porte le type de bâtiment et les leviers, sans gain chiffré. |

Détails repris de références à côté : Advizeo (n° 18) titre un replay « Covéa Immobilier : -33 % de consommation sur 1000 bâtiments, la méthode » (chiffre, périmètre et méthode dans la même ligne). BatteryLoop (n° 12) décompose le gain par levier, à transposer en clair (réglages CVC, détection de dérives, suivi).

### 6. Impact cumulé

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 6 | Cambium : Impact | [capture](captures/inspis/06-dribbble-cambium-impact.jpg) | Un chiffre par écran, l'unité en petit, une phrase qui le rend concret. | La mise en page des indicateurs MWh et tCO₂ évités. |
| 25 | MapMortar | [capture](captures/inspis/25-dribbble-mapmortar-decarbonisation.jpg) | Cartes chiffres avec l'unité et la période : « 876,000 kg per year » de CO₂ scope 1, « 257,200 kWh per year ». | Les cartes d'indicateurs avec unité et période. Pour Sobra, pas de valeur : l'unité, la période et le lien vers la méthode. |

Détail repris d'une référence à côté : Advizeo (n° 18) date son chiffre cumulé (« 1 TWh d'économies d'énergie réalisées en 2025 »).

### 7. Qui sommes-nous et cadres suivis

Aucune inspiration. Aucune référence vue ne montre un bloc équipe sans photo ni une liste de textes réglementaires servis. Ce que le brief impose suffit à cadrer le bloc : un « Qui sommes-nous » de 3 phrases avec le logo, les textes servis cités avec leur source (décret tertiaire, BACS, CEE sous réserve d'éligibilité), aucun logo de label, de partenaire ni de l'ADEME.

**Photos d'équipe** : recherche faite le 2026-11-13, sans résultat exploitable. Unsplash (`/s/photos/hvac-engineer`, `/s/photos/engineer-building`) renvoie « Access Denied », Pexels (`/search/hvac engineer/`) une vérification Cloudflare. Aucune des deux n'a été contournée. Pas d'exigence de photo réelle ni de portrait dans ce bench.

### 8. Contact / demande d'audit

Aucune inspiration. Les références vues s'arrêtent au bouton (« Get a demo » chez Deepki, « Get in touch » chez ON Energy). Le formulaire suit le brief : nom, organisation, e-mail, surface totale, nombre de sites, résultat du simulateur prérempli, prise de rendez-vous, et les messages de la section 9.

### Pied de page : page Méthode

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 15 | carbonplan | [site](captures/inspis/15-carbonplan.jpg) | Le ton sec, les dates visibles, des petites data-viz comme illustration à la place d'une photo, des chiffres en mono. Site sombre par défaut (`#1B1E23`), avec un bouton pour passer en clair. À éviter : le fond sombre par défaut. | « Page Méthode (calculs du simulateur et du compteur) ». |

---

## Mobile

Observé en 390 × 844 px sur 3 sites réels.

| Site | Capture | Ce qu'on voit au premier écran |
|---|---|---|
| Deepki (inspiration) | [mobile](captures/inspis/mobile-deepki.jpg) | H1 35 px sur 4 lignes, la preuve « Trusted by 900+ companies », puis le bouton « Get a demo » (51 px de haut). La capture de la plateforme rétrécit au point d'être illisible. Plus bas, les 3 cartes chiffres s'empilent, environ 350 px de haut chacune. Pas de bouton collant. |
| ON Energy (inspiration) | [mobile](captures/inspis/mobile-on-energy.jpg) | Logo et menu dans une pastille jaune en haut à droite, H1 37 px graisse 300 sur la photo produit, carte jaune « Explore AI UPS » en bas. Le bouton « Get in touch » n'est pas dans le premier écran. |
| Citron (à côté) | [mobile](captures/a-cote/mobile-citron.jpg) | H1 24 px, bouton « Contacter un expert » de 38 px de haut seulement (sous les 44 px du critère 2.5.5 des WCAG 2.2, niveau AAA), logos clients dès le premier écran. Le bouton flottant des cookies recouvre le bas à gauche. |

Ce qu'on en tire, relié au brief :
- **Critère « comprendre en 5 secondes » et indicateur des demandes d'audit** : le CTA « Demander mon audit gratuit » dans le premier écran, à 48 px de haut, comme Deepki (51 px). Citron (38 px) est trop petit, ON Energy cache le sien.
- **Captures réelles de la plateforme (bloc 3)** : ne pas réduire une capture entière en mobile, la recadrer sur une seule courbe lisible (Deepki la rend illisible).
- **Blocs 2 et 6** : les cartes chiffres empilées prennent vite de la place (Deepki : plus de 1 000 px pour 3 cartes). Garder des cartes compactes.
- **Simulateur au clavier et sur mobile** : non observé, aucun des 3 sites ne propose d'outil juste après le hero. Le brief place le simulateur en bloc 4 et le relie au hero par le CTA « Estimer mes économies ». En mobile, l'ordre est entrées puis résultat (repère du n° 8, à côté), et le résultat reste visible sans défilement après le calcul.
- **Poids < 1,5 Mo et LCP ≤ 2,5 s (Core Web Vitals)** : plusieurs références ouvrent sur une vidéo plein cadre (n° 2, 18, 20, à côté). Pour Sobra, une photo fixe compressée. Le poids des pages vues n'a pas été mesuré.

---

## Directions

Le brief demande un moodboard en 3 pistes (section 10). Les trois pistes restent : elles utilisent la palette du brief et n'emploient aucun visuel proscrit. Aucune n'est retirée.

**A. « Relevé de compteur » (recommandée)**
Fond sable, grands chiffres en Archivo étendu vert profond, une seule courbe avant/après en trait fin. Le jaune marque le delta (le « -26 % » du hero, la fourchette du simulateur) en fond, derrière un chiffre vert profond, jamais en texte sur sable.
Photos de capteurs et de locaux techniques (à produire : banque d'images ou prise de vue), en noir et blanc légèrement teinté vert. Pas de portrait d'équipe.
Sensation : précision d'ingénieur, rapport technique bien mis en page.
Inspirations :
- photo d'équipement désaturée et un seul accent jaune (n° 3) ;
- un chiffre par écran, unité en petit, une phrase dessous (n° 6, n° 1) ;
- fiche signée par un type de client et datée, sans gain chiffré pour Sobra (n° 5, n° 17) ;
- simulateur entrées à gauche, résultat à droite, phrase « indicatif » (n° 24), résultat en fourchette (n° 13) ;
- carte à points colorés selon la trajectoire (n° 25).

**B. « Tableau de bord de nuit »**
Fond vert profond quasi noir, chiffres en sable, jaune pour les gains. Le simulateur ressemble à un instrument.
Inspirations : le registre d'ON Energy (n° 3 : fond sombre, photo produit en niveaux de gris, un seul accent jaune), et la courbe de trajectoire de Deepki (n° 5) en version sombre.
Risque : les dashboards sombres vus (n° 11 et 12, à côté, et n° 13) se ressemblent tous, l'effet « SaaS générique » est fort. Pas de néon (le n° 11 est le contre-exemple). À garder pour la section Impact cumulé si la piste A est choisie.

**C. « Rapport annuel éditorial »**
Mise en page magazine : Space Grotesk, grandes marges, chiffres en exergue, notes de bas de page pour les sources.
Inspirations : le ton et les dates visibles de carbonplan (n° 15, pas sa mise en page sombre), la citation datée et attribuée d'Ubigreen (n° 17).
Très crédible auprès des foncières et des investisseurs. Moins direct pour la conversion : il faut un CTA collant.

**Observation sur l'accent jaune** : les 3 sites primés vus utilisent un seul accent jaune ou vert-jaune fluo (ON Energy `#FFF313`, Energy Park `#FFF555`, Breakthrough Energy `#DFFF5C`). Le jaune soleil de Sobra (`#F2C230`) est plus chaud et plus doré, ce qui le distingue de cette tendance. La palette ne change pas.

---

## Palette, polices, design tokens, composants

Toutes les valeurs ont été vérifiées contre le brief : palette vert profond, sable, jaune soleil, pas de bleu « tech », WCAG 2.2 AA (4,5:1 pour le texte, 3:1 pour les éléments graphiques et l'indicateur de focus). Contrastes recalculés le 2026-11-12 (formule de luminance relative WCAG).

**Corrections de la refonte** :
- `color.semantic.success` `#2F7D4F` → `#276B43` : 4,06:1 sur sable, sous 4,5:1 pour un message texte. La nouvelle valeur donne 5,17:1.
- `color.semantic.warning` `#B86E00` → `#8F5600` : prévu « texte sur clair », mais 3,21:1 sur sable. La nouvelle valeur donne 4,84:1.
- `color.semantic.info` `#2D5C7A` → `#2E5B4B` : c'était un bleu, proscrit par le brief. La nouvelle valeur est un vert-gris, 6,23:1 sur sable.
- `shadow.focus` `0 0 0 3px #F2C230` → anneau vert profond sur fond clair : le jaune sur sable donne 1,35:1, sous les 3:1 demandés pour un indicateur de focus. L'anneau jaune reste sur fond vert profond (7,44:1), sous le nom `shadow.focus-on-dark`.

### Palette (direction A)

| Rôle | Hex | Usage |
|---|---|---|
| Vert profond | `#0E3B2E` | Titres, chiffres, fond des sections sombres |
| Vert encre | `#0A2A21` | Texte courant sur sable (contraste élevé) |
| Sable | `#EFE6D2` | Fond principal |
| Sable clair | `#F8F4EA` | Cartes, fond du simulateur |
| Jaune soleil | `#F2C230` | Accent unique : fond du delta d'économie, CTA et focus sur fond vert |
| Gris vert data | `#7C8F86` | Courbe « avant » sur sable clair (pas de texte, voir les contrastes) |
| Rouge alerte (rare) | `#B8452F` | Dérive de consommation dans les courbes |

Contrastes : le jaune `#F2C230` sur sable `#EFE6D2` donne 1,35:1, il **échoue**. Le jaune ne s'utilise que sur vert profond (7,44:1 avec `#0E3B2E`), ou en fond derrière un texte vert profond.
Le gris vert data `#7C8F86` donne 2,76:1 sur sable et 3,12:1 sur sable clair : trop faible pour du texte, et sous 3:1 pour un trait de courbe sur sable. Les légendes passent en `neutral.700` `#3F4A44` (7,44:1 sur sable). `#7C8F86` reste pour la courbe « avant », sur sable clair uniquement. Le rouge alerte `#B8452F` donne 4,30:1 sur sable : valable pour un trait de courbe, pas pour du texte courant.

### Polices (Google Fonts)

Conformes au brief (« Archivo en largeur étendue ou Space Grotesk » pour les chiffres).
- **Archivo** (police variable, axe de largeur jusqu'à 125, plus la graisse) : gros chiffres et titres en largeur étendue, graisses 700 à 800.
- **Space Grotesk** : alternative pour les titres en direction C.
- **Inter** : texte courant et interface du simulateur.
- **JetBrains Mono** ou **IBM Plex Mono** : unités, valeurs dans les graphiques, notes de méthode.

### 3 « à ne pas faire »

1. **Pas de feuille, de planète, d'éolienne ni de prise électrique verte**, et pas de vert pomme. Rien qui crie « écolo » à la place de « mesuré ».
2. **Pas de dashboard décoratif** : pas de widgets inventés, pas de néon sur fond noir. Montrer une vraie courbe (anonymisée) avec une annotation lisible.
3. **Pas de chiffre sans méthode** : pas de « jusqu'à -40 % », pas de compteur qui tourne sans date de mise à jour ni lien vers le calcul.

### Design tokens : couleurs

| Token | Hex | Usage |
|---|---|---|
| `color.brand.primary` | `#0E3B2E` | Vert profond : titres, chiffres, fonds sombres, bouton primaire |
| `color.brand.primary-hover` | `#155240` | Survol du bouton primaire |
| `color.brand.ink` | `#0A2A21` | Texte courant |
| `color.brand.sand` | `#EFE6D2` | Fond principal |
| `color.brand.sand-light` | `#F8F4EA` | Cartes, simulateur |
| `color.brand.accent` | `#F2C230` | Jaune soleil : fond du delta d'économie, CTA et focus sur fond vert uniquement |
| `color.semantic.success` | `#276B43` | Économie confirmée, envoi réussi (corrigé) |
| `color.semantic.error` | `#B3261E` | Erreur de champ, échec d'envoi |
| `color.semantic.warning` | `#8F5600` | Dérive de consommation, hors périmètre (texte sur clair, corrigé) |
| `color.semantic.info` | `#2E5B4B` | Notes de méthode, infobulles (corrigé, n'est plus un bleu) |
| `color.neutral.900` | `#1A1F1C` | Texte maximal |
| `color.neutral.700` | `#3F4A44` | Texte secondaire, légendes et valeurs des graphiques |
| `color.neutral.500` | `#7C8F86` | Courbe « avant » et traits d'axe, sur sable clair (pas de texte) |
| `color.neutral.300` | `#C9CFC6` | Bordures |
| `color.neutral.100` | `#EEF0EB` | Fonds neutres |
| `color.neutral.0` | `#FFFFFF` | Champs de formulaire |

Contrastes sur sable `#EFE6D2` : `brand.ink` 12,39:1 · `brand.primary` 10,05:1 · `primary-hover` 7,32:1 · `neutral.700` 7,44:1 · `semantic.info` 6,23:1 · `semantic.error` 5,27:1 · `semantic.success` 5,17:1 · `semantic.warning` 4,84:1. `sand-light` sur `brand.primary` (bouton primaire) : 11,36:1, et 8,27:1 au survol. Le jaune `#F2C230` est interdit en texte sur fond clair (1,35:1 sur sable). `neutral.500` ne sert pas au texte (2,76:1 sur sable).

### Design tokens : typographie

| Token | Police | Taille (desktop / mobile) | Graisse | Interligne |
|---|---|---|---|---|
| `type.display` (chiffre du hero) | Archivo, largeur 125 | 120 / 64 px | 800 | 0.95 |
| `type.h1` | Archivo, largeur 115 | 56 / 36 px | 700 | 1.05 |
| `type.h2` | Archivo, largeur 110 | 40 / 28 px | 700 | 1.1 |
| `type.h3` | Archivo | 24 / 20 px | 600 | 1.25 |
| `type.stat` (cartes chiffres) | Archivo, largeur 125 | 64 / 48 px | 800 | 1.0 |
| `type.body-lg` | Inter | 20 / 18 px | 400 | 1.55 |
| `type.body` | Inter | 17 / 16 px | 400 | 1.6 |
| `type.small` | Inter | 14 px | 500 | 1.45 |
| `type.mono` (unités, méthode) | JetBrains Mono | 14 / 13 px | 500 | 1.4 |

### Design tokens : espacement, rayons, ombres, motion

Espacement (base 4 px) : `space.1` 4 · `space.2` 8 · `space.3` 12 · `space.4` 16 · `space.5` 24 · `space.6` 32 · `space.7` 48 · `space.8` 64 · `space.9` 96 · `space.10` 128 px.
Section : 128 px desktop, 64 px mobile. Gouttière : 24 px, et 16 px de marge latérale sur mobile.

Rayons : `radius.sm` 4 px (champs, tags) · `radius.md` 8 px (boutons) · `radius.lg` 16 px (cartes, simulateur) · `radius.full` 999 px (pastilles). Les angles restent assez vifs pour garder un registre technique.

Ombres :
- `shadow.none` : par défaut, on préfère les bordures `neutral.300`.
- `shadow.sm` : `0 1px 2px rgba(10,42,33,.08)` (cartes au repos).
- `shadow.md` : `0 4px 16px rgba(10,42,33,.10)` (simulateur, carte survolée).
- `shadow.focus` : `0 0 0 2px #F8F4EA, 0 0 0 4px #0E3B2E` (anneau de focus sur fond clair, 10,05:1 sur sable, corrigé).
- `shadow.focus-on-dark` : `0 0 0 3px #F2C230` (anneau de focus sur fond vert profond, 7,44:1).

Motion :
- Durées : `motion.fast` 120 ms (survol, focus) · `motion.base` 200 ms (ouverture, transitions d'état) · `motion.slow` 400 ms (mise à jour du résultat du simulateur) · `motion.count` 1 200 ms (compteur, une seule fois à l'apparition).
- Easings : `ease.standard` `cubic-bezier(.2,0,0,1)` · `ease.enter` `cubic-bezier(0,0,0,1)` · `ease.exit` `cubic-bezier(.3,0,1,1)`.
- `prefers-reduced-motion` : compteur et courbes affichés directement à leur valeur finale.

### Composants clés

- **Bouton primaire** : fond `brand.primary`, texte `sand-light`, `radius.md`, hauteur 48 px (zone tactile d'au moins 44 px, critère 2.5.5 des WCAG 2.2).
  - Survol : `primary-hover`. Focus : `shadow.focus`. Actif : enfoncé de 1 px.
  - Désactivé : fond `neutral.300` et texte `neutral.700`. Ajouter `aria-disabled` et dire pourquoi il est désactivé.
  - Chargement : spinner et libellé « Envoi… », sans changement de largeur.
- **Bouton secondaire** : contour de 1,5 px `brand.primary`, fond transparent.
  - Survol : fond `neutral.100`. Focus, désactivé et chargement comme le primaire.
  - **Sur fond vert** : fond `accent` et texte `brand.primary`, focus `shadow.focus-on-dark`.
- **Carte chiffre** : fond `sand-light`, chiffre `type.stat`, unité `type.mono`, une ligne de contexte, et le lien « source » avec sa date en `type.small` (blocs 2 et 6).
- **Carte cas client** : mini-courbe avant/après sans valeurs, légendée « illustration », type de bâtiment, ville, leviers, indicateur suivi, et le lien « Voir la courbe complète » (bloc 5).
- **Formulaire / simulateur** :
  - libellé toujours visible au-dessus du champ ;
  - aide en `type.small` ;
  - erreur en `semantic.error`, avec icône et texte (jamais la couleur seule) ;
  - type de bâtiment en boutons segmentés, surface en curseur doublé d'un champ numérique (n° 24) ;
  - résultat annoncé par `aria-live="polite"` ;
  - résultat en fourchette avec l'unité en petit (n° 13), suivi d'une phrase « estimation indicative » et du lien vers les hypothèses (n° 24, n° 10) ;
  - courbe de position sur la trajectoire 2030 doublée d'un tableau de données.

| À faire | À ne pas faire |
|---|---|
| Un seul bouton primaire par écran (audit ou simulation) | Deux CTA jaunes côte à côte |
| Afficher la source et la date sous chaque chiffre | Un compteur animé sans date ni méthode |
| Libellés de champ visibles et unités explicites (m², kWh) | Placeholder qui sert de libellé |
| Erreur décrite (ce qui s'est passé, pourquoi, comment corriger) | « Champ invalide » en rouge seul |
| Courbes avec une alternative en tableau de données | Graphique sans texte alternatif ni légende |
| Jaune réservé à l'accent, et au focus sur fond vert | Jaune en texte ou en anneau de focus sur fond sable |

---

## À côté

| # | Référence | Capture | Pourquoi à côté |
|---|---|---|---|
| 2 | Breakthrough Energy (Awwwards SOTD 15/01/2026, Resn), https://www.breakthroughenergy.org/ | [fiche](captures/a-cote/02-breakthrough-energy-awwwards.jpg) · [site](captures/a-cote/02-breakthrough-energy-site.jpg) · [plus bas](captures/a-cote/02-breakthrough-energy-sections.jpg) | Accueil sans chiffre ni preuve (un titre, une newsletter, un menu) : contraire au ton « concret, chiffré ». Collage avec éoliennes et champs (éoliennes proscrites). Accent vert-jaune `#DFFF5C` hors palette. Détail repris au bloc 3. |
| 4 | Galactic Energy (Land-book), https://land-book.com/websites/26111-galactic-energy | aucune | Non vérifié : Land-book bloque par un challenge Cloudflare. Le nom correspond probablement au lanceur de fusées chinois, hors secteur. |
| 6 (tag) | Tag Dribbble « impact », https://dribbble.com/tags/impact | [tag](captures/a-cote/06-dribbble-tag-impact.jpg) | Page de logos (« ImpactPilot »), rien pour un bloc du brief. Le shot Cambium du même numéro est une inspiration. |
| 7 | Green Energy Website Design Inspiration (Pinterest) | aucune | Non vérifié : mur de connexion. Derrière la fenêtre, des gabarits à éoliennes et vert vif (proscrits). |
| 8 | Savings calculator (Opendoor Design, Dribbble), https://dribbble.com/shots/13944005-Savings-calculator | [capture](captures/a-cote/08-dribbble-opendoor-savings-calculator.jpg) | Projet immobilier, contexte seulement. Le n° 24 montre mieux le simulateur. Détail repris au bloc 4 et en mobile. |
| 9 | Savings Slider (Dribbble), https://dribbble.com/shots/2635549-Savings-Slider | [capture](captures/a-cote/09-dribbble-savings-slider.jpg) | Projet immobilier, une seule image floue. Le curseur doublé d'un champ est mieux montré par le n° 24. |
| 11 | Energy Consumption Dashboard UI (Fuselab, Dribbble), https://dribbble.com/shots/25574779-Energy-Consumption-Dashboard-UI | [capture](captures/a-cote/11-dribbble-fuselab-energy-dashboard.jpg) | Ville 3D de nuit en néon bleu et magenta : bleu « tech » proscrit, et dashboard décoratif contraire à « pas de widgets inventés » (« à ne pas faire » n° 2). Ne montre qu'un site, pas une carte comparative. |
| 12 | BatteryLoop dashboard (Dribbble), https://dribbble.com/shots/21454833-Dashboard-for-an-innovative-energy-storage-product | [capture](captures/a-cote/12-dribbble-batteryloop-dashboard.jpg) | Concept sombre vert-noir en SEK, pas une capture réelle, et le gain par levier n'est pas demandé tel quel par le brief. Détail repris aux blocs 3 et 5. |
| 14 | eTactica (Lapa Ninja), https://www.lapa.ninja/post/etactica/ | aucune | Non vérifié : Lapa Ninja bloqué par Cloudflare, et le site est mort (domaine à vendre). |
| 16 | Citron (site réel, FR), https://citron.io/ | [capture](captures/a-cote/16-citron.jpg) · [mobile](captures/a-cote/mobile-citron.jpg) | H1 exhortatif avec point d'exclamation (ton « sans superlatif »), dégradé vert et illustration d'une femme à la loupe devant une maquette de tableau de bord (le brief demande des captures réelles), bouton magenta `#E71B6D` hors palette, bouton mobile de 38 px. Détail repris au bloc 2. |
| 18 | Advizeo (by Hager, site réel, FR), https://www.advizeo.io/ | [capture](captures/a-cote/18-advizeo.jpg) · [chiffres](captures/a-cote/18-advizeo-chiffres.jpg) | Contre-exemple de la règle « chaque chiffre a une source » : « + de 300 clients » puis « plus de 250 acteurs » sur la même page, « leader de l'Energy Management » sans source. Palette violet, rose et bleu nuit `#0D123C` hors marque. Détails repris aux blocs 5 et 6. |
| 19 | Manatee Energy (tubik, Behance + Dribbble), https://dribbble.com/shots/26339570-Website-Design-Landing-page-for-Manatee-Energy | [Dribbble](captures/a-cote/19-dribbble-manatee-energy-landing.jpg) | Illustration isométrique et bouton bleu vif (bleu « tech » proscrit), plateforme grand public. Behance non vérifié (erreur 400). |
| 20 | Energy Park (Awwwards SOTD 07/12/2023, Outpost), https://www.awwwards.com/sites/energy-park | [fiche](captures/a-cote/20-energy-park-awwwards.jpg) | Site réel non vérifié (certificat HTTPS invalide). Vidéo aérienne de route en forêt : décor nature contraire à « mesuré », et vidéo lourde pour le poids mobile. |
| 21 | Renewable Energy / Clean Tech Web Design (Pinterest), https://www.pinterest.com/jackkoppa/renewable-energyclean-tech-web-design/ | aucune | Non vérifié : mur de connexion. Tableau de 12 ans, infographie devinée avec éolienne (proscrite). |
| 22 | Utilities / Energy websites (Pinterest), https://www.pinterest.com/backinvenice/utilities-energy-websites/ | aucune | Non vérifié : mur de connexion. Sites devinés en bleu, violet et rose, hors marque. |
| 23 | Sunora AI : Energy Calculator Web (Trexa Lab, Dribbble), https://dribbble.com/shots/27487059-Sunora-AI-Solar-Energy-Website-Design-Energy-Calculator-Web | [capture](captures/a-cote/23-dribbble-sunora-energy-calculator.jpg) | « 70% Potential bill reduction » sans méthode (règle « chaque chiffre a une source »), champ solaire au couchant, CTA vert vif hors palette. Détail repris au bloc 4. |

---

## Galeries : requêtes lancées

| Galerie | Requête ou page | Résultat |
|---|---|---|
| Dribbble | Tag « impact » | Logos, rien de « Our impact » (n° 6, tag à côté). |
| Dribbble | Shots ouverts par leur URL (n° 6, 8 à 13, 19, 23 à 25) | Ouverts et capturés. Les n° 23, 24 et 25 ont été ajoutés lors de la vérification. |
| Dribbble | Recherche « energy case study » (refonte du 2026-11-12) | Page « Let's confirm you are human », non contournée. Aucun résultat. |
| Awwwards | Fiches n° 2, 3, 20 | Ouvertes et capturées. |
| Awwwards | Recherche « energy efficiency » (refonte du 2026-11-12) | 31 fiches listées. Energy Upgrades (Acron, studio DAYTWO, mention du 13/11/2025) ouverte : éléments 3D animés, rien pour les blocs 7 et 8. Non retenue. |
| One Page Love | « energy » | 20 résultats hors sujet (un guide de 2012 hors ligne, des gabarits solaires). Aucun retenu. |
| Godly | non essayé | Redirige vers recent.design. |
| Land-book, Lapa Ninja | n° 4, 14, 15, 20 | Challenge Cloudflare, non contourné. |
| Behance | n° 19 | Erreur HTTP 400. |
| Pinterest | n° 7, 21, 22 | Mur de connexion. |

---

## Arbitrages

- **Hero.** On ouvre sur le chiffre public « -26 % » (bilan OPERAT 2024-2025), sa source juste dessous, et le titre de l'option A. Sobra n'a pas de résultat mesuré : un « -27 % » serait inventé.
- **Bloc 7.** Le bloc devient « Qui sommes-nous et cadres suivis », sans logo de label ni de partenaire, parce que Sobra n'en a obtenu aucun. Les textes servis (décret tertiaire, BACS, CEE sous réserve d'éligibilité) sont cités en clair avec leur source.
- **Photos d'équipe.** On remplace les portraits par un « Qui sommes-nous » de 3 phrases, sans photo, avec le logo. La recherche de photos de banque d'images a été bloquée sur Unsplash et sur Pexels le 2026-11-13, et on ne cherche pas plus loin.
- **Cas clients et impact cumulé.** Les 3 fiches et les indicateurs d'impact ne portent aucune valeur, parce qu'elle serait inventée. Les fiches montrent le type, la ville, les leviers et l'indicateur suivi, avec une courbe légendée « illustration ».
- **Écrans de la plateforme.** On les dessine nous-mêmes, sans valeur chiffrée, légendés « illustration », parce qu'il n'existe pas de plateforme à capturer.
