# Benchmark visuel : Veilla (santé / medtech)

Ce bench suit le brief client bloc par bloc : chaque référence retenue sert un bloc de l'arborescence (section 6 du brief) ou une exigence précise du brief.

> **Veilla est fictive.** Les références ci-dessous sont réelles.

## Limites, à lire en premier

- **Vérification** : faite le 2026-11-12 avec un vrai navigateur (Chrome piloté par Playwright). La première version avait été écrite sans navigateur. 14 des 20 références d'origine ont été vues : 10 à leur URL (n° 1, 2, 5, 6, 7, 8, 10, 12, 15, 17), 4 sur le site réel ou la page du studio parce que la galerie était bloquée (n° 3, 13, 14, 20). Captures en 1440 × 900 px, au-dessus de la ligne de flottaison, plus une seconde capture quand un bloc clé est plus bas. Les couleurs et les polices citées ont été relevées dans la page (`getComputedStyle`), ou dans l'image du shot pour Dribbble. Les chiffres cités sont ceux affichés le 2026-11-12.
- **Non vérifié (6)** : Withings n° 4 (challenge Cloudflare, non contourné), Behance n° 9 et 11 (erreur HTTP 400), Carbon Health n° 16 (Land-book et carbonhealth.com bloqués par Cloudflare), épingles Pinterest n° 18 et 19 (mur de connexion : seuls le titre, le texte alternatif et la description ont été lus). Lapa Ninja (n° 3, 13) et Land-book (n° 14) bloquent aussi par Cloudflare.
- **Ajouts de la vérification (4)** : n° 21 Calmedica (concurrent français direct), n° 22 et 23 (Dribbble, à la place des Behance n° 11 et 9), n° 24 (Dribbble, sauge). Plus 4 captures mobiles en 390 × 844 px (M1 à M4).
- **Corrections de la vérification** (gardées) :
  1. Implicity (n° 6) n'utilise pas le format « grand chiffre, légende, source » sur sa page CIED : ses chiffres sont dans des paragraphes de 14 à 15 px, avec appels de note. Le modèle du format est Resilience (n° 5).
  2. Cureety (n° 10) n'a pas de centre d'aide « activer son compte, se connecter » : c'est un formulaire de contact. Une fenêtre de choix « patient ou professionnel » s'ouvre à la première visite.
  3. Resilience (n° 5) et Implicity (n° 6) ouvrent une fenêtre « contenu réservé aux professionnels de santé » avant la page.
  4. Plusieurs sites ont changé depuis leur indexation : Heva (n° 2), Doxy.me (n° 14, titre devenu un superlatif), Fluent Health (n° 3, devenu avaros.ai). Brightlab (n° 12) montre une application patient. Institute of Health (n° 7) est un organisme de formation, sans comité scientifique.
  5. Le guide Pinterest (n° 17) conseille un accent chaud pour les CTA. Veilla garde un CTA bleu : le rouge et l'orange signalent l'alerte dans le produit.
- **Refonte du 2026-11-12** :
  - Chaque référence est triée : **11 inspirations** (n° 5, 6, 10, 17, 20, 21, 22, 23, 25, 26 et la capture mobile M1) et **19 références à côté** (n° 1, 2, 3, 4, 7, 8, 9, 11, 12, 13, 14, 15, 16, 18, 19, 24 et les captures mobiles M2, M3, M4). Rien n'est supprimé : une référence à côté garde sa ligne et sa raison, et son détail utile est cité dans le bloc concerné avec un renvoi.
  - Les captures sont rangées dans [`captures/inspis/`](captures/inspis/) et [`captures/a-cote/`](captures/a-cote/), noms et numéros inchangés.
  - Le bench est réorganisé selon l'arborescence du brief, avec un tableau de couverture.
  - **Nouvelles références (2)** pour les blocs sans inspiration : n° 25 CardiaTec (équipe et actualités datées, trouvée via One Page Love) et n° 26 Implicity, page « Clinical Evidence » (cartes d'études). Le n° 26 est le même site que le n° 6, mais une autre page et un autre usage : il a son propre numéro. Les pages de shots Dribbble affichent maintenant une vérification « Let's confirm you are human », non contournée : aucun shot n'a été ajouté (voir « Galeries : requêtes lancées »).
  - **Directions** : passées de 3 à 2. Le brief impose à tous le visuel de la direction C (tableau de bord et questionnaire sur téléphone dans le hero), et les titres en serif de la direction B sortent de la typographie du brief. Détail dans « Directions ».
  - **Token corrigé** : `text-caption` passe de 16 px à 18 px, car le brief impose un texte de 18 px minimum (sections 7, « Marque » et « Accessibilité »). Tous les autres tokens sont conformes et restent inchangés.
- **Bannières cookies** : refusées partout où un refus existait. Aucune fenêtre « je suis un professionnel de santé » n'a été validée, y compris sur la nouvelle page Implicity (n° 26) : le texte a été lu sans cliquer, et la capture montre la fenêtre.
- **Vie privée** : avatars des designers floutés sur les captures Dribbble et Awwwards. Photos de personnes présentées comme patientes ou élèves floutées (Cureety, Institute of Health). Les photos de l'équipe CardiaTec (n° 25) sont floutées aussi : le bench retient la mise en page, pas les visages.

**Répartition** : 26 références, plus 4 captures mobiles. Sites réels 7 · Dribbble 5 · Awwwards 3 · Pinterest 3 · Behance 3 (bloqués ; le n° 20 a été vu sur la page du studio) · Land-book 2 et Lapa Ninja 2 (bloqués ; les n° 3, 13 et 14 ont été vus sur le site réel) · One Page Love 1 (et la source du n° 25). Godly : aucun résultat.

---

## Couverture du brief

| Exigence du brief | Inspirations | Manque |
|---|---|---|
| 1. Hero : titre, sous-titre, deux CTA « Je suis un établissement » et « Je suis un patient », visuel tableau de bord + questionnaire sur téléphone | 10, 5 | Aucun hero vu ne montre le tableau de bord et le téléphone ensemble : Withings (n° 4) n'a pas pu être vu, avaros.ai (n° 3, à côté) est hors marque. Le visuel se valide en maquette. |
| 2. Le parcours patient en 4 étapes, illustrations simples | 23, 10, 20 | Aucune illustration au trait du parcours vue dans une palette proche. Les 4 illustrations sont à produire (livrable 5). |
| 3. Le tableau de bord soignant : capture annotée, chiffres de charge de travail | 22, 21 | Aucune capture annotée (légendes reliées à l'écran) vue sur un site réel. Le principe des fragments mis en avant vient du n° 13 (à côté). |
| 4. Preuves : cartes d'études (type, n, critère, résultat, lien), chiffres clés sourcés, logos d'établissements | 5, 26, 6 | Aucune carte vue n'affiche le n et le critère : Implicity (n° 26) donne la citation complète, pas les deux champs. Aucune rangée de logos d'établissements vue. |
| 5. Conformité et sécurité : statut DM et CE, HDS, RGPD (DPO, base légale), sécurité, liens vers les documents | 21, 5, 6 | Le statut « en cours de marquage CE » n'est vu nulle part : tous les sites vus sont déjà marqués ou certifiés. La rangée de badges sous le hero vient du n° 14 (à côté). |
| 6. Équipe médicale et comité scientifique : photos réelles, titres, liens d'intérêts déclarés | 25 | Aucun site vu ne publie les liens d'intérêts. CardiaTec (n° 25) mélange l'équipe et le comité dans un même carrousel. |
| 7. Publications et presse : liste datée, filtrable par type, CMS | 25, 26, 5 | Aucun filtre par type vu. |
| 8. Contact : formulaire établissement, bloc patient séparé (espace sécurisé, FAQ, « En cas d'urgence : 15 ») | 10 | Aucun formulaire établissement capturé, aucun rappel « 15 » vu. Les champs et les messages sont fixés par le brief (sections 6 et 9). |
| Pages annexes : FAQ patient, notice du DM, déclaration d'accessibilité | aucune | Aucune page annexe n'a été ouverte. La mention réglementaire datée de Resilience (n° 5) sert de repère pour la notice. |
| Mobile : chemin patient en premier, gros bouton « Accéder à mon espace », texte 18 px | M1 | Aucun bouton patient de 64 px vu. M2, M3 et M4 (à côté) sont des contre-exemples utiles. |
| Marque : blanc chaud, vert sauge, bleu profond, pas de rouge hors alerte | 17, 20, 10 | Aucun site vu ne combine les trois teintes. Le couple vert sombre et crème vient du n° 2, la sauge en fond d'icône du n° 24 (tous deux à côté). |
| Marque : typographie humaniste (Atkinson Hyperlegible ou Source Sans 3), 18 px minimum | aucune | Aucune référence vue n'utilise ces polices. Seul repère : le texte courant en 18 px de Cureety sur mobile (M2, à côté). |
| Accessibilité : contraste ≥ 4,5:1, niveau d'alerte = couleur + icône + texte, `prefers-reduced-motion` | 22, 23 | `prefers-reduced-motion` n'est pas observable sur une capture. Contre-exemples de contraste : n° 6, 24, 25. |
| Preuve « Moins de réhospitalisations » formulée comme objectif, résultats observationnels du pilote | 5, 26 | Aucune référence ne présente un résultat comme observationnel. Les sites vus citent des études publiées. |
| Preuve « 2 minutes par jour » (durée médiane mesurée) | aucune | Aucun site vu n'affiche une durée de questionnaire mesurée. |
| Preuve « Les alertes arrivent aux bonnes personnes » (taux d'alertes, faux positifs) | 6, 21 | Implicity (n° 6) cite une baisse des faux positifs avec appel de note, Calmedica (n° 21) un témoignage chiffré. Aucun taux d'alertes par patient vu. |
| Preuve « Conçu avec des soignants » (fondatrice, comité nommé) | 25 | Le n° 25 nomme les membres du comité, sans liens d'intérêts. |
| Preuve « Hébergé en France chez un hébergeur HDS » (nom, certificat) | 21 | Le n° 21 cite HDS et le certificat ISO 27001 avec numéro et date. |
| Preuve « en cours de marquage CE » avant obtention | aucune | Voir le bloc 5 : statut jamais vu en cours. Le format daté de Resilience (n° 5) s'adapte. |

---

## Inspirations, bloc par bloc

### 1. Hero

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 10 | Cureety, espace patient (site réel), https://www.cureety.com/en-us/patient | [choix](captures/inspis/10-cureety-patient.jpg) · [page patient](captures/inspis/10b-cureety-patient-hero.jpg) | À la première visite, deux cartes : « Patient or caregiver » (bouton vert `#487D4C`, texte blanc 4,9:1) et « Healthcare professional » (bouton bleu `#354D8C`, 8,1:1). Le codage vert pour le patient, bleu pour le soignant. À éviter : la fenêtre bloquante et le libellé « Enter ». | Les deux CTA « Je suis un patient » et « Je suis un établissement », intégrés au hero et non en fenêtre. |
| 5 | Resilience Oncology (site réel), https://www.resilience.care/healthcare-providers/oncology | [capture](captures/inspis/05-resilience-oncology.jpg) | La fenêtre « This site is intended for healthcare professionals » propose toujours une sortie vers le chemin patient (« Not a healthcare professional? Visit patients.resilience.care »). Titre serif EB Garamond 64 px `#282421` sur blanc, bouton « Request a demo » `#282421` à texte `#F4F1E9` (13,6:1). | Si les affaires réglementaires réservent une partie du contenu aux professionnels (régime de publicité des DM, section 7 du brief), le patient garde une sortie claire. Voir « Points à remonter au client ». |

Détails tirés de références à côté : la preuve courte sous le CTA du n° 1 (à reprendre seulement avec une source), les deux entrées de menu nommées par public du n° 8 (« For you », « For professionals »), le sous-titre qui dit le bénéfice soignant en une phrase du n° 3.

### 2. Le parcours patient en 4 étapes

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 23 | Medical Test Kit Website, How It Works Section, Creliq (Dribbble), https://dribbble.com/shots/26450174-Medical-Test-Kit-Website-How-It-Works-Section | [capture](captures/inspis/23-dribbble-creliq-how-it-works.jpg) | Étapes en liste verticale reliées par un filet. L'étape active est marquée par une icône sur fond vert clair **et** un trait noir, pas par la couleur seule. À gauche, un visuel qui suit l'étape. À éviter : la photo de banque d'images. | Les 4 étapes, une illustration par étape, et la règle « pas d'information portée par la seule couleur ». |
| 10 | Cureety, page patient | [page patient](captures/inspis/10b-cureety-patient-hero.jpg) | 4 étapes numérotées de 01 à 04 sur la page patient. La phrase qui rappelle que l'équipe soignante crée le compte. | Étape 1 « sortie de l'unité avec l'application activée » : dire au patient que l'unité active son accès. |
| 20 | Visilant, Transatlantico Studio (page du studio), https://transatlantico.studio/visilant/ | [capture](captures/inspis/20-transatlantico-visilant.jpg) | Identité construite sur un détail médical réel (la grille 5 × 5 des lettres de Sloan), déclinée en infographies et motion. Page en blanc chaud `#F2F0ED`. Résultat annoncé : « Increased credibility with investors and healthcare partners ». | Les illustrations simples du parcours : partir de l'échelle de douleur ou du rythme quotidien du questionnaire. |

### 3. Le tableau de bord soignant

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 22 | Remote Patient Monitoring Dashboard, Sayem (Dribbble), https://dribbble.com/shots/27191544-Remote-Patient-Monitoring-Dashboard | [capture](captures/inspis/22-dribbble-rpm-dashboard.jpg) | Rangée de 4 indicateurs (patients suivis, alertes critiques, appareils hors ligne, nouvelles alertes) avec tendance, puis un tableau patients. Statut en **pastille avec libellé** (« Critical » sur rose `#FFDCDC`, « Stable » sur vert d'eau, « Warning » sur ambre `#F3BA5B`). Noms fictifs. À éviter : la courbe colorée sans libellé et le rouge répété partout. | La capture annotée (liste des patients, niveau d'alerte, historique) et le niveau d'alerte en couleur + icône + texte. |
| 21 | Calmedica, télésuivi patient (site réel, FR), https://calmedica.com/ | [capture](captures/inspis/21-calmedica.jpg) · [chiffres](captures/inspis/21b-calmedica-chiffres.jpg) | Témoignage d'une cadre de chirurgie ambulatoire : « on ne passe plus que 1 ou 2 appels par jour ». À éviter : ses grands chiffres sans source. | Les chiffres sur la charge de travail, portés par une paire (persona Claire). |

Détails tirés de références à côté : montrer des fragments de l'interface mis en avant par un contour plutôt qu'un écran entier illisible (Canvas, n° 13) ; poser la capture en carte arrondie sur un fond doux, sans cadre de navigateur (Brightlab, n° 12).

### 4. Preuves

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 5 | Resilience Oncology | [capture](captures/inspis/05-resilience-oncology.jpg) | Le meilleur bloc preuves du panel : 4 grands chiffres (« +5,2 Months in overall survival », « +1,9 Months of treatment duration », « +88 % », « -25 % severe toxicities »), chacun avec appel de note, et un lien « See sources » (Basch, JCO 2017 ; Basch et al., JAMA 2022 ; Mir et al., 2020 ; Patt, 2023). | Chiffres clés sourcés, et la règle « chaque chiffre affiché a une source et une date » (section 13). |
| 26 | Implicity, Clinical Evidence (site réel, ajout), https://implicity.com/clinical-evidence/ | [chiffres](captures/inspis/26-implicity-clinical-evidence.jpg) · [études](captures/inspis/26b-implicity-etudes.jpg) | En haut, 4 cartes chiffrées (« 26% reduction in mortality », « up to 76% fewer false-positive ILR episodes », « 35 days », « 300+ hours saved per year at 200 patients »), chiffres en Montserrat 66 px graisse 900, chacun avec appel de note. Puis des **cartes d'études** : nom de l'étude (« EVIDENCE-RM STUDY »), étiquette revue et année (« HEART RHYTHM · 2024 ») ou « PDF », titre, citation complète, lien « Read More ». À éviter : les étiquettes en 10 à 11 px, et le « up to ». | Les cartes d'études (type, résultat, lien). Il faut ajouter le n et le critère, absents ici. |
| 6 | Implicity, CIED Remote Monitoring (site réel), https://implicity.com/cied-remote-monitoring/ | [capture](captures/inspis/06-implicity-cied.jpg) | Chaque chiffre (-79 % de faux positifs, -85 % d'alertes FA inutiles, 28 % de patients reconnectés) a un appel de note vers une référence publiée. À éviter : ces chiffres noyés dans des paragraphes de 14 à 15 px, et le bouton « Request a demo » blanc sur `#2B8F9C` (3,8:1, sous le seuil AA). | Preuve « Les alertes arrivent aux bonnes personnes » : un taux de faux positifs avec sa source. |

Logos d'établissements : aucune référence retenue. Rappel du brief : aucun logo sans accord écrit.

### 5. Conformité et sécurité

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 21 | Calmedica | [chiffres](captures/inspis/21b-calmedica-chiffres.jpg) | Bloc sécurité exemplaire : ISO 27001 avec organisme, numéro et date du certificat (29 octobre 2025), HDS, RGPD avec DPO. | HDS, RGPD (DPO), sécurité (ISO 27001 si visé), chaque certification liée à son document. |
| 5 | Resilience Oncology | [capture](captures/inspis/05-resilience-oncology.jpg) | En pied de page : « Class IIa medical device », « CE 0459 », « reimbursed by the French Assurance Maladie », « Update : March 2026 ». | Statut DM et CE, en mention datée. Avant obtention, la même ligne dit « en cours de marquage CE ». |
| 6 | Implicity, CIED | [capture](captures/inspis/06-implicity-cied.jpg) | Les notes de bas de page donnent le statut réglementaire de chaque module (classe, marquage CE ou FDA). | Un statut exact par fonctionnalité, si l'algorithme et l'application n'ont pas le même statut. |

Détail tiré d'une référence à côté : la rangée de badges de conformité sous le hero (« HIPAA-compliant », « SOC 2-certified », « GDPR-compliant ») de Doxy.me (n° 14).

### 6. Équipe médicale et comité scientifique

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 25 | CardiaTec Biosciences (site réel, ajout, trouvé via One Page Love), https://cardiatec.ai/ | [équipe](captures/inspis/25-cardiatec-equipe.jpg) | Section « Team » : photos réelles traitées toutes en noir et blanc, en grille de 6, nom et fonction sous chaque photo, lien LinkedIn. Les membres du comité scientifique sont nommés et étiquetés « SAB Member ». À éviter : le comité mélangé à l'équipe dans un carrousel à flèches, et les noms et fonctions en 14 px, `#09155A` à 50 % d'opacité (≈ 3,4:1 sur blanc). | Photos réelles, titres, comité nommé (preuve « Conçu avec des soignants »). Pour Veilla : le comité dans un bloc à part, avec les liens d'intérêts déclarés sous chaque nom. |

### 7. Publications et presse

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 25 | CardiaTec Biosciences | [actualités](captures/inspis/25b-cardiatec-actualites.jpg) | Section « News » : liste de 6 entrées sur 2 rangées, la date complète au-dessus du titre (« 19 March 2026 », 13 px), le titre en 20 px avec les mots clés en gras, une entrée « New publication selected for the Nature Portfolio ». Puis une rangée de logos presse en gris. À éviter : la date trop petite, le carrousel, et le superlatif « World-Leading » dans un titre. | La liste datée, alimentée par le CMS. Il faut ajouter le filtre par type, absent ici. |
| 26 | Implicity, Clinical Evidence | [études](captures/inspis/26b-implicity-etudes.jpg) | L'étiquette de type et de source sur chaque carte (« HEART RHYTHM · 2024 », « PDF »), et le lien vers le document. | Le type de chaque publication, qui sert de base au filtre. |
| 5 | Resilience Oncology | [capture](captures/inspis/05-resilience-oncology.jpg) | Rubrique « Latest Publications » et lien « Scientifics publications ». | CTA « Voir toutes les publications ». |

### 8. Contact

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 10 | Cureety, page patient | [page patient](captures/inspis/10b-cureety-patient-hero.jpg) | Le bloc **aidants** (« Report symptoms on their behalf »), les boutons « Contact us » (`#565269`, 7,5:1) et « Ask a question », la phrase qui dit que l'équipe soignante crée le compte. À éviter : « 94 % of patients feel more supported… » sans source visible. | Le bloc patient séparé : Sophie peut agir pour sa mère, et le patient sait qu'il n'a pas de compte à créer. |

Formulaire établissement et rappel « En cas d'urgence : 15 » : aucune référence. Le contenu est déjà fixé par le brief (champs en section 6, messages en section 9).

### Marque (transverse)

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 17 | A Color Palette for a Medical Website That Feels Trustworthy, Not Icy (Pinterest, guide), https://guide.pinterest.com/design/color-palette-for-medical-website/ | [capture](captures/inspis/17-pinterest-guide-palette.jpg) | Base neutre, un bleu dominant, le vert en second pour les signaux de soutien (succès, badges, séparateurs). Une palette tout en vert et blanc ferait penser aux compléments alimentaires. Neutres chauds (« Champagne and Oxford Blue », « Eggshell ») contre l'éblouissement du blanc pur. Veilla ne suit pas son conseil d'accent chaud pour les CTA. | Blanc chaud, vert sauge, bleu profond, et le partage des rôles entre bleu (action) et sauge (soutien). |
| 20 | Visilant | [capture](captures/inspis/20-transatlantico-visilant.jpg) | Blanc chaud `#F2F0ED` en fond, bleu nuit pour le hero. Une jeune marque qui annonce un gain de crédibilité auprès des investisseurs et des partenaires de santé. | Blanc chaud, ton calme, et le déclencheur « levée de série A » (section 2). |
| 10 | Cureety | [choix](captures/inspis/10-cureety-patient.jpg) | Vert pour le patient, bleu pour le soignant. | Sauge foncée pour le chemin patient, bleu profond pour l'établissement. |

Détails tirés de références à côté : le couple vert olive `#39442B` et crème `#FDFDF1` de Heva (n° 2, boutons à 10,1:1), la sauge réservée aux fonds d'icônes chez Carely (n° 24).

### Accessibilité (transverse)

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 22 | RPM Dashboard, Sayem | [capture](captures/inspis/22-dribbble-rpm-dashboard.jpg) | Pastille de statut avec libellé. | Niveau d'alerte = couleur + icône + texte. |
| 23 | Creliq, How It Works | [capture](captures/inspis/23-dribbble-creliq-how-it-works.jpg) | Étape active marquée par un trait, pas seulement par la couleur. | Pas d'information portée par la seule couleur. |

Contre-exemples à garder en tête : le bouton à 3,8:1 d'Implicity (n° 6), le mot du titre en sauge pâle de Carely (n° 24, à côté), les noms à ≈ 3,4:1 de CardiaTec (n° 25), l'animation d'entrée qui cache le titre de Calmedica (n° 21).

---

## Mobile

Exigences du brief : chemin « Je suis un patient » en premier sur mobile, gros bouton « Accéder à mon espace », texte 18 px minimum, cibles tactiles ≥ 44 × 44 px, Core Web Vitals mobiles. Les captures sont en 390 × 844 px.

| # | Référence | Capture | Observation | Exigence du brief |
|---|---|---|---|---|
| M1 | Cureety, choix du public (inspiration) | [capture](captures/inspis/mobile-cureety-choix.jpg) | La carte **patient passe en premier**, avec un bouton vert pleine largeur (276 × 48 px). La carte soignant suit, bouton bleu. Libellés « Enter » en 14 px. | Patient en premier. Veilla va plus loin : 64 px de haut, libellé explicite en 20 px (« Je suis un patient »). |
| M2 | Cureety, page patient (à côté) | [capture](captures/a-cote/mobile-cureety.jpg) | Texte courant en 18 px, titre fin sur 2 lignes. Deux boutons côte à côte (118 × 48 et 127 × 48 px, libellés en 14 px). Le bouton de connexion est caché dans le menu. | Le 18 px est le bon repère. « Accéder à mon espace » reste visible sans ouvrir le menu. |
| M3 | Resilience Oncology (à côté) | [capture](captures/a-cote/mobile-resilience.jpg) | La fenêtre « professionnels de santé » ne s'est pas affichée sur mobile (présente dans la page, mais masquée). Titre serif centré sur 3 lignes, un seul CTA « Request a demo ». | Si Veilla filtre un contenu pro, le filtre marche aussi sur mobile, ou n'existe pas. |
| M4 | Doxy.me (à côté) | [capture](captures/a-cote/mobile-doxy-me.jpg) | Titre en 52 px sur 4 lignes, CTA qui n'arrivent qu'à 474 px du haut. Deux CTA côte à côte de **37 px de haut**. | Sous la cible tactile de 44 px. Le `text-display` de Veilla passe à 36 px sur mobile pour faire monter le CTA patient. |

Poids de page et LCP : non mesurés sur les références.

---

## Directions

Le brief ne fixe pas de nombre de pistes. Il impose en revanche le visuel du hero (« capture du tableau de bord et du questionnaire sur téléphone ») et la typographie (Atkinson Hyperlegible ou Source Sans 3). Deux pistes restent.

- **Direction C « Produit au premier plan » retirée comme piste à part** : son trait distinctif, le hero en split téléphone et tableau de bord, est imposé par le brief aux deux pistes. Sa référence principale (Withings, n° 4) n'a pas pu être vue. La démo animée du trajet d'une alerte devient une option des deux pistes, avec une version en 4 images fixes pour `prefers-reduced-motion`.
- **Titres en serif (Source Serif 4) retirés de la direction B** : le brief demande une typographie humaniste, Atkinson Hyperlegible ou Source Sans 3.

### Direction A : « Clinique chaleureuse » (recommandée)
- Blanc chaud dominant, bleu profond pour les titres et les CTA, sauge pour les fonds de section et les badges de conformité (guide n° 17, Visilant n° 20).
- Choix du public dans le hero : « Je suis un patient » en sauge foncée, « Je suis un établissement » en bleu profond, comme le codage de Cureety (n° 10). Sur mobile, la carte patient passe en premier (M1).
- Hero en split : questionnaire sur téléphone et tableau de bord. Captures en cadres arrondis, fragments mis en avant (n° 22 ; principe du n° 13, à côté), statut en pastille avec libellé (n° 22).
- Parcours en liste verticale de 4 étapes illustrées au trait, étape active marquée par la forme (n° 23, n° 10).
- Conformité : badges sauge, certifications avec organisme, numéro et date (n° 21), mention réglementaire datée en pied de page (n° 5).

### Direction B : « Éditorial scientifique »
- Grille éditoriale, titres en Source Sans 3 700, chiffres en très grand avec appel de note et lien « Voir les sources » (n° 5, n° 26).
- Preuves et Publications deviennent la colonne vertébrale : cartes d'études avec type, n, critère, résultat et lien (n° 26), liste datée et filtrable (n° 25), équipe et comité en grille de portraits homogènes (n° 25).
- Fond blanc chaud et texte généreux pour ne pas paraître distant (Resilience, n° 5). Le bloc patient garde la même clarté que dans la direction A.
- Même hero en split que la direction A, imposé par le brief.

---

## Palette, polices, design tokens, composants

Toutes les valeurs ont été vérifiées contre le brief : palette (blanc chaud, sauge, bleu profond, rouge réservé aux alertes), polices (Atkinson Hyperlegible, Source Sans 3), texte 18 px minimum, contraste ≥ 4,5:1, cibles ≥ 44 px, niveau d'alerte en couleur + icône + texte. Une seule correction : `text-caption` passe de 16 à 18 px.

### Palette recommandée (contrastes calculés sur #FAF8F4)

| Rôle | Hex | Usage | Contraste |
|---|---|---|---|
| Fond blanc chaud | `#FAF8F4` | Fond principal | Fond de référence |
| Texte | `#1E2A33` | Corps de texte | 13,8:1 |
| Bleu profond | `#1F3A5F` | Titres, CTA principal (texte blanc : 11,5:1) | 10,8:1 |
| Sauge foncée | `#4E6B57` | Liens secondaires, icônes, badges | 5,6:1 (AA) |
| Sauge | `#7A9A82` | Décor, illustrations uniquement | 2,9:1 (**jamais pour le texte**) |
| Sauge pâle | `#E3EBE4` | Fonds de section | texte #1E2A33 : 12,0:1 |
| Alerte | `#B3261E` | **Uniquement** pour les alertes dans l'interface montrée et les erreurs de formulaire | 6,2:1 |

Les sites observés confirment le blanc chaud (`#F2F0ED` à `#FDFDF1` chez Visilant, Institute of Health, Heva) et un vert sombre pour l'action (Heva, Cureety).

### Polices (Google Fonts)
- **Atkinson Hyperlegible** : corps de texte et interface, 18 px minimum (20 px pour le bloc patient).
- **Source Sans 3** : titres (graisses 600 et 700), dans les deux directions.

### 3 « à ne pas faire »
1. **Du rouge ou de l'orange vif pour les CTA** : le rouge signifie « alerte » dans le produit, il ne doit pas apparaître ailleurs. Le guide n° 17 conseille l'inverse ; Canvas (n° 13) et Calmedica (n° 21) le font.
2. **Des photos de banque d'images de médecins ou de patients souriants** : préférer l'équipe réelle, des captures et des illustrations. Le motif est partout dans les shots Dribbble (n° 1, 23, 24).
3. **Du texte gris clair ou sauge sur fond blanc cassé** pour faire « doux » : la cible patient âgée exige un contraste ≥ 4,5:1 partout. Implicity (n° 6) a un bouton à 3,8:1, Carely (n° 24) un mot du titre en sauge pâle, CardiaTec (n° 25) des noms à ≈ 3,4:1.

### Design tokens

> Format design system. Noms en kebab-case, prêts pour des variables CSS. Contrastes calculés sur `#FAF8F4` (revérifiés le 2026-11-12).

#### Couleurs

**Marque**

| Token | Hex | Usage |
|---|---|---|
| `color-brand-primary` | `#1F3A5F` | CTA principal, titres (10,8:1 ; texte blanc 11,5:1) |
| `color-brand-primary-hover` | `#162B47` | Survol et état pressé (13,5:1 ; texte blanc 14,3:1) |
| `color-brand-primary-light` | `#2D5A8A` | Liens (6,7:1) |
| `color-brand-secondary` | `#4E6B57` | Badges de conformité, icônes, liens secondaires (5,6:1) |
| `color-brand-secondary-strong` | `#3F5E49` | Fond du CTA patient (texte blanc 7,2:1) |
| `color-brand-secondary-soft` | `#7A9A82` | Décor et illustrations uniquement (2,9:1) |
| `color-brand-secondary-tint` | `#E3EBE4` | Fonds de section (texte #1E2A33 : 12,0:1) |

**Sémantiques** (toujours couleur + icône + libellé)

| Token | Hex | Contraste | Remarque |
|---|---|---|---|
| `color-success` | `#2E6B47` | 6,0:1 | Statut « conforme », envoi réussi |
| `color-alert` | `#B3261E` | 6,2:1 | **Seul rouge autorisé** : alertes patient dans les captures et erreurs de formulaire (section 9 du brief) |
| `color-warning` | `#8A5A00` | 5,6:1 | Alerte modérée (niveau orange du tableau de bord), statut « en cours » |
| `color-info` | `#1F5F8B` | 6,5:1 | Encadrés d'information (« En cas d'urgence, appelez le 15 ») |

**Neutres**

| Token | Hex | Usage |
|---|---|---|
| `color-neutral-0` | `#FFFFFF` | Cartes, champs |
| `color-neutral-50` | `#FAF8F4` | Fond de page (blanc chaud) |
| `color-neutral-100` | `#EEEAE3` | Fonds alternés |
| `color-neutral-300` | `#D6D0C6` | Séparateurs décoratifs (1,5:1, pas pour les bordures de champs) |
| `color-neutral-600` | `#5A6670` | Texte secondaire, bordures de champs (5,6:1) |
| `color-neutral-900` | `#1E2A33` | Texte principal (13,8:1) |

#### Échelle typographique (base 18 px, ratio ≈ 1,25)

| Token | Police | Taille | Graisse | Interlignage |
|---|---|---|---|---|
| `text-display` | Source Sans 3 | 52 px (mobile 36) | 700 | 1,1 |
| `text-h1` | Source Sans 3 | 40 px (mobile 32) | 700 | 1,2 |
| `text-h2` | Source Sans 3 | 32 px (mobile 26) | 600 | 1,25 |
| `text-h3` | Source Sans 3 | 24 px | 600 | 1,3 |
| `text-stat` | Source Sans 3 | 56 px (mobile 40) | 700 | 1,0 (grands chiffres de la section Preuves) |
| `text-body-lg` | Atkinson Hyperlegible | 20 px | 400 | 1,6 (bloc patient) |
| `text-body` | Atkinson Hyperlegible | 18 px | 400 | 1,6 |
| `text-label` | Atkinson Hyperlegible | 18 px | 700 | 1,4 |
| `text-caption` | Atkinson Hyperlegible | **18 px** (corrigé, était 16 px) | 400 | 1,5 (sources des chiffres, mentions ; se distingue du corps par la couleur `color-neutral-600`) |

Repère observé : Doxy.me met son titre en 52 px sur mobile, sur 4 lignes, et ses CTA n'arrivent qu'à 474 px du haut (M4). Le `text-display` de Veilla passe à 36 px sur mobile pour laisser monter le CTA patient.

#### Espacements (base 8 px)

`space-1` 4 · `space-2` 8 · `space-3` 12 · `space-4` 16 · `space-5` 24 · `space-6` 32 · `space-7` 48 · `space-8` 64 · `space-9` 96 · `space-10` 128 (entre sections, desktop) · gouttière mobile : 16 px.

#### Rayons

`radius-sm` 4 px (badges, champs) · `radius-md` 8 px (boutons) · `radius-lg` 16 px (cartes, captures) · `radius-full` 999 px (avatars de l'équipe).

#### Ombres (teintées bleu nuit)

- `shadow-sm` : `0 1px 2px rgba(30, 42, 51, 0.06)`
- `shadow-md` : `0 4px 16px rgba(30, 42, 51, 0.08)` (cartes de preuve)
- `shadow-lg` : `0 16px 40px rgba(30, 42, 51, 0.12)` (captures du tableau de bord, mockups)
- `focus-ring` : `0 0 0 3px #FAF8F4, 0 0 0 6px #2D5A8A`

#### Motion

| Token | Valeur | Usage |
|---|---|---|
| `duration-fast` | 120 ms | Survol, focus |
| `duration-base` | 200 ms | Accordéons (FAQ, conformité) |
| `duration-slow` | 400 ms | Apparition de l'alerte dans la démo du parcours (option des deux directions) |
| `ease-standard` | `cubic-bezier(0.2, 0, 0, 1)` | Par défaut |
| `ease-emphasized` | `cubic-bezier(0.3, 0, 0, 1.0)` | Entrées de mockups |
| `ease-exit` | `cubic-bezier(0.4, 0, 1, 1)` | Sorties |

`prefers-reduced-motion: reduce` : durées à 0 ms, la démo animée est remplacée par 4 images statiques numérotées. Le titre du hero n'est jamais animé à l'entrée : il doit être visible même si le script ne se lance pas (contre-exemple : Calmedica, n° 21).

### Composants clés

#### Choix du public (hero)
- Deux cartes côte à côte sur desktop, empilées sur mobile avec **la carte patient en premier** (modèle : Cureety, n° 10 et M1).
- Carte patient : bouton `color-brand-secondary-strong` « Je suis un patient ». Carte établissement : bouton `color-brand-primary` « Je suis un établissement ». Libellés explicites, jamais « Entrer ».
- Intégré au hero, pas en fenêtre bloquante : le visiteur voit la promesse avant de choisir. Si un contenu doit être réservé aux professionnels, la fenêtre de filtre propose toujours une sortie claire vers le chemin patient, comme Resilience (n° 5), et marche aussi sur mobile (M3).

#### Bouton primaire (« Demander une présentation », « Je suis un établissement »)
- Fond `color-brand-primary`, texte blanc `text-label`, hauteur 52 px (56 px sur mobile), padding horizontal 24 px, `radius-md`.
- **États** : *repos* #1F3A5F · *survol* #162B47 · *focus* `focus-ring` · *pressé* #162B47 et translation de 1 px · *désactivé* fond #D6D0C6, texte #5A6670, raison affichée · *chargement* : spinner et « Envoi en cours… ».

#### Bouton patient (« Je suis un patient », « Accéder à mon espace patient »)
- Fond `color-brand-secondary-strong` #3F5E49, texte blanc 20 px, hauteur **64 px** sur mobile, pleine largeur. Premier bouton sur mobile, visible sans ouvrir le menu (contre-exemple : M2).
- Repère observé : Cureety fait 48 px de haut avec un libellé de 14 px (M1). Veilla vise plus grand pour des patients âgés.

#### Bouton secondaire (« Voir toutes les publications »)
- Transparent, bordure 2 px #1F3A5F, texte #1F3A5F. *Survol* fond #E3EBE4 · *focus* `focus-ring` · *désactivé* opacité 60 % et raison affichée.

#### Carte de preuve
- Fond blanc, `radius-lg`, `shadow-md`, padding `space-6`. Contenu : un chiffre en `text-stat`, une légende en `text-body`, puis **obligatoirement** une ligne `text-caption` « Source : [étude], n = [x], [date] » avec un lien. Tant qu'aucune étude n'est publiée, la carte dit « résultats observationnels du pilote ».
- Modèles observés : Resilience (n° 5), appel de note sur chaque chiffre et lien « Voir les sources » ; Implicity (n° 26), étiquette de type et citation complète. Contre-exemples : Calmedica (n° 21), Institute of Health (n° 7), Cureety (« 94 % », n° 10).

#### Carte d'étude et de publication
- Étiquette de type (« Étude observationnelle », « Poster », « Presse ») en `text-label`, date complète, titre en `text-h3`, puis n, critère, résultat et lien vers le document. Même carte pour la section Publications, avec un filtre par type au-dessus de la liste.
- Modèles observés : Implicity (n° 26) pour l'étiquette et la citation, CardiaTec (n° 25) pour la date au-dessus du titre. Les étiquettes restent à 18 px, pas à 10 ou 13 px.

#### Portrait de l'équipe et du comité
- Photo réelle, traitement homogène, nom en `text-label`, titre en `text-body`, contraste plein (pas d'opacité réduite). Pour le comité scientifique, une ligne « Liens d'intérêts : [déclaration] » avec un lien.
- Modèle observé : CardiaTec (n° 25), en séparant l'équipe et le comité.

#### Badge de conformité
- Pastille `radius-sm`, fond #E3EBE4, icône et texte #3F5E49 (5,9:1) (« Hébergeur certifié HDS », « RGPD »). Un statut en cours s'affiche en style warning : « Marquage CE : en cours ».
- Une rangée de badges sous le hero (détail de Doxy.me, n° 14, à côté). Dans la section Conformité, chaque certification porte son organisme, son numéro et sa date, comme Calmedica (n° 21).

#### Mention réglementaire (pied de page)
- Une ligne `text-caption` sous le pied de page : statut du DM, classe, numéro de l'organisme notifié une fois obtenu, fabricant, date de mise à jour. Modèle : Resilience (« Class IIa medical device… CE 0459… Update : March 2026 »). Avant le marquage : « Logiciel en cours de marquage CE ».

#### Formulaire établissement
- Champs : nom, établissement, fonction, e-mail professionnel, téléphone (facultatif), message (facultatif). Libellés au-dessus, champs de 52 px, bordure 2 px #5A6670.
- Aucune donnée de santé. Une mention le rappelle à côté du formulaire (« Patients : n'indiquez aucune information médicale ici »).
- Erreurs sous le champ, reliées par `aria-describedby`, icône et texte en `color-alert` (section 9 du brief).

#### À faire / À ne pas faire

| À faire | À ne pas faire |
|---|---|
| Chaque chiffre accompagné de sa source, son n et sa date | Grands chiffres sans légende ni source (Calmedica, Institute of Health) |
| Rouge réservé aux alertes (captures et erreurs) | Rouge ou orange vif pour les CTA ou la décoration |
| Statut réglementaire exact (« en cours » si c'est en cours) | « Certifié », « remboursé » par anticipation |
| Mention réglementaire datée en pied de page | Statut du DM introuvable sur le site |
| Niveau d'alerte = couleur + icône + texte | Pastille de couleur seule |
| CTA patient en premier et pleine largeur sur mobile | Deux CTA côte à côte de 40 px sur mobile (Doxy.me : 37 px) |
| Choix du public visible dans le hero, avec sortie vers le chemin patient | Fenêtre bloquante sans sortie pour le patient |
| Titre du hero visible sans attendre une animation | Intro vidéo ou animation qui masque le titre |
| Captures avec des données fictives clairement anonymisées | Captures avec de vrais noms de patients, même floutés |
| Libellés visibles au-dessus des champs | Placeholders utilisés comme libellés |
| Liens d'intérêts sous chaque membre du comité | Comité mélangé à l'équipe, sans déclaration |

---

## À côté

| # | Référence | Capture | Pourquoi à côté |
|---|---|---|---|
| 1 | Medical Website Design (Hero Section), Isfak Sarder (Dribbble), https://dribbble.com/shots/19190049-Medical-Website-Design-Hero-Section | [capture](captures/a-cote/01-dribbble-isfak-hero.jpg) | Photo de banque d'images d'un médecin, chiffres sans source (« 2,491 Happy Customers », « 4.9/5 Rating ») et jaune vif `#F3D348` : enfreint l'interdit « chiffres sans source » et la palette du brief. Seul détail retenu : la preuve courte sous le CTA (bloc 1). |
| 2 | Heva Health, Site of the Day 26/07/2024 (Awwwards), https://www.awwwards.com/sites/heva-health | [capture](captures/a-cote/02-awwwards-heva-health.jpg) · [site](captures/a-cote/02b-heva-site.jpg) | Ton bien-être hors du ton « calme, factuel » du brief, fenêtre d'inscription « 30 % off » dès l'arrivée, « 4.9/5 from 12,000+ successful consultations » sans source (interdit). Seul détail retenu : le couple olive `#39442B` et crème `#FDFDF1` (Marque). |
| 3 | Fluent Health, devenu avaros.ai (Lapa Ninja bloqué, site réel), https://avaros.ai/ | [capture](captures/a-cote/03-fluent-avaros.jpg) | Thème sombre `#051023` et vert fluo `#BFFF99` : hors palette (blanc chaud, sauge, bleu profond). Seul détail retenu : le sous-titre qui dit le bénéfice soignant en une phrase (bloc 1). |
| 4 | Withings Health Solutions, Remote Patient Monitoring, https://www.withings.com/us/en/health-solutions/remote-patient-monitoring | Aucune | Non vérifié : challenge Cloudflare, non contourné. |
| 7 | Institute of Health, Honorable Mention 05/02/2026 (Awwwards), https://www.awwwards.com/sites/institute-of-health | [capture](captures/a-cote/07-awwwards-institute-of-health.jpg) · [site](captures/a-cote/07b-institute-of-health-site.jpg) | Organisme de formation, pas de comité scientifique. Superlatifs (« Global leaders », « The only… ») et chiffres sans source (966, 46, 22) : enfreint les interdits du brief. Détail possible : la colonne de chiffres à filets fins, à n'utiliser qu'avec des sources. |
| 8 | MyHealthPrac, Site of the Day 11/07/2025 (Awwwards), https://www.awwwards.com/sites/myhealthprac | [capture](captures/a-cote/08-awwwards-myhealthprac.jpg) · [site](captures/a-cote/08b-myhealthprac-site.jpg) | Ton grand public (« See Beyond. Unlock Your Health », « Join Waitlist »), texte blanc sur photo au contraste variable : contraire à la règle des 4,5:1. Seul détail retenu : deux entrées de menu nommées par public (bloc 1). |
| 9 | Medtech, Healthcare Service Landing Page, MultiQoS (Behance), https://www.behance.net/gallery/182360867/Medtech-Healthcare-Service-Landing-Page | Aucune | Non vérifié : erreur HTTP 400. Remplacé par le n° 23. |
| 11 | Real-Time Patient Monitoring Dashboard, MD Jubaer Riyad (Behance), https://www.behance.net/gallery/213693587/Real-Time-Patient-Monitoring-Dashboard-UXUI-Design | Aucune | Non vérifié : erreur HTTP 400. Remplacé par le n° 22. |
| 12 | Medical Web Application, Brightlab (Dribbble), https://dribbble.com/shots/23641909--Medical-Web-Application-Changing-Healthcare-with-Web-App | [capture](captures/a-cote/12-dribbble-brightlab-medical-webapp.jpg) | Application patient commerciale (réductions, blog), fond lavande et accents violets (couleurs estimées à l'œil) : hors palette, et pas un tableau de bord soignant. Seul détail retenu : la capture posée en carte sans chrome de navigateur (bloc 3). |
| 13 | Canvas Medical (Lapa Ninja bloqué, site réel), https://www.canvasmedical.com/ | [capture](captures/a-cote/13-canvas-medical.jpg) | Thème sombre `#030B14`, dégradé bordeaux et CTA orange `#FB923C` : hors palette, et l'orange est réservé aux alertes. Seul détail retenu : les fragments d'interface mis en avant par un contour (bloc 3). |
| 14 | Doxy.me (Land-book bloqué, site réel), https://doxy.me/site/ | [capture](captures/a-cote/14-doxy-me.jpg) | Titre superlatif « The world's most loved telehealth platform » (interdit du brief). La formule « No patient login » ne s'applique pas : Veilla a un espace patient. Seul détail retenu : la rangée de badges de conformité sous le hero (bloc 5). |
| 15 | Medical Website Examples, 29 sites (One Page Love), https://onepagelove.com/tag/medical | [capture](captures/a-cote/15-onepagelove-medical.jpg) | Contexte seulement : une galerie de comparaison, pas un élément précis. Elle a servi à trouver le n° 25. |
| 16 | Carbon Health (Land-book), https://land-book.com/websites/14601-carbon-health-modern-primary-urgent-care | Aucune | Non vérifié : Land-book et carbonhealth.com bloqués par Cloudflare. |
| 18 | Sage Organic Branding, dental clinic (Pinterest), https://www.pinterest.com/pin/wellness-branding-and-squarespace-design-for-organic-dental-clinic--609534130826660036/ | Aucune | Non vérifié : mur de connexion. Le texte alternatif décrit un logo vert et blanc ; l'image entrevue est vert d'eau, pas sauge. |
| 19 | Healthcare webdesign homepage green hex colors (Pinterest), https://www.pinterest.com/pin/816699713670139085/ | Aucune | Non vérifié visuellement (mur de connexion). Nuancier générique (`#b2dabc`, `#add4c5`…), pas une page santé. La règle reste : tons pâles pour les fonds, jamais pour le texte. |
| 24 | Carely, Modern Healthcare Landing Page, Peter Jackson (Dribbble), https://dribbble.com/shots/27709011-Carely-Modern-Healthcare-Landing-Page | [capture](captures/a-cote/24-dribbble-carely-sage.jpg) | Mot du titre en sauge pâle (contraste insuffisant), photo de médecin souriant, chiffres sans source (20k+, 98 %) : enfreint le contraste de 4,5:1 et l'interdit « chiffres sans source ». Seul détail retenu : la sauge réservée aux fonds d'icônes (Marque). |
| M2 | Cureety, page patient, mobile | [capture](captures/a-cote/mobile-cureety.jpg) | Connexion cachée dans le menu, boutons côte à côte avec libellés en 14 px : contraire au « gros bouton Accéder à mon espace » du brief. Seul détail retenu : le texte courant en 18 px (Mobile). |
| M3 | Resilience Oncology, mobile | [capture](captures/a-cote/mobile-resilience.jpg) | Contre-exemple : la fenêtre « professionnels de santé » ne s'affiche pas sur mobile. |
| M4 | Doxy.me, mobile | [capture](captures/a-cote/mobile-doxy-me.jpg) | Contre-exemple : CTA de 37 px de haut, sous la cible tactile de 44 px du brief. |

---

## Points à remonter au client

- **Contenu réservé aux professionnels** : Resilience (n° 5) et Implicity (n° 6 et 26) affichent leurs chiffres cliniques derrière une fenêtre « réservé aux professionnels de santé ». Le brief demande de vérifier le régime de publicité des DM auprès de l'ANSM, mais ne dit pas si la section Preuves peut être vue par les patients. La réponse change le hero et le parcours patient : à trancher avec les affaires réglementaires avant les wireframes (S2).
- **Liens d'intérêts** : aucun site vu ne les publie. Le format (déclaration publique, lien vers la base Transparence Santé, texte libre) est à fixer avec la direction médicale.

---

## Galeries : requêtes lancées

| Date | Galerie | Requête ou page | Résultat |
|---|---|---|---|
| 2026-11-12 | Dribbble | Recherche « scientific advisory board » | Résultats hors sujet (conseil d'entreprise, logos). Rien de retenu. |
| 2026-11-12 | Dribbble | Recherche « medical team section » | Pistes : « DocuVerse, Medical Team & Contact Page UI », « Dental Specialists Section ». Pages des shots bloquées par « Let's confirm you are human », non contourné. |
| 2026-11-12 | Dribbble | Recherches « healthcare publications », « research publications page » | Couvertures de livres, applications. Une piste (« RAI Institute insights ») bloquée par la même vérification. |
| 2026-11-12 | One Page Love | Tag « medical » (n° 15), fiches Eigen Therapeutics, Aether Bio, TelMD, CardiaTec | CardiaTec a des sections « Team » et « News » : retenu (n° 25). Eigen : biotech de découverte de médicaments, non approfondi. Aether Bio : thème sombre. TelMD : site hors ligne. |
| 2026-11-12 | Site réel | implicity.com, lien « Clinical Evidence » (implicity.com/publications renvoie une 404) | Cartes d'études et chiffres avec notes : retenu (n° 26). |
| 2026-11-12 | Behance, Land-book, Lapa Ninja, Pinterest | Non réessayés (consigne) | Bloqués lors de la vérification : erreur 400, Cloudflare, mur de connexion. |
| 2026-11-12 (vérification) | Godly | Recherche santé | Aucun résultat. |
