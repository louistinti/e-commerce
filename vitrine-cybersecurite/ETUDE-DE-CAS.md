# Étude de cas : site vitrine d'un SOC managé pour PME

Entreprise du projet : **Rempart**, entreprise **fictive** (SOC managé 24/7 pour PME et ETI, conformité NIS2 incluse, prix fixe par poste). Les entreprises analysées sont réelles.

## Executive summary

NIS2 fait passer le nombre d'entités régulées en France d'environ 500 à environ 15 000, alors que 8 PME sur 10 se disent mal armées et dépensent moins de 2 000 € par an en cyber. Les 5 sites analysés (Stoïk, Dattak, Advens, Huntress, Arctic Wolf) prouvent leur sérieux par des chiffres et des certifications. Mais 4 sur 5 n'affichent aucun prix, et la recherche n'a trouvé de numéro d'urgence visible sur aucun. Rempart peut se démarquer avec trois éléments que personne ne combine : un prix par poste affiché, un quiz qui donne un résultat utile sans exiger d'e-mail, et une ligne d'urgence présente sur chaque écran, le tout dans un ton calme et pédagogique.

---

## 1. Le marché en 5 lignes

- **NIS2 multiplie le nombre d'entités régulées par 30 environ** : près de 15 000 entités dans 18 secteurs, contre environ 500 opérateurs sous NIS1 ([Kiteworks](https://www.kiteworks.com/fr/?p=258118), [tech-insider](https://tech-insider.org/fr/directive-nis-2-transposition-france-2026/)). Le seuil type est l'entreprise moyenne : 50 salariés ou plus, ou plus de 10 M€ de chiffre d'affaires.
- **La loi française n'est toujours pas votée** : le projet de loi « Résilience » a été repoussé à septembre 2026 au plus tôt ([Leto](https://www.leto.legal/news/nis2-transposition-septembre-2026)). La Commission aurait renvoyé la France devant la CJUE en juillet 2026, d'après une seule source ([IT-Connect](https://www.it-connect.fr/nis2-transposition-france-saisine-cjue/)). L'ANSSI a publié son référentiel ReCyf ([Next](https://next.ink/229605/nis-2-lanssi-publie-son-recyf-la-csnp-simpatiente-et-le-fait-savoir/)). **Pour le site** : parler de « se préparer », pas « être conforme à la loi ».
- **Les PME sont exposées** : 16 % ont subi un incident en 12 mois, environ 8 sur 10 se disent mal armées, la majorité dépense moins de 2 000 € par an ([Cybermalveillance.gouv.fr, oct. 2025](https://www.cybermalveillance.gouv.fr/medias/2025/10/CP-TPE-PME-07102025-3.pdf), [infographie](https://www.cybermalveillance.gouv.fr/medias/2025/10/250910_InfographieMaturiteCyberTPE-PME_SCREEN.pdf)). France Num 2025 donne plus d'une PME sur trois déjà touchée ([Siècle Digital](https://siecledigital.fr/2025/09/17/barometre-france-num-2025-comment-evoluent-les-usages-numeriques-dans-les-pme/)).
- **Leurs freins** : 63 % citent le manque de connaissances, 61 % le budget, 59 % le temps ([Liora](https://liora.io/les-tpe-pme-francaises-accusent-un-retard-en-maturite-cyber-selon-une-analyse-2025)).
- **L'offre descend en gamme** : Micro-SOC chez Orange Cyberdefense, EDR managé chez Free Pro, SOC inclus dans l'assurance chez Stoïk. Ordres de grandeur : 20 à 30 € par poste et par an pour un EDR managé d'entrée de gamme, environ 20 000 € par an pour un SOC complet pour 150 salariés ([JDN](https://www.journaldunet.com/cybersecurite/1542941-pme-les-criteres-de-choix-pour-un-soc-adapte-a-ses-besoins/), article non daté). Il existe aussi un dispositif public gratuit, MonAideCyber : un diagnostic d'1 h 30 qui donne 6 recommandations ([Fiducial](https://www.fiducial.fr/Articles-et-dossiers/MonAideCyber-Diagnostic-gratuit-pour-proteger-les-TPE-PME)).

## 2. Analyse de 5 sites réels (framework « design critique »)

> Les pages n'ont **pas** pu être affichées : le réseau de la session bloquait l'accès direct. La première impression, la hiérarchie et l'accessibilité sont évaluées **d'après la description** des résultats de recherche (titres, textes, structure). Contraste et taille de texte : **non observables**, sauf mention contraire.

### 2.1 Stoïk (FR) : https://www.stoik.com/assurance, https://www.stoik.com/cybersecurite
- **Positionnement** : un assureur cyber qui inclut de la sécurité (scans, sensibilisation, réponse à incident, MDR avec CrowdStrike). Vendu par des courtiers.
- **Première impression (2 s)** : la preuve chiffrée attire l'œil (« 14 000+ PME et ETI », « SOC européen internalisé 24h/7j »). L'objectif est clair pour un courtier, moins pour un dirigeant, puisque l'assurance et la sécurité sont sur deux pages distinctes.
- **Usabilité** : le CTA de devis renvoie vers un courtier ([devis](https://www.stoik.com/devis)), ce qui fait une étape de plus pour le dirigeant. La navigation est segmentée par audience (entreprises, [courtiers](https://www.stoik.com/courtiers)) et par sujet ([prix](https://www.stoik.com/prix-assurance-cyber), [NIS2](https://www.stoik.com/nis2)).
- **Hiérarchie visuelle** : chiffres de preuve, puis garanties, puis services inclus (d'après l'ordre des extraits).
- **Accessibilité** : non observable. Les plafonds diffèrent selon la langue (2 Md€ en FR, 1 Md€ ailleurs), ce qui pose un problème de clarté du contenu.
- **Ce qui marche** : des preuves chiffrées, un scan externe gratuit comme porte d'entrée, une page entière consacrée au prix, une page NIS2 pour le SEO.
- **Recommandations** : 1) un CTA direct pour le dirigeant, en plus du canal courtier ; 2) des chiffres identiques dans toutes les langues ; 3) dater les pages anciennes.

### 2.2 Dattak (FR) : https://www.dattak.io/fr, https://www.dattak.io/fr/entreprises
- **Positionnement** : un « opérateur de gestion des risques technologiques ». L'assurance cyber est proactive, avec un CERT et une plateforme de surveillance.
- **Première impression (2 s)** : la baseline est abstraite. Il faut lire pour comprendre qu'il s'agit d'assurance cyber.
- **Usabilité** : un double parcours, entreprises ([entreprises](https://www.dattak.io/fr/entreprises)) et [courtiers](https://www.dattak.io/fr/courtiers). Le devis annoncé en environ 2 min sans questionnaire technique (grâce au scan) est un argument fort de faible friction.
- **Hiérarchie visuelle** : l'offre est découpée en **avant, pendant, après** l'incident ([cyberattack](https://www.dattak.io/fr/cyberattack)). C'est une structure narrative lisible.
- **Accessibilité** : non observable.
- **Ce qui marche** : une hotline CERT 24/7 avec un délai affiché (moins de 2 min), une page de [témoignages](https://www.dattak.io/fr/temoignages), un blog de réflexes post-attaque, des chiffres de volume (3 500+ assurés, 400+ incidents).
- **Recommandations** : 1) remplacer la baseline par le bénéfice ; 2) unifier le plafond d'éligibilité (50, 200 ou 500 M€ selon les pages) ; 3) mettre le numéro du CERT dans l'en-tête.

### 2.3 Advens (FR) : https://www.advens.com/mysoc/offres/
- **Positionnement** : un pure player et MSSP français, « leader du SOC-as-a-Service », qualifié PDIS par l'ANSSI depuis septembre 2025 ([news](https://www.advens.com/media/news-advens/qualification-pdis/)), plus PASSI et PRIS.
- **Première impression (2 s)** : des qualifications et des classements analystes (ISG, Markess). L'objectif est clair pour un RSSI de grand compte, opaque pour une PME (mySOC, MDR, OT/IoT).
- **Usabilité** : les offres sont organisées « selon votre trajectoire de sécurité ». Il y a une page service et portail ([service](https://www.advens.com/mysoc/service/)) et des [cas clients](https://www.advens.com/cas-clients/soc-securite-groupe-international/). La recherche n'a trouvé ni prix ni numéro d'urgence.
- **Hiérarchie visuelle** : la marque d'offre passe avant le bénéfice (d'après les titres).
- **Accessibilité** : non observable. Le jargon pose un problème d'accessibilité cognitive pour la cible PME.
- **Ce qui marche** : une preuve d'autorité forte (ANSSI), un SOC Manager dédié qui incarne le service, des paliers par maturité.
- **Recommandations** : 1) un parcours PME sans acronymes ; 2) une ligne d'urgence visible ; 3) au moins un « à partir de ».

### 2.4 Huntress (international) : https://www.huntress.com/why-huntress, https://www.huntress.com/pricing
- **Positionnement** : la sécurité managée pour les PME et les MSP, avec un « 24/7 SOC » inclus, porté par une IA et des analystes humains.
- **Première impression (2 s)** : des chiffres de vitesse : délai moyen de résolution (MTTR) de 8 min, déploiement en moins de 20 min, environ 285 000 clients. La promesse PME est claire.
- **Usabilité** : une page tarifs publique, des pages produits par brique, des comparatifs face aux concurrents.
- **Hiérarchie visuelle** : bénéfice, puis chiffres, puis produits. Le catalogue est large (EDR, ITDR, SIEM, SAT).
- **Accessibilité** : non observable. La multiplication des acronymes pèse sur la charge cognitive.
- **Ce qui marche** : **le prix par endpoint est affiché** et le SOC « included at no additional cost ». Les comparatifs captent les recherches d'intention.
- **Recommandations** : 1) un seul prix de référence (8,99 $ par endpoint d'un côté, 4,80 $ par identité de l'autre, ce qui crée de la confusion) ; 2) supprimer les dates futures (« 2027 ») des pages SEO ; 3) regrouper les briques en 2 ou 3 paliers.

### 2.5 Arctic Wolf (international) : https://arcticwolf.com/how-it-works/, https://arcticwolf.com/solutions/bundles/
- **Positionnement** : un SOC « concierge », avec une équipe de triage 24x7 et une équipe de sécurité nommée.
- **Première impression (2 s)** : le modèle de service humain (Concierge), et récemment l'« agentic AI » (60 % des investigations résolues par l'IA, selon le communiqué de novembre 2026).
- **Usabilité** : 3 bundles (Core, Plus, Total) avec une garantie financière par palier. Une page « How it works » et une page [Inside the SOC](https://arcticwolf.com/uk/inside-the-soc/).
- **Hiérarchie visuelle** : les paliers et la garantie sont lisibles (d'après les extraits).
- **Accessibilité** : non observable.
- **Ce qui marche** : 3 paliers, une garantie chiffrée, un SOC humanisé sans hacker à capuche.
- **Recommandations** : 1) ne pas laisser le discours IA éclipser l'humain pour la cible PME ; 2) afficher un ordre de prix ; 3) sourcer les affirmations du type « 9x moins cher ».

Hackuity et Netsec, cités dans le README comme prospects, n'ont pas été analysés : Hackuity vise les grands comptes, et le budget de recherche était épuisé.

## 3. Thèmes clés

| Thème | Prévalence | Observations (faits relevés) | Interprétation |
|---|---|---|---|
| Preuve par les chiffres | **5 sur 5** | Stoïk : 14 000+ PME. Dattak : 3 500+ assurés, moins de 2 min. Huntress : 8 min, 285 000. Arctic Wolf : garantie chiffrée. Advens : classements ISG et Markess. | Les chiffres sont la norme, donc ils ne différencient plus. Les **délais** (minutes) parlent davantage au dirigeant que les volumes. |
| Pas de prix affiché | **4 sur 5** | Seul Huntress a une page tarifs publique. Stoïk a une page « prix » éditoriale, avec un exemple daté. | Le prix est le premier frein (61 % citent le budget). L'afficher crée un avantage immédiat. |
| Vente intermédiée ou commerciale | **4 sur 5** | Stoïk et Dattak passent par les courtiers. Advens et Arctic Wolf passent par un commercial. | Le dirigeant n'a pas de parcours autonome. Un diagnostic ou un quiz en libre-service comble ce vide. |
| Jargon et acronymes | **3 sur 5** | Advens (MDR, OT/IoT, DFIR), Huntress (EDR, ITDR, SIEM, SAT), Arctic Wolf (agentic SOC). | Une barrière pour les 63 % de PME qui manquent de connaissances. |
| Récit temporel de l'incident | **2 sur 5** | Dattak (avant, pendant, après), Arctic Wolf (triage puis concierge). | Raconter la réponse rassure davantage que décrire la technologie. |
| Urgence visible | **0 sur 5** (d'après les recherches) | Aucun numéro d'urgence relevé en tête de page. Dattak mentionne une hotline CERT 24/7 dans le contenu. | Un manque direct pour le persona « attaqué ce matin ». |
| Page NIS2 dédiée | **1 sur 5** confirmé | Stoïk /nis2. | Une demande de recherche forte et peu couverte côté MSSP. |

## 4. Insights → Opportunités

| Insight | Opportunité | Impact | Effort |
|---|---|---|---|
| 4 sites sur 5 cachent le prix, et le budget est le 2e frein | Grille par poste et simulateur « nombre de postes → €/mois » | H | M |
| Pas de parcours autonome pour le dirigeant | Quiz de 5 questions avec résultat et 3 actions sans e-mail. Rapport complet contre un e-mail | H | M |
| Aucun numéro d'urgence visible | Bouton « Urgence : nous appeler » fixe sur mobile, numéro dans l'en-tête sur desktop | H | B |
| Le jargon exclut les dirigeants non techniques | Les briques traduites en verbes (« on détecte, on bloque, on vous appelle ») et un glossaire en infobulle | M | B |
| Le récit temporel rassure (Dattak) | Timeline « minute par minute » avec la personne qui agit à chaque étape | H | M |
| NIS2 est recherchée, la loi est floue | Test « Suis-je concerné ? », checklist datée, page longue SEO | M | M |
| Le discours IA peut inquiéter | Analystes nommés, photo réelle du SOC | M | B |
| Prix incohérents d'une page à l'autre (Huntress) | Une seule source de prix (composant unique réutilisé partout) | M | B |

## 5. Erreurs à éviter

- **Jouer sur la peur** : hacker à capuche, cadenas rouge, code Matrix, compte à rebours.
- **Les acronymes non traduits.**
- **Promettre une conformité NIS2 « garantie »** alors que la loi n'est pas votée et que la conformité dépend aussi du client.
- **Afficher des certifications non obtenues** : ISO 27001 et PDIS sont vérifiables. Sur la démo, il faut des placeholders explicites.
- **Un quiz qui exige l'e-mail avant le score.**
- **Des prix différents selon les pages.**

## 6. Conclusion appliquée à Rempart

- Rempart se positionne comme **« le SOC d'une grande entreprise, au prix et au langage d'une PME »**. Ses trois différenciateurs : prix par poste affiché, numéro d'urgence, quiz utile.
- Le hero promet le résultat. Le CTA principal est « Faire le test (2 min) » et le CTA secondaire « Demander mon diagnostic gratuit ».
- NIS2 suit le format « Suis-je concerné ? » en 3 questions, avec une checklist datée et la mention « transposition française en cours ».
- Les preuves s'affichent dans cet ordre : délai de prise en charge, qualifications (placeholders), témoignages de dirigeants de PME, partenaires.
- Le ton est celui du pompier, pas celui de l'alarme.
- Le nom est provisoire et fictif : il faut vérifier l'INPI et n'emprunter aucun code visuel à Stoïk, Dattak ou Advens.

## 7. Questions à valider en recherche utilisateur

1. Un dirigeant de PME fait-il confiance à un prix affiché, ou le perçoit-il comme « trop beau, donc incomplet » ? Que doit contenir la mention « ce qui n'est pas inclus » ?
2. Le quiz de 5 questions est-il compris sans aide ? Quelle question fait abandonner ?
3. Quel est le seuil d'acceptation pour laisser son e-mail : après le score, ou pour le rapport seulement ?
4. Qu'est-ce qui rassure le plus : le délai en minutes, la certification ANSSI, le témoignage d'un pair, ou la photo de l'équipe ?
5. Un dirigeant sait-il dire s'il est concerné par NIS2 ? Comprend-il la différence entre être une entité régulée et être fournisseur d'une entité régulée ?
6. Sur mobile, en situation d'urgence simulée, combien de secondes faut-il pour trouver et appeler le numéro ?

## 8. Notes de méthode

- **Sources** : recherches web (novembre 2026) sur les sites des entreprises, la presse spécialisée (JDN, Next, Siècle Digital, Le Monde Informatique) et les publications publiques (Cybermalveillance.gouv.fr, ANSSI MonAideCyber).
- **Limites** :
  - **les visuels n'ont pas été vus** : l'accès direct aux sites est bloqué par le réseau de la session. Le critique est fondé sur les textes et la structure décrits par les résultats de recherche ;
  - le contraste, la taille de texte et le comportement mobile ne sont pas évalués ;
  - les chiffres des entreprises sont déclaratifs ;
  - le statut de NIS2 est à revérifier à la date de mise en ligne ;
  - le budget de recherche web a été épuisé en cours d'étude, ce qui explique l'absence de références Behance, Dribbble et Awwwards et l'absence d'un intégrateur régional analysé.
- **Échantillon** : 5 sites, 3 français et 2 internationaux. Ce n'est pas représentatif des intégrateurs régionaux, qui sont la cible commerciale du README.
