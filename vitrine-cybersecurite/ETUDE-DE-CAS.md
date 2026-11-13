# Étude de cas : site vitrine d'un SOC managé pour PME

Entreprise du projet : **Rempart**, entreprise **fictive** (SOC managé 24/7 pour PME et ETI, conformité NIS2 incluse, prix fixe par poste). Les entreprises analysées sont réelles. Aucun chiffre n'est inventé : chaque donnée de marché a sa source, et Rempart n'a aucun résultat chiffré.

## Executive summary

NIS2 fait passer le nombre d'entités régulées en France d'environ 500 à près de 15 000, alors que 80 % des TPE-PME ne se disent pas préparées et que 3 sur 4 investissent moins de 2 000 € par an en cybersécurité (sources en section 1). Les 5 sites analysés (Stoïk, Dattak, Advens, Huntress, Arctic Wolf) prouvent leur sérieux par des chiffres et des qualifications. Un seul publie un prix par poste (Huntress), et aucun n'affiche un numéro d'urgence en clair : Arctic Wolf a un lien dans l'en-tête, Advens un bouton flottant qui ne lance pas d'appel. Rempart peut se démarquer avec trois éléments que personne ne combine : un prix par poste affiché, un quiz qui donne un résultat utile sans exiger d'e-mail, et une ligne d'urgence présente sur chaque écran, le tout dans un ton calme et pédagogique.

---

## 1. Le marché en 5 lignes

- **NIS2 multiplie le nombre d'entités régulées par 30 environ** : d'environ 500 à près de 15 000 entités, dans 18 secteurs au lieu de 6, d'après la note explicative du projet de loi ([Kiteworks](https://www.kiteworks.com/fr/conformite-reglementaire/france-nis2-report-retard-conformite/), mis à jour le 12 octobre 2026, vu le 2026-11-13). Le seuil type est l'entreprise de taille moyenne des secteurs des annexes I et II ([Stoïk](https://www.stoik.com/nis2), vu le 2026-11-13). Au sens européen, une petite entreprise occupe moins de 50 personnes et son chiffre d'affaires ou son bilan n'excède pas 10 M€ ([recommandation 2003/361, EUR-Lex](https://eur-lex.europa.eu/legal-content/FR/TXT/HTML/?uri=CELEX:32003H0361), vu le 2026-11-13).
- **La loi française n'est toujours pas votée** : le Sénat a adopté le projet de loi « Résilience » en mars 2025 ([Kiteworks](https://www.kiteworks.com/fr/conformite-reglementaire/france-nis2-report-retard-conformite/)). Le 6 octobre 2026, l'Assemblée nationale l'a retiré de son ordre du jour, sans nouvelle date, et la Commission européenne a saisi la CJUE contre la France ([Leto](https://www.leto.legal/news/nis2-transposition-septembre-2026), mise à jour du 19 octobre 2026, vu le 2026-11-13). Kiteworks date cette saisine du 8 juillet 2026. L'ANSSI a publié son référentiel ReCyF ([ANSSI](https://cyber.gouv.fr/reglementation/cybersecurite-systemes-dinformation/directives-nis-nis2-et-dispositif-saiv/directive-nis-2/), vu le 2026-11-13). **Pour le site** : parler de « se préparer », pas « être conforme à la loi ».
- **Les PME sont exposées** : 16 % des TPE-PME se déclarent victimes d'au moins un incident, 80 % ne sont pas préparées, 3 sur 4 investissent moins de 2 000 € par an (enquête OpinionWay, 588 entreprises de moins de 250 salariés, juin et juillet 2025, [infographie Cybermalveillance.gouv.fr](https://www.cybermalveillance.gouv.fr/medias/2025/10/250910_InfographieMaturiteCyberTPE-PME_SCREEN.pdf), bench n° 18, vu le 2026-11-12). Le baromètre France Num 2025 donne plus d'une PME sur trois déjà confrontée à un incident ([Siècle Digital](https://siecledigital.fr/2025/09/17/barometre-france-num-2025-comment-evoluent-les-usages-numeriques-dans-les-pme/), vu le 2026-11-13).
- **Leurs freins** : 63 % citent le manque de connaissances, 61 % le budget, 59 % le temps, selon Cybermalveillance.gouv.fr ([Liora](https://liora.io/les-tpe-pme-francaises-accusent-un-retard-en-maturite-cyber-selon-une-analyse-2025), vu le 2026-11-13).
- **L'offre descend en gamme** : Micro-SOC chez Orange Cyberdefense, MDR supervisé par un SOC chez Stoïk, en abonnement distinct de l'assurance ([Stoïk](https://www.stoik.com/assurance), vu le 2026-11-13). Ordres de grandeur cités par le [JDN](https://www.journaldunet.com/cybersecurite/1542941-pme-les-criteres-de-choix-pour-un-soc-adapte-a-ses-besoins/) (4 juillet 2025, vu le 2026-11-13) : 20 à 30 € par poste et par an pour le micro-SOC d'Orange Cyberdefense, environ 20 000 € par an pour un SOC managé couvrant réseau et cloud d'une PME de 150 salariés. Il existe aussi un dispositif public gratuit, MonAideCyber : un diagnostic d'1 h 30 qui aboutit à 6 mesures de sécurité ([Fiducial](https://www.fiducial.fr/Articles-et-dossiers/MonAideCyber-Diagnostic-gratuit-pour-proteger-les-TPE-PME), vu le 2026-11-13).

## 2. Analyse de 5 sites réels (framework « design critique »)

> La première version de cette section était écrite d'après les résultats de recherche. Les pages ont depuis été ouvertes et capturées dans un vrai navigateur le 2026-11-12 (voir [BENCH.md](BENCH.md)), et les chiffres des concurrents revérifiés le 2026-11-13. Les affirmations que le bench contredit sont corrigées ci-dessous. Les chiffres des entreprises sont ceux affichés sur leurs pages.

### 2.1 Stoïk (FR) : https://www.stoik.com/assurance, https://www.stoik.com/cybersecurite
- **Positionnement** : un assureur cyber qui ajoute de la sécurité. Scans de vulnérabilités et réponse à incident inclus dans chaque police, MDR supervisé par un SOC en abonnement distinct. Vendu par des courtiers.
- **Première impression (2 s)** : grande carte bleu saturé, puis la preuve chiffrée : « 14 000+ PME et ETI européennes protégées et assurées », « 24h/7j de surveillance par un SOC européen internalisé » (vu le 2026-11-13). Le premier bouton est « Devenir partenaire », avant « Se protéger » (bench n° 2) : l'objectif est clair pour un courtier, moins pour un dirigeant.
- **Usabilité** : le CTA de devis renvoie vers un courtier ([devis](https://www.stoik.com/devis)), ce qui fait une étape de plus pour le dirigeant. La navigation est segmentée par audience (entreprises, [courtiers](https://www.stoik.com/courtiers)) et par sujet ([prix](https://www.stoik.com/prix-assurance-cyber), [NIS2](https://www.stoik.com/nis2)).
- **Hiérarchie visuelle** : chiffres de preuve, puis garanties, puis services inclus.
- **Accessibilité** : contraste non mesuré. Clarté du contenu : sur la page assurance, « 2 Md€ » est le chiffre d'affaires maximal des entreprises éligibles et 10 M€ le plafond de garantie. Les deux montants s'affichent en pastilles côte à côte (bench n° 5), faciles à confondre.
- **Ce qui marche** : des preuves chiffrées, une page éditoriale sur le prix avec des prix d'appel par secteur et leurs hypothèses écrites (bench n° 12), une page NIS2 pour le SEO.
- **Recommandations** : 1) un CTA direct pour le dirigeant, en plus du canal courtier ; 2) distinguer en toutes lettres plafond de chiffre d'affaires et plafond de garantie ; 3) dater les pages anciennes (l'article prix date du 14 juin 2023).

### 2.2 Dattak (FR) : https://www.dattak.io/fr, https://www.dattak.io/fr/entreprises
- **Positionnement** : un « opérateur de gestion des risques technologiques ». L'assurance cyber est proactive, avec un CERT et une plateforme de surveillance.
- **Première impression (2 s)** : hero sombre, titre qui reste une catégorie (« Dattak réduit et assure les risques technologiques des entreprises », bench n° 3). Il faut lire pour comprendre qu'il s'agit d'assurance cyber.
- **Usabilité** : un double parcours, [entreprises](https://www.dattak.io/fr/entreprises) et [courtiers](https://www.dattak.io/fr/courtiers).
- **Hiérarchie visuelle** : l'offre est découpée en **avant, pendant, après** l'incident ([cyberattack](https://www.dattak.io/fr/cyberattack), qui redirige vers /fr/insurance). C'est une structure narrative lisible.
- **Accessibilité** : bouton terracotta `#C4684A` à texte blanc, 3,9:1, sous le seuil AA de 4,5:1 (bench n° 3).
- **Ce qui marche** : un CERT avec un délai affiché (« Intervention en moins de 2 minutes »), une page de [témoignages](https://www.dattak.io/fr/temoignages), un blog de réflexes post-attaque, des chiffres de volume (3 500+ entreprises, 400+ incidents gérés, vu le 2026-11-13 sur dattak.io/fr).
- **Recommandations** : 1) remplacer la baseline par le bénéfice ; 2) porter le bouton principal à 4,5:1 ; 3) mettre le numéro du CERT dans l'en-tête.

### 2.3 Advens (FR) : https://www.advens.com/mysoc/offres/
- **Positionnement** : un pure player français, « leader du SOC-as-a-Service » selon lui, qualifié PDIS par l'ANSSI en septembre 2025 ([news](https://www.advens.com/media/news-advens/qualification-pdis/), article du 30 septembre 2025).
- **Première impression (2 s)** : bandeau noir, titre bleu `#006BFF` en Space Grotesk (bench n° 17). La page qualification renvoie vers le classement ISG Provider Lens 2025. L'objectif est clair pour un RSSI de grand compte, opaque pour une PME (mySOC, MDR, OT/IoT).
- **Usabilité** : l'offre est une trajectoire en 3 phases (schéma en image), « selon votre trajectoire de sécurité ». Il y a une page service et portail ([service](https://www.advens.com/mysoc/service/)) et des [cas clients](https://www.advens.com/cas-clients/soc-securite-groupe-international/). Aucun prix. Un bouton flottant « Assistance 24/7 » reste visible, y compris sur mobile, mais il ne lance pas d'appel (aucun lien `tel:`).
- **Hiérarchie visuelle** : la marque d'offre passe avant le bénéfice.
- **Accessibilité** : le bouton « Assistance 24/7 » fait 2,4:1, texte blanc sur `#0AB3FF` (bench n° 13). Le jargon pose un problème d'accessibilité cognitive pour la cible PME.
- **Ce qui marche** : une preuve d'autorité forte (ANSSI), « un même plan de surveillance, un même analyste », qui incarne le service, une offre par maturité.
- **Recommandations** : 1) un parcours PME sans acronymes ; 2) un bouton d'urgence qui lance l'appel, à 4,5:1 ; 3) au moins un « à partir de ».

### 2.4 Huntress (international) : https://www.huntress.com/why-huntress, https://www.huntress.com/pricing
- **Positionnement** : la sécurité managée pour les PME et les MSP, avec un SOC 24/7 inclus.
- **Première impression (2 s)** : fond quasi noir, titre en capitales, photo de salle serveurs aux néons (bench n° 1). Pas de chiffre sous le titre : « 285,000 businesses » n'apparaît que plus bas, et le déploiement « in under 20 minutes » dans un paragraphe.
- **Usabilité** : une page tarifs publique, mais un formulaire « Get pricing » passe avant les prix (bench n° 10). Des pages produits par brique.
- **Hiérarchie visuelle** : bénéfice, puis produits. Le catalogue est large (EDR, ITDR, SIEM, SAT).
- **Accessibilité** : contraste du texte non mesuré. Le bouton cyan à texte noir fait 11,8:1. La multiplication des acronymes pèse sur la charge cognitive.
- **Ce qui marche** : **le prix par poste est public** (Managed EDR à 8,99 $ par poste et par mois) et le SOC est « included at no additional cost » (bench n° 10).
- **Recommandations** : 1) montrer les prix avant le formulaire ; 2) remonter une preuve sous le titre ; 3) regrouper les briques en 2 ou 3 paliers.

### 2.5 Arctic Wolf (international) : https://arcticwolf.com/how-it-works/, https://arcticwolf.com/solutions/bundles/
- **Positionnement** : un SOC « concierge », avec une équipe de triage 24x7 et une équipe de sécurité nommée.
- **Première impression (2 s)** : le modèle de service humain (Concierge Delivery Model), et dans le menu l'« Agentic SOC » (vu le 2026-11-13).
- **Usabilité** : 3 bundles (Core, Plus, Total) avec des options de garantie financière de 100 k$ à 1,5 M$ selon le palier (vu le 2026-11-13). Une page « How it works » et une page [Inside the SOC](https://arcticwolf.com/uk/inside-the-soc/). Un lien « Experienced a Breach? » dans l'en-tête desktop, caché dans le menu burger sur mobile.
- **Hiérarchie visuelle** : les paliers et la garantie sont lisibles.
- **Accessibilité** : non mesurée.
- **Ce qui marche** : 3 paliers, une garantie chiffrée, une vraie photo d'analyste au lieu d'un hacker à capuche.
- **Recommandations** : 1) ne pas laisser le discours IA éclipser l'humain pour la cible PME ; 2) afficher un ordre de prix ; 3) garder le lien d'urgence visible sur mobile, hors du menu.

Hackuity et Netsec, cités dans le README comme prospects, n'ont pas été analysés : Hackuity vise les grands comptes, et le budget de recherche était épuisé.

## 3. Thèmes clés

| Thème | Prévalence | Observations (faits relevés) | Interprétation |
|---|---|---|---|
| Preuve par les chiffres | **5 sur 5** | Stoïk : 14 000+ PME et ETI. Dattak : 3 500+ entreprises, 400+ incidents, moins de 2 min. Huntress : 285 000 entreprises, moins de 20 min. Arctic Wolf : garanties chiffrées. Advens : classement ISG. | Les chiffres sont la norme, donc ils ne différencient plus. Rempart, fictive, n'en a pas : sa preuve passe par le prix affiché, la timeline et les chiffres publics sourcés. |
| Pas de prix par poste | **4 sur 5** | Seul Huntress publie des prix par poste, après un formulaire. Stoïk a une page « prix » éditoriale, avec des exemples datés de 2023. | Le budget est un frein cité par 61 % des TPE-PME. Afficher un prix crée un avantage immédiat. |
| Vente intermédiée ou commerciale | **4 sur 5** | Stoïk et Dattak passent par les courtiers. Advens et Arctic Wolf passent par un commercial. | Le dirigeant n'a pas de parcours autonome. Un diagnostic ou un quiz en libre-service comble ce vide. |
| Jargon et acronymes | **3 sur 5** | Advens (MDR, OT/IoT), Huntress (EDR, ITDR, SIEM, SAT), Arctic Wolf (Agentic SOC). | Une barrière pour les 63 % de TPE-PME qui citent le manque de connaissances. |
| Récit temporel de l'incident | **2 sur 5** | Dattak (avant, pendant, après), Arctic Wolf (triage puis concierge). | Raconter la réponse rassure davantage que décrire la technologie. |
| Numéro d'urgence en clair | **0 sur 5** | Arctic Wolf : lien « Experienced a Breach? » sans numéro, caché sur mobile. Advens : bouton flottant « Assistance 24/7 » sans lien d'appel. Dattak : le CERT et son délai dans le contenu. | Un manque direct pour le persona « attaqué ce matin ». |
| Page NIS2 dédiée | **1 sur 5** confirmé | Stoïk /nis2. | Une demande de recherche forte et peu couverte côté MSSP. |

## 4. Insights → Opportunités

| Insight | Opportunité | Impact | Effort |
|---|---|---|---|
| Un seul site sur 5 publie un prix par poste, et le budget est le 2e frein | Grille par poste et simulateur « nombre de postes → €/mois » | H | M |
| Pas de parcours autonome pour le dirigeant | Quiz de 5 questions avec résultat et 3 actions sans e-mail. Rapport complet contre un e-mail | H | M |
| Aucun numéro d'urgence en clair | Bouton « Urgence : nous appeler » fixe sur mobile, numéro dans l'en-tête sur desktop | H | B |
| Le jargon exclut les dirigeants non techniques | Les briques traduites en verbes (« on détecte, on bloque, on vous appelle ») et un glossaire en infobulle | M | B |
| Le récit temporel rassure (Dattak) | Timeline étape par étape avec la personne qui agit à chaque étape | H | M |
| NIS2 est recherchée, la loi est floue | Test « Suis-je concerné ? », checklist datée, page longue SEO | M | M |
| Le discours IA peut inquiéter | Analystes nommés, bloc « Qui sommes-nous » court | M | B |
| Des montants faciles à confondre (Stoïk : 2 Md€ de chiffre d'affaires, 10 M€ de garantie) | Une seule source de prix et de chiffres (composant unique réutilisé partout), chaque montant avec son libellé | M | B |

## 5. Erreurs à éviter

- **Jouer sur la peur** : hacker à capuche, cadenas rouge, code Matrix, compte à rebours.
- **Les acronymes non traduits.**
- **Promettre une conformité NIS2 « garantie »** alors que la loi n'est pas votée et que la conformité dépend aussi de l'entreprise.
- **Afficher des certifications non obtenues** : ISO 27001 et PDIS sont vérifiables. Sur la démo, les emplacements sont marqués « exemple ».
- **Un quiz qui exige l'e-mail avant le score.**
- **Des prix différents selon les pages.**

## 6. Conclusion appliquée à Rempart

- Rempart se positionne comme **« le SOC d'une grande entreprise, au prix et au langage d'une PME »**. Ses trois différenciateurs : prix par poste affiché, numéro d'urgence, quiz utile.
- Le hero promet le résultat. Le CTA principal est « Faire le test (2 min) » et le CTA secondaire « Demander mon diagnostic gratuit ».
- NIS2 suit le format « Suis-je concerné ? » en 3 questions, avec une checklist datée et la mention « transposition française en cours ».
- Les preuves s'affichent dans cet ordre : la timeline (qui agit à chaque étape), le « Qui sommes-nous », les qualifications (emplacements marqués « exemple »), les témoignages fictifs marqués « exemple », les partenaires.
- Le ton est celui du pompier, pas celui de l'alarme.
- On garde le nom Rempart pour la démo, sans dépôt : le site n'est pas commercial et porte la mention « entreprise fictive ». Aucun code visuel n'est emprunté à Stoïk, Dattak ou Advens.

## 7. Questions pour la recherche utilisateur

1. Un dirigeant de PME fait-il confiance à un prix affiché, ou le perçoit-il comme « trop beau, donc incomplet » ? Que doit contenir la mention « ce qui n'est pas inclus » ?
2. Le quiz de 5 questions est-il compris sans aide ? Quelle question fait abandonner ?
3. Quel est le seuil d'acceptation pour laisser son e-mail : après le score, ou pour le rapport seulement ?
4. Qu'est-ce qui rassure le plus : la timeline, la certification ANSSI, le témoignage d'un pair, ou le « Qui sommes-nous » ?
5. Un dirigeant sait-il dire s'il est concerné par NIS2 ? Comprend-il la différence entre être une entité régulée et être fournisseur d'une entité régulée ?
6. Sur mobile, en situation d'urgence simulée, combien de secondes faut-il pour trouver et appeler le numéro ?

## 8. Notes de méthode

- **Sources** : recherches web (novembre 2026) sur les sites des entreprises, la presse spécialisée (JDN, Siècle Digital), des veilles juridiques (Leto, Kiteworks) et les publications publiques (Cybermalveillance.gouv.fr, ANSSI, EUR-Lex). Pages ouvertes et capturées le 2026-11-12 (bench), chiffres de marché et de concurrents revérifiés le 2026-11-13.
- **Limites** :
  - les sites sont vus en capture au-dessus de la ligne de flottaison et en texte : les parcours complets n'ont pas été testés ;
  - le contraste n'est mesuré que sur les boutons cités, le clavier et le lecteur d'écran ne sont pas testés ;
  - les chiffres des entreprises sont déclaratifs ;
  - le statut de NIS2 est celui du 19 octobre 2026 (Leto). Le site affiche « Transposition française en cours, mis à jour le [date de publication] » ;
  - Behance, Pinterest, Land-book et Lapa Ninja sont inaccessibles au navigateur automatisé ; Dribbble, Awwwards et One Page Love sont dans le bench. Aucun intégrateur régional n'est analysé.
- **Échantillon** : 5 sites, 3 français et 2 internationaux. Ce n'est pas représentatif des intégrateurs régionaux, qui sont la cible commerciale du README.
