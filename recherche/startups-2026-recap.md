# Recap : startups, scale-ups et PME qui se lancent le plus (France, fin octobre 2026)

Objectif : repérer les secteurs et entreprises en croissance pour leur proposer des sites vitrines.

> Les données viennent de recherches web (résumés de Maddyness, Les Pépites Tech / Eldorado, FrenchWeb, Licorne Society, INSEE, Crunchbase). Les totaux varient d'une source à l'autre, car chaque média compte sur un périmètre différent. Vérifie chaque entreprise (site actuel, contact) avant de la démarcher.

## 1. Le contexte en chiffres

- **France, S1 2026** : environ 5 Md€ levés (meilleur semestre depuis 4 ans, +40 %), mais **moins d'opérations** (257). L'argent se concentre : les 10 plus grosses levées font environ 49 % du total.
- **Septembre 2026** : 3,29 Md€, dont environ 3 Md€ pour la seule levée de Mistral AI (série D).
- **Octobre 2026** : de 41 à 270 M€ par semaine, avec 8 à 15 opérations par semaine, en majorité en seed ou série A.
- **IA** : présente dans environ 35 % des levées françaises, et dans 64 % des montants investis dans le monde au T3 2026 (Crunchbase, 159 Md$ au total).
- **Création d'entreprises (INSEE, sept. 2026)** : forte hausse sur un an. Les plus gros contributeurs sont les **services aux entreprises** (+12 400, dont le nettoyage de bâtiments), le **commerce** (+10 700) et l'**information-communication** (+10 000).

## 2. Les domaines qui se lancent le plus, et pourquoi

| Domaine | Pourquoi ça explose | Exemples 2026 |
|---|---|---|
| **IA appliquée / agents IA (B2B)** | Les investisseurs financent l'IA « verticale » qui automatise un métier précis. Les tickets seed sont faciles à obtenir, il y a énormément de nouvelles boîtes. | Goodweek (10,7 M€, gouvernance IA pour PME), Webyn (7 M€, agents de personnalisation e-commerce), Reduck (2,7 M€, automatisation web pour agents IA), AQQI (4 M€, assistant IA d'achat immobilier), INEVITABLE (10 M€, outils IA pour studios de cinéma), Vocca (20 M$ série A), Arlequin AI (28 M€) |
| **Santé, medtech, biotech + IA** | Le second secteur le plus financé : besoin de diagnostic, de découverte de médicaments et de télésuivi, avec un fort soutien de Bpifrance. | Rivercell (22,5 M€, modélisation cellulaire IA), Biolevate (30 M€), Implicity (35 M€, télésurveillance cardiaque), Incepto (14 M€, radiologie IA), HighLife (80 M€) |
| **Climat, énergie, GreenTech** | Secteur le plus représenté dans le French Tech 120 (25 entreprises). Il est porté par la régulation (CSRD, décret tertiaire) et par le coût de l'énergie. | CarbonFarm (5,5 à 7 M€, suivi du méthane par satellite), Deepki, Jimmy (micro-réacteurs), Mylight150, Upsun (solaire) |
| **Deeptech, spatial, défense, quantique** | Souveraineté européenne et contexte géopolitique : de gros tickets publics et privés. | The Exploration Company (387 M€), Aura Aero (340 M€), Pasqal (340 M€, quantique), Harmattan AI (licorne de la défense), Vates (30 M€) |
| **Industrie 4.0 / robotique** | Réindustrialisation et « physical AI ». Les financements mondiaux de la robotique ont progressé de 185 % sur un an au T3. | Wormsensing (6,5 M€, maintenance prédictive) |
| **Cybersécurité** | Obligations NIS2, et les PME sont désormais ciblées. | Netsec (8,9 M€), Hackuity (16,3 M€), Stoïk (cyber-assurance), GitGuardian |
| **Fintech / SaaS de gestion** | Facturation électronique obligatoire et financement alternatif. | Pennylane (175 M€), Pigment (222 M€), Wavo (10 M€, financement de stock), Wealthcome (15 M€), Spiko |
| **RH, intérim, mobilité, loisirs (scale-ups)** | Des marchés matures qui se digitalisent. | Hellocse, Verley, Mistertemp', Ornikar, Stych, Yespark, Weezevent, HomeExchange |

## 3. Qui cibler pour des sites vitrines (le plus important)

Les grosses scale-ups (Mistral, Pigment, Pennylane, Alan…) ont des équipes marketing en interne : ce ne sont **pas** des clients réalistes.

Les meilleures cibles :

1. **Startups seed / pré-seed (1 à 10 M€ levés)** : elles viennent de lever, doivent paraître crédibles auprès des clients et des recruteurs, et n'ont souvent qu'un site Webflow fait à la va-vite. Exemples ci-dessus : Reduck, AQQI, Goodweek, Webyn, CarbonFarm, Wormsensing, Netsec, Wavo. Source à suivre chaque semaine : MaddyMoney (Maddyness) et le récap hebdo de Les Pépites Tech.
2. **PME / TPE de services aux entreprises en création** (premier moteur de créations selon l'INSEE) : nettoyage, conseil, sécurité, maintenance. Elles ont un besoin immédiat d'un site pour le SEO local et les devis.
3. **Artisans de la rénovation énergétique / du solaire / des bornes de recharge** : forte demande, nécessité d'inspirer confiance (labels RGE, aides), et ils sont peu équipés en sites.
4. **Silver économie / services à domicile** : marché en croissance, clientèle (les familles) qui cherche en ligne.
5. **Indépendants créatifs et commerces locaux** (comme `larralde-surf`) : petits budgets, mais en grand volume.

## 4. Proposition d'organisation dans le repo

- Un dossier et une branche par client ou maquette : `site/<slug>` (ex. `site/carbonfarm-demo`).
- Ou d'abord une branche par **secteur-template**, réutilisable ensuite :
  - `template/startup-ia-b2b` (hero + démo produit + logos clients + recrutement)
  - `template/medtech` (confiance, conformité, publications)
  - `template/greentech-energie` (impact chiffré, carte, certifications)
  - `template/services-pme` (devis, zone d'intervention, avis Google)
  - `template/artisan-renovation` (RGE, aides, réalisations avant/après)

## Sources

- [Maddyness, 30/10/2026 : l'IA concentre plus de 90 % des 41 M€](https://www.maddyness.com/2026/10/30/french-tech-lia-concentre-plus-de-90-des-41-millions-deuros-leves-cette-semaine/)
- [Maddyness, 23/10/2026 : 271 M€ portés par Pigment](https://www.maddyness.com/2026/10/23/french-tech-pres-de-271-millions-deuros-leves-en-une-semaine-portes-par-pigment/)
- [Maddyness, 16/10/2026 : 58,5 M€](https://www.maddyness.com/2026/10/16/les-startups-francaises-ont-leve-585-millions-deuros-cette-semaine/)
- [Maddyness, 09/10/2026 : 217 M€](https://www.maddyness.com/2026/10/09/les-startups-francaises-ont-leve-217-millions-deuros-cette-semaine/)
- [Les Pépites Tech, semaine 42](https://lespepitestech.com/blog/2026/10/20/1088-millions-deuros-leves-par-les-startups-francaises-semaine-42-2026)
- [Les Pépites Tech, semaine 41](https://lespepitestech.com/node/34684)
- [FrenchWeb : Spiko, Wiremind, Vates](https://www.frenchweb.fr/spiko-wiremind-vates-pres-de-270-millions-deuros-annonces-par-la-french-tech-cette-semaine/463906)
- [Licorne Society : bilan S1 2026](https://www.licornesociety.com/blog/bilan-levees-de-fonds-s1-2026)
- [Eldorado : juillet 2026](https://eldorado.co/blog/2026/08/12/juillet-2026-les-startups-francaises-levent-114-milliard-deuros)
- [Eldorado : avril 2026](https://eldorado.co/blog/2026/05/07/avril-2026-les-startups-francaises-levent-659-millions-deuros)
- [FrenchWeb : French Tech 120 2026](https://www.frenchweb.fr/french-tech-120-2026-a-quoi-ressemble-leconomie-francaise-de-la-prochaine-decennie/462367)
- [Siècle Digital : French Tech 120 2026](https://siecledigital.fr/2026/06/17/french-tech-120-2026-la-nouvelle-selection-revele-les-futurs-geants-francais-de-la-tech/)
- [France FinTech : promotion Next40/120](https://francefintech.org/promotion-2026-du-french-tech-next-40-120/)
- [INSEE : créations d'entreprises juillet-septembre 2026](https://www.insee.fr/fr/statistiques/9078876)
- [INSEE : août 2026](https://www.insee.fr/fr/statistiques/9052433)
- [Crunchbase : T3 2026, financement mondial](https://news.crunchbase.com/venture/q3-2026-global-startup-funding-ai-billion-dollar-rounds-exits-data/)
- [Crunchbase : robotique T3 2026](https://news.crunchbase.com/venture/q3-2026-us-china-robotics-startup-funding-jumps-physical-ai-push/)
- [CCI Lyon : silver économie](https://www.lyon-metropole.cci.fr/actualite/la-silver-economie-saisir-un-marche-porteur)
