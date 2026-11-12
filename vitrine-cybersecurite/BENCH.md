# Benchmark : site vitrine Rempart (SOC managé PME, entreprise fictive)

Ce bench suit le brief client bloc par bloc : chaque référence retenue sert une exigence précise de [BRIEF-CLIENT.md](BRIEF-CLIENT.md), les autres sont rangées à côté avec leur raison.

## Limites, à lire en premier

**Vérification du 2026-11-12**, faite avec un vrai navigateur (Chrome piloté par Playwright).

- **Ce qui a été vu** : les 18 références d'origine ont été ouvertes. 18 captures, dont une page de remplacement pour le PDF MonAideCyber, qui ne s'affiche plus. Une capture par référence, en 1440 × 900 px, au-dessus de la ligne de flottaison. Les couleurs et les polices citées ont été relevées dans la page (`getComputedStyle`), pas devinées. Les chiffres cités sont ceux affichés sur la page le 2026-11-12.
- **Corrections** : plusieurs affirmations d'une version antérieure, écrites « d'après la description », étaient fausses. Elles sont corrigées (n° 1, 4, 5, 6, 10, 17 surtout).
- **URL mortes ou redirigées** : le PDF MonAideCyber (n° 4) ne s'affiche plus, il est remplacé par la page du diagnostic en accès libre. La page Dattak n° 7 redirige vers `/fr/insurance`. Le site d'Enshore (n° 23) ne répond plus : seule sa fiche Awwwards a été vue.
- **Galeries** : 8 références (Dribbble, Awwwards, One Page Love). Behance, Land-book, Lapa Ninja, Pinterest et Godly n'ont rien donné : voir « Galeries : requêtes lancées ».
- **Pas vérifié** : le nombre de recommandations du diagnostic MonAideCyber (il faut accepter des CGU, ce qui n'a pas été fait) et le résultat de l'estimateur Coverall (il faut envoyer nom, e-mail et téléphone). Aucun quiz n'a été testé au clavier ni au lecteur d'écran.
- **Bannières cookies** : refusées partout où un refus existait (« Tout refuser », « Refuser », « Continuer sans accepter »). Sur Advens mobile, le widget a été fermé en laissant tous les choix décochés.

**Refonte du 2026-11-12** (même jour, après vérification).

- **Tri** : 17 références sont des inspirations, 12 sont à côté (9 références numérotées et les 3 captures mobiles). Les captures sont rangées dans [`captures/inspis/`](captures/inspis/) et [`captures/a-cote/`](captures/a-cote/), sans changer de nom ni de numéro.
- **Nouvelle organisation** : un tableau de couverture du brief, puis les inspirations rangées par bloc de l'arborescence du brief (section 6), puis les références à côté.
- **Directions** : le brief demande 2 pistes de maquette. La direction A « Tour de contrôle » est retirée (raison dans « Directions »). Il reste B (recommandée) et C.
- **Corrections de tokens** : `semantic.error` passe de `#B42318` (un rouge) à `#9A3412` (rouille), parce que le brief réserve le rouge à l'urgence. Le token `mono` (JetBrains Mono) devient `timestamp` en Manrope, parce que le brief limite la typographie à Manrope ou Plus Jakarta Sans. Le badge « Le plus choisi » devient « Recommandé », parce que Rempart ne peut pas le prouver (brief : pas d'allégations non vérifiables). Un niveau « élevé » manquait pour le quiz : il utilise `semantic.error`. Toutes les autres valeurs ont été recalculées et sont inchangées.
- **Nouvelles références** : aucune. La recherche ciblée sur les blocs sans inspiration (« Ce que couvre l'offre », formulaire de diagnostic) n'a rien donné : Dribbble affiche désormais une vérification « Let's confirm you are human » (non contournée), et les premiers écrans des sections « Pricing Table » et « Contact Form » de One Page Love ne montrent rien d'utilisable pour Rempart.

---

## Couverture du brief

| Exigence du brief | Inspirations | Manque |
|---|---|---|
| 1. Hero (titre, sous-titre, CTA test, CTA diagnostic, numéro d'urgence en haut à droite) | 19, 25, 9 | Aucune référence n'affiche un numéro d'urgence en clair en haut à droite : Arctic Wolf (n° 9) a un lien texte sans numéro. Le duo « test » + « diagnostic » n'a pas été vu. |
| 2. Test express (5 questions, niveau et 3 recommandations sans e-mail, rapport contre e-mail) | 4, 20, 24 | Aucun quiz court à résultat immédiat n'a été vu sur un site réel. Dribbble « security quiz » ne renvoie que des applis de formation sombres. |
| 3. Ce que couvre l'offre (4 cartes, encart « Ce qui n'est pas inclus ») | 10 (partiel) | Aucune référence ne montre 4 cartes de service ni un encart « pas inclus ». Huntress (n° 10) écrit seulement ce qui est inclus. Détail utile chez Advens (n° 17, à côté). |
| 4. En cas d'attaque (timeline en 6 étapes, de T+0 à J+2) | 7, 9 | Aucune timeline minute par minute vue : Dattak découpe en 3 temps. Le format en 6 étapes horodatées est à dessiner. |
| 5. NIS2 expliquée (3 paragraphes, test, checklist PDF datée) | 16, 18, 26 | Aucune checklist PDF datée vue, ni de mention « mis à jour le ». |
| 6. Certifications et partenaires | 13 | Pas de bandeau de logos partenaires technologiques (le repli prévu par le brief sans certification). Advens n° 17 (à côté) montre des logos clients, pas partenaires. |
| 7. Tarifs (3 paliers par poste, simulateur) | 10, 11, 21, 25 | Aucune référence ne montre à la fois 3 paliers chiffrés et un simulateur. Les deux sont à assembler. |
| 8. Contact (bloc urgence 24/7, formulaire de diagnostic) | 8, 9, 23 | Formulaire de diagnostic court (nom, entreprise, postes, téléphone, créneau) : aucune inspiration. Coverall (n° 6, à côté) est le contre-exemple. |
| Page annexe « NIS2 pour les PME » | 16, 26, 18 | Rien. |
| Page annexe « Urgence cyberattaque » | 8 | La mise en page mobile d'une page d'urgence n'a pas été vue. |
| Mobile : bouton d'urgence fixe, 1 tap, trouvé en moins de 5 s | aucune | Le seul bouton fixe vu (Advens mobile, à côté) fait 2,4:1 et n'a pas de lien `tel:`. |
| Mobile : quiz en plein écran | aucune | Aucun quiz affiché sur mobile dans le panel. |
| Marque : marine, blanc cassé, accent cyan, rouge réservé à l'urgence ; jamais de hacker, de cadenas rouge ni de code | 19, 25, 4, 9 | Le secteur est sombre (n° 1, 3, 22 à côté). Aucune référence n'utilise Manrope ni Plus Jakarta Sans. |
| Accessibilité : contraste 4,5:1, niveau jamais par la couleur seule, bouton d'urgence 44 × 44 px | 20 | Contre-exemples de contraste : Dattak 3,9:1 (n° 3), bouton Advens 2,4:1 (n° 13). Clavier et lecteur d'écran non testés. |
| Preuve : photo réelle de l'équipe, nombre d'analystes, localisation du SOC | 23 | Aucune photo d'équipe claire, en lumière du jour. Arctic Wolf (n° 15) et Stoïk (n° 2) sont à côté, avec renvoi. |
| Preuve : timeline et délai moyen de prise en charge | 7, 9 | Voir bloc 4. |
| Preuve : grille par poste et simulateur | 10, 21 | Voir bloc 7. |
| Preuve : test « Suis-je concerné ? » et checklist datée | 16 | Checklist datée : voir bloc 5. |
| Preuve : certifications justifiées | 13 | Rien. |
| Preuve : 3 témoignages (nom, fonction, secteur, taille) | 14 | Le secteur et la taille d'entreprise ne sont pas affichés chez Dattak. |
| Réglementaire : pas d'allégations non vérifiables, chiffres sourcés | 18, 26 | Rien. |

---

## Inspirations, bloc par bloc

Les numéros sont ceux du bench d'origine. Une référence peut apparaître dans plusieurs blocs.

### 1. Hero

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 19 | [Latch : Cybersecurity Landing Page (Dipa Inhouse)](https://dribbble.com/shots/27193953-Latch-Cybersecurity-Landing-Page), Dribbble | [capture](captures/inspis/19-dribbble-latch.jpg) | L'une des rares maquettes claires de la recherche : fond blanc bleuté, titre fin centré, bouton pastille bleu, beaucoup d'air. Plus bas, la photo d'une personne souriante. | Ton rassurant et pédagogique, fond blanc cassé dominant. |
| 25 | [Steadily (assurance de bailleurs)](https://onepagelove.com/steadily), One Page Love (publié le 16 juin 2022) | [capture](captures/inspis/25-onepagelove-steadily.jpg) | Fond crème, titre « Get fast, affordable landlord insurance », un seul champ (l'adresse) et un bouton « Get a quote », illustration au trait (main, téléphone avec un devis à 60 $ par mois, maison), logos presse puis avis 5 étoiles. | Un service de protection présenté sans image de menace ; illustrations au trait fournies par l'agence (« schémas, pas de personnages menaçants »). |
| 9 | [Arctic Wolf : How it works](https://arcticwolf.com/how-it-works/), site réel (US) | [capture](captures/inspis/09-arcticwolf-how.jpg) | Un lien « Experienced a Breach? » dans l'en-tête, visible sur desktop. | Numéro d'urgence en haut à droite. Chez Rempart, le numéro lui-même, cliquable, en rouge discret. |

À éviter : la serif de titre de Steadily (Faustina), le bouclier-serrure 3D de Latch (cousin du cadenas). Détails pris chez des références à côté : la mention géographique du SOC (Stoïk n° 2) et le bouton cyan à texte sombre (Huntress n° 1).

### 2. Test express

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 4 | [MonAideCyber (ANSSI) : diagnostic en accès libre](https://monaide.cyber.gouv.fr/diagnostic-libre-acces), site public. PDF d'origine mort : https://monaidecyber.ssi.gouv.fr/fichiers/Plaquette_MonAideCyber.pdf | [capture](captures/inspis/04-monaidecyber-diagnostic.jpg) | Charte de l'État (police Marianne), illustration au trait d'une personne devant un écran. Aucun e-mail pour commencer. Un lien propose un diagnostic accompagné. | Résultat sans e-mail ; illustration non menaçante. Le lien vers un diagnostic accompagné correspond au CTA « Demander mon diagnostic gratuit ». |
| 20 | [Ghost UI risk score widget (Evil Martians)](https://dribbble.com/shots/24816320-Ghost-UI-risk-score-widget), Dribbble | [capture](captures/inspis/20-dribbble-risk-score.jpg) | Une jauge en arc, un chiffre (2.9), un libellé (« Low ») et une légende (« Median app risk »). Le niveau ne passe jamais par la couleur seule. | Niveau faible, moyen ou élevé, affiché avec un libellé et une phrase. Chez Rempart, sur fond clair. |
| 24 | [SAFE security](https://www.awwwards.com/sites/safe-security-1), Awwwards (mention honorable) | [capture](captures/inspis/24-awwwards-safe.jpg) | Version primée : fond marine, un score « 3.14, Risk: Low » dans un nuage de points cyan, bouton cyan. Le site actuel a changé (fond noir et violet, autre message). | Le score et son libellé côte à côte, en écho au résultat du quiz (direction C). |

À éviter : la case CGU obligatoire avant la première question (MonAideCyber). Le consentement explicite du brief porte sur l'envoi du rapport, pas sur le démarrage.

### 3. Ce que couvre l'offre

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 10 | [Huntress : Pricing](https://www.huntress.com/pricing), site réel (US) | [capture](captures/inspis/10-huntress-pricing.jpg) | Les puces du hero : « No confusing tiers, add-ons, or expensive bundles. », « 24/7 SOC Management included at no additional cost. » | Dire en clair ce qui est inclus (persona Karim : « ce qui est couvert, ce qui ne l'est pas »). |

Manque : ni les 4 cartes, ni l'encart « Ce qui n'est pas inclus ». Détail utile chez Advens (n° 17, à côté) : « un même plan de surveillance, un même analyste », qui illustre le SOC Manager attitré.

### 4. En cas d'attaque

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 7 | [Dattak : Assurance Cyber Proactive](https://www.dattak.io/fr/cyberattack) (redirige vers /fr/insurance), site réel (FR) | [capture](captures/inspis/07-dattak-cyberattack.jpg) | Le découpage « Avant l'incident », « Pendant l'incident », « Après l'incident », avec deux délais chiffrés : « scan et analyse en 5 minutes », « intervention en moyenne en moins de 2 minutes ». | Timeline et délai moyen de prise en charge (preuve « On agit, on ne fait pas qu'alerter »). |
| 9 | [Arctic Wolf : How it works](https://arcticwolf.com/how-it-works/), site réel (US) | [capture](captures/inspis/09-arcticwolf-how.jpg) | Le « Concierge Delivery Model » montre qui agit (alertes triées, conseils suivis). Sous le hero, 5 chiffres dont « <1 actionable event per day ». | Nommer qui agit à chaque étape de la timeline ; un chiffre qui parle au dirigeant. |

À éviter : le hero sombre de Dattak. Chez Rempart, la timeline peut vivre dans une section marine (`bg.inverse`), le reste de la page restant clair.

### 5. NIS2 expliquée

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 16 | [Stoïk : NIS2](https://www.stoik.com/nis2), site réel (FR) | [capture](captures/inspis/16-stoik-nis2.jpg) | Un titre-question, « Êtes-vous concerné par NIS2 ? », un chiffre (environ 160 000 entités européennes) et le bouton « Vérifier si je suis concerné ». Intertitres en langage courant : « Réglons d'abord le point qui fâche. », « Une directive, pas un règlement. ». | Test « Suis-je concerné ? » ; « NIS2 sans jargon ». |
| 18 | [Cybermalveillance.gouv.fr : infographie maturité TPE-PME 2025](https://www.cybermalveillance.gouv.fr/medias/2025/10/250910_InfographieMaturiteCyberTPE-PME_SCREEN.pdf), PDF public de 2 pages | [capture](captures/inspis/18-cybermalveillance-infographie.jpg) | Chiffres en jauges : 16 % des entreprises se déclarent victimes d'au moins un incident, 80 % ne sont pas préparées, 3 TPE-PME sur 4 investissent moins de 2 000 € par an. Source en pied : enquête OpinionWay, 588 entreprises de moins de 250 salariés, juin et juillet 2025. | 2 ou 3 chiffres officiels avec leur source écrite (pas d'allégation non vérifiable). |
| 26 | [The State of Software Delivery in Healthcare (Thoughtbot)](https://onepagelove.com/the-state-of-software-delivery-in-healthcare), One Page Love | [capture](captures/inspis/26-onepagelove-thoughtbot.jpg) | Sections blanc cassé, grands pourcentages et graphiques, méthode d'enquête écrite. | Mise en scène des chiffres sourcés de la section NIS2. |

À éviter : le cadenas rouge ouvert qui illustre le 16 % (n° 18), le fond brun sombre et la serif de Thoughtbot.

### 6. Certifications et partenaires

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 13 | [Advens : qualification PDIS](https://www.advens.com/media/news-advens/qualification-pdis/), site réel (FR) | [capture](captures/inspis/13-advens-pdis.jpg) | Article du 30 septembre 2025. Hero bleu très clair `#E6F6FF`, titre Space Grotesk 700 en `#1F1F1F`, visuel du « Visa de sécurité » de l'ANSSI, lien vers la qualification dans le texte. | Certifications justifiées : logo officiel et lien vers le justificatif (placeholders sur la démo, « uniquement si obtenues »). |

À éviter : le bouton flottant « Assistance 24/7 » de la même page, texte blanc sur `#0AB3FF` à 2,4:1.

### 7. Tarifs

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 10 | [Huntress : Pricing](https://www.huntress.com/pricing), site réel (US) | [capture](captures/inspis/10-huntress-pricing.jpg) | Plus bas que la capture : Managed EDR à 8,99 $ par poste et par mois, ITDR à 4,80 $ par identité, prix catalogue dégressif, SOC 24/7 inclus. | Prix unitaire public par poste ; « un prix clair, sans surprise ». |
| 11 | [Arctic Wolf : Bundles](https://arcticwolf.com/solutions/bundles/), site réel (US) | [capture](captures/inspis/11-arcticwolf-bundles.jpg) | 3 paliers Core, Plus et Total, avec des options de garantie financière chiffrées (à partir de 100 k$). | 3 paliers (Essentiel, Pro, NIS2) avec une ligne d'engagement par palier. |
| 21 | [B2B SaaS Pricing Page UX (Katerina Bulkina)](https://dribbble.com/shots/27813140-B2B-SaaS-Pricing-Page-UX-for-Plans-Trials-Enterpris), Dribbble | [capture](captures/inspis/21-dribbble-pricing-seat.jpg) | « Pay per seat. Talk to us when you need more control. », 12 $ par siège et par mois, le total annuel et le prix mensuel écrits sous le montant, « See your estimate below before you start ». | Simulateur « nombre de postes → prix mensuel », estimation avant tout engagement. |
| 25 | [Steadily](https://onepagelove.com/steadily), One Page Love | [capture](captures/inspis/25-onepagelove-steadily.jpg) | Un seul champ, puis un prix (devis à 60 $ par mois dans l'illustration). | Le simulateur de Rempart : 1 champ (postes), le prix tout de suite, aucune coordonnée. |

À éviter : le formulaire « Get pricing » au-dessus de prix pourtant publics (n° 10), des paliers sans prix (n° 11), le dégradé violet et le jaune fluo (n° 21). Détails pris chez des références à côté : la FAQ prix avec hypothèses écrites (Stoïk n° 12) et la promesse « fourchette instantanée » (Coverall n° 6).

### 8. Contact

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 8 | [Dattak : gestes des premières heures](https://www.dattak.io/fr/blog/dattak-blog-gestes-cyberattaque-reponse-incident), blog (FR) | [capture](captures/inspis/08-dattak-blog-gestes.jpg) | Article du 25 novembre 2025. Gestes : déconnecter les systèmes compromis, isoler les sauvegardes, couper internet si nécessaire. Erreurs citées : redémarrer trop tôt, payer une rançon sans accompagnement juridique, agir seul. Résumé : « Déconnecter, isoler, documenter ». | Bloc « Les 3 réflexes en attendant notre appel » à côté du numéro d'urgence (persona Laurent). |
| 9 | [Arctic Wolf : How it works](https://arcticwolf.com/how-it-works/), site réel (US) | [capture](captures/inspis/09-arcticwolf-how.jpg) | Le lien d'urgence est dans l'en-tête, hors du formulaire de contact. | Séparer le bloc urgence du formulaire de diagnostic. |
| 23 | [Enshore Security (Ricardo Dol)](https://www.awwwards.com/sites/enshore-security), Awwwards (nominé, décembre 2023) | [capture](captures/inspis/23-awwwards-enshore.jpg) | Plus bas dans l'aperçu (la capture ne montre que le hero) : un encart « Laissez-nous vous aider » avec 2 auditeurs nommés, en photo, avec leur qualification, à côté de 3 chiffres de volume (1 500+ audits internes, 400+ audits de certification, 30+ ISMS gérés). | « Un interlocuteur humain » (persona Claire) ; preuve « nombre d'analystes ». |

À éviter : le cadenas et le point d'exclamation rouge de l'infographie Dattak, la Terre vue de l'espace d'Enshore. Le formulaire de diagnostic n'a pas d'inspiration : Coverall (n° 6, à côté) montre ce qu'il ne faut pas faire.

### Pages annexes

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 16 | [Stoïk : NIS2](https://www.stoik.com/nis2) | [capture](captures/inspis/16-stoik-nis2.jpg) | Le ton des intertitres. | Page « NIS2 pour les PME » (version longue, cible SEO). |
| 26 | [Thoughtbot](https://onepagelove.com/the-state-of-software-delivery-in-healthcare) | [capture](captures/inspis/26-onepagelove-thoughtbot.jpg) | Rapport en une page, méthode écrite. | Page « NIS2 pour les PME ». |
| 8 | [Dattak : gestes](https://www.dattak.io/fr/blog/dattak-blog-gestes-cyberattaque-reponse-incident) | [capture](captures/inspis/08-dattak-blog-gestes.jpg) | Les gestes et les erreurs à éviter. | Page « Urgence cyberattaque » (recherche mobile). |

### Preuves sans bloc dédié (section 5 du brief)

Le brief demande 3 témoignages et une photo réelle de l'équipe, mais aucun bloc de l'arborescence ne les accueille (voir « Points à remonter au client »).

| # | Référence | Capture | Ce qu'on reprend | Pour quelle exigence du brief |
|---|---|---|---|---|
| 14 | [Dattak : Témoignages](https://www.dattak.io/fr/temoignages), site réel (FR) | [capture](captures/inspis/14-dattak-temoignages.jpg) | Chaque témoignage est une carte : vidéo à gauche, citation d'une phrase en italique, nom, fonction et entreprise. | « Des PME comme vous » : 3 témoignages courts sur la home, page complète en lien, vidéo en option. Ajouter secteur et taille. |
| 23 | [Enshore Security](https://www.awwwards.com/sites/enshore-security) | [capture](captures/inspis/23-awwwards-enshore.jpg) | Chiffres et visages nommés dans le même bloc. | « Surveillé 24 h/24 par des humains, en France » : photo réelle et nombre d'analystes. |

Détail pris chez une référence à côté : de vraies photos d'analystes plutôt que des hackers à capuche (Arctic Wolf n° 15), mais claires, en lumière du jour.

---

## Mobile

Trois sites vus en 390 × 844 px. Les trois captures sont à côté : aucune ne respecte les exigences mobiles du brief, mais chacune apprend quelque chose.

| Site | Capture | Ce qu'on observe | Exigence du brief concernée |
|---|---|---|---|
| Stoïk : Cybersécurité | [capture](captures/a-cote/mobile-stoik.jpg) | Le hero bleu tient sur l'écran, les 2 boutons passent l'un sous l'autre en pleine largeur, « Devenir partenaire » en premier. Aucun numéro ni bouton d'urgence, aucun élément fixe. | Numéro joignable en 1 tap depuis n'importe quel écran : absent. |
| Advens : offres mySOC | [capture](captures/a-cote/mobile-advens.jpg) | Le seul site du panel avec un bouton d'urgence fixe sur mobile : la pastille « Assistance 24/7 » reste en bas à droite pendant le défilement. Mais son contraste est de 2,4:1 et la page n'a aucun lien `tel:` : le bouton ne lance pas d'appel. | Bon emplacement ; échoue sur le 1 tap et sur le contraste 4,5:1. |
| Arctic Wolf : How it works | [capture](captures/a-cote/mobile-arcticwolf.jpg) | Les 5 chiffres passent en grille de 2 colonnes. Le lien « Experienced a Breach? », visible dans l'en-tête sur desktop, disparaît dans le menu burger sur mobile. | Numéro trouvé en moins de 5 s : un lien caché dans le menu échoue. |

Ce que ces observations donnent pour Rempart :
- une barre d'urgence fixe en bas (« Urgence : appeler le 0X XX XX XX XX », rouge discret). Elle porte un vrai lien `tel:`, mesure au moins 44 px de haut et a un contraste d'au moins 4,5:1 (blanc sur `#C8102E` : 5,9:1). Elle ne se cache jamais dans le menu (critère de réussite : 1 tap depuis n'importe quel écran) ;
- un quiz en plein écran, une question par écran, une barre de progression, un bouton retour. Aucune page vue n'affiche de quiz directement (Stoïk renvoie vers un test NIS2 par un bouton) : c'est un point de différence ;
- une grille tarifaire en carrousel horizontal avec le palier « Pro » centré par défaut (tâche du test utilisateur : trouver le prix pour 80 postes) ;
- les chiffres clés en grille de 2 colonnes, comme Arctic Wolf.

---

## Directions

Le brief demande 2 pistes de maquette, au ton « rassurant et pédagogique ».

**Constats après observation (2026-11-12)**
- Le panel sectoriel est sombre : Huntress (`#050707`), Arctic Wolf (`#00112C`) et Dattak (noir vers marine) ont un hero sombre, Stoïk un bleu saturé. Seuls Advens (article PDIS, `#E6F6FF`) et MonAideCyber ont un hero clair. Sur Dribbble, environ trois quarts des vignettes « cybersecurity landing page » sont sombres.
- Aucun concurrent ne montre un prix sans demander de coordonnées en premier (Huntress cache ses prix sous un formulaire, Coverall exige 7 champs, Arctic Wolf n'affiche pas de prix). Le simulateur sans e-mail de Rempart est un argument de différence.

**Direction retirée : A « Tour de contrôle »** (fond marine profond dominant, données en cyan). Le brief ne demande que 2 pistes, et A est la seule dont les références (Huntress n° 1, Arctic Wolf SOC n° 15) relèvent du registre sombre et dramatique que le brief écarte (« aucune image ni formulation anxiogène »). Ses bons éléments passent dans B : la timeline dans une section marine (`bg.inverse`) et les horodatages précis.

**Piste 1 : B « Le cabinet de confiance »** (recommandée)
- Fond blanc cassé dominant, marine pour la structure, cyan en touches sur fond marine seulement.
- Un ton de médecin de famille : schémas simples, illustrations au trait, beaucoup d'air.
- C'est la plus cohérente avec « rassurant et pédagogique » et avec la cible de dirigeants non techniques. Elle se démarque aussi d'un secteur sombre.
- Inspirations : Steadily (n° 25) pour le hero et le champ unique, Latch (n° 19) pour la clarté, MonAideCyber (n° 4) pour l'illustration, Thoughtbot (n° 26) et Cybermalveillance (n° 18) pour les chiffres sourcés, Dattak (n° 14) pour les témoignages.

**Piste 2 : C « Le tableau de bord »**
- Des cartes façon interface sur fond blanc cassé (score de risque, statut « surveillé »), des micro-interactions sobres.
- Le produit est montré comme il sera vécu, avec le score du quiz en écho.
- Le risque est de faire « éditeur SaaS » plutôt que service humain, ce qui affaiblirait le message « surveillé par des humains, en France ». On le compense par les visages nommés des analystes à côté des cartes (n° 23).
- Inspirations : la jauge Evil Martians (n° 20), le score SAFE (n° 24), les chiffres d'Arctic Wolf (n° 9).

**3 choses à ne pas faire**
1. Pas de hacker à capuche, de cadenas rouge, de code Matrix ni de compte à rebours anxiogène.
2. Pas de rouge hors urgence : sinon il ne signale plus rien.
3. Pas de quiz qui exige l'e-mail avant d'afficher le score.

---

## Palette, polices, design tokens, composants

Contrastes calculés selon la formule WCAG 2.1, recalculés le 2026-11-12. Le fond de référence est `bg.default` (`#F7F5F0`). Chaque valeur a été vérifiée contre les contraintes du brief (marine, blanc cassé, accent cyan, rouge réservé à l'urgence, Manrope ou Plus Jakarta Sans, contraste 4,5:1, cyan clair jamais en texte sur fond clair).

### Palette recommandée

| Rôle | Hex | Usage |
|---|---|---|
| Marine | `#0B1F3A` | Titres, fonds sombres. Contraste de 15,2:1 sur blanc cassé |
| Blanc cassé | `#F7F5F0` | Fond principal |
| Texte | `#1E293B` | Corps de texte (13,4:1) |
| Texte secondaire | `#5B6B80` | Légendes (5,0:1) |
| Cyan accent | `#00B8D9` | Accent sur fond marine seulement (7,0:1). Jamais pour du texte sur fond clair |
| Cyan texte | `#006B85` | Liens et accent sur fond clair (5,6:1) |
| Rouge urgence | `#C8102E` | Bouton et numéro d'urgence uniquement. Blanc sur rouge : 5,9:1 |

Observé chez Huntress (n° 1, à côté) : un bouton cyan à texte sombre. L'équivalent Rempart (texte marine sur `#00B8D9`) fait 7,0:1. Il peut servir de CTA dans les sections sombres, sans nouveau token.

### Polices Google Fonts

- **Manrope** (600 à 800) pour les titres, **Manrope** (400 et 500) pour le texte. Une seule famille, rapide à charger (LCP inférieur à 2,5 s).
- Alternative : **Plus Jakarta Sans** pour les titres.
- **Corrigé** : JetBrains Mono n'est plus proposé pour les horodatages de la timeline. Le brief limite la typographie à Manrope ou Plus Jakarta Sans. Les horodatages (« T+05 min ») passent en Manrope 600 avec `font-variant-numeric: tabular-nums` (vérifié le 2026-11-12 sur le Manrope de Google Fonts : avec `tabular-nums`, « 1111 » et « 0000 » ont la même largeur).
- Observé : les références les plus rassurantes des galeries (n° 25, 26) titrent en serif. Le brief impose une grotesque : on ne reprend pas la serif.

### Couleurs

| Token | Hex | Usage | Contraste |
|---|---|---|---|
| `brand.navy` | `#0B1F3A` | Titres, fonds sombres, bouton primaire | 15,2:1 sur bg |
| `brand.navy-hover` | `#132E54` | Survol du bouton primaire | 12,5:1 |
| `brand.cyan` | `#00B8D9` | Accent sur fond navy uniquement | 7,0:1 sur navy, **2,2:1 sur bg, donc jamais en texte clair** |
| `brand.cyan-text` | `#006B85` | Liens et accent sur fond clair | 5,6:1 |
| `semantic.urgent` | `#C8102E` | Bouton et numéro d'urgence **uniquement** | 5,4:1. Blanc sur rouge : 5,9:1 |
| `semantic.error` | `#9A3412` | Erreurs de formulaire, niveau de risque « élevé ». **Corrigé** : était `#B42318`, un rouge, alors que le brief réserve le rouge à l'urgence | 6,7:1 |
| `semantic.success` | `#15803D` | Confirmation, niveau de risque « faible » | 4,6:1 |
| `semantic.warning` | `#B45309` | Niveau de risque « moyen », avertissements | 4,6:1 |
| `neutral.900` | `#1E293B` | Corps de texte | 13,4:1 |
| `neutral.600` | `#5B6B80` | Texte secondaire | 5,0:1 |
| `neutral.400` | `#7A8699` | Bordures de champs (contraste non textuel ≥ 3:1) | 3,4:1 |
| `neutral.200` | `#E2E0D8` | Séparateurs décoratifs | décoratif |
| `bg.default` | `#F7F5F0` | Fond de page | sans objet |
| `bg.surface` | `#FFFFFF` | Cartes, champs | sans objet |
| `bg.inverse` | `#0B1F3A` | Sections sombres (timeline, footer) | sans objet |

Le niveau de risque du quiz ne doit jamais être signalé par la couleur seule : chaque niveau porte aussi un libellé et une icône. C'est d'autant plus nécessaire que `semantic.warning` et `semantic.error` sont deux teintes proches.

### Typographie (Manrope)

| Token | Taille (mobile / desktop) | Graisse | Interligne |
|---|---|---|---|
| `display` | 36 / 56 px | 800 | 1,1 |
| `h1` | 30 / 44 px | 800 | 1,15 |
| `h2` | 24 / 32 px | 700 | 1,2 |
| `h3` | 20 / 24 px | 700 | 1,3 |
| `body-lg` | 18 / 20 px | 400 | 1,6 |
| `body` | 16 / 17 px | 400 | 1,6 |
| `small` | 14 px | 500 | 1,5 |
| `timestamp` (timeline) | 14 / 15 px | 600, chiffres tabulaires | 1,4 |

### Espacement, rayons, ombres, motion

| Catégorie | Tokens |
|---|---|
| Espacement (base 4) | `space.1`=4, `2`=8, `3`=12, `4`=16, `6`=24, `8`=32, `12`=48, `16`=64, `24`=96 px. Sections : 64 px en mobile, 96 px en desktop |
| Rayons | `radius.sm`=6 px (champs), `radius.md`=10 px (boutons), `radius.lg`=16 px (cartes), `radius.full` (pastilles) |
| Ombres | `shadow.sm` = 0 1px 2px rgba(11,31,58,.08) ; `shadow.md` = 0 4px 16px rgba(11,31,58,.10) ; `shadow.focus` = 0 0 0 3px #006B85 |
| Motion | `duration.fast`=120 ms (survol), `duration.base`=200 ms (ouverture, transitions du quiz), `duration.slow`=320 ms (révélation du score). `ease.out` = cubic-bezier(.2,.8,.2,1), `ease.in-out` = cubic-bezier(.4,0,.2,1). Respecter `prefers-reduced-motion` : animations remplacées par un fondu de 0 ms |

### Composants clés

**Bouton primaire** : fond `brand.navy`, texte blanc, `radius.md`, hauteur 48 px (44 px minimum).
- Survol : `brand.navy-hover`.
- Focus : `shadow.focus` visible.
- Actif : translateY(1px).
- Désactivé : opacité 0,5, `aria-disabled`, curseur not-allowed.
- Chargement : spinner et libellé « Envoi… ».

**Bouton secondaire** : fond transparent, bordure de 1,5 px `brand.navy`, texte navy. Mêmes états. Survol : fond `#0B1F3A0D`.

**Bouton urgence** : fond `semantic.urgent`, texte blanc, icône téléphone et numéro visible, lien `tel:`, 44 × 44 px minimum. Fixe en bas sur mobile, en haut à droite dans l'en-tête sur desktop.

**Carte d'offre** : fond `bg.surface`, `radius.lg`, `shadow.sm`, padding `space.6`. Elle contient une icône au trait, un titre `h3`, 3 puces et un lien. Au survol : `shadow.md`. L'encart « Ce qui n'est pas inclus » suit les 4 cartes, sur fond `bg.default` avec une bordure `neutral.400`.

**Carte de tarif** : le palier mis en avant porte une bordure de 2 px `brand.cyan-text` et un badge « Recommandé ». **Corrigé** : le badge disait « Le plus choisi », une allégation que Rempart ne peut pas prouver sur la démo.

**Formulaire et quiz** :
- labels visibles au-dessus des champs, hauteur 48 px, bordure `neutral.400` ;
- erreur affichée sous le champ en `semantic.error`, avec icône et texte, et `aria-describedby` ;
- quiz : une question par écran, barre de progression « 2/5 », gros boutons-réponses en cartes, bouton Retour, navigable au clavier.

| À faire | À ne pas faire |
|---|---|
| Un seul bouton primaire par écran | Deux boutons primaires concurrents dans le hero |
| Le rouge réservé à l'urgence, l'erreur en rouille | Le rouge pour les erreurs, la décoration ou les badges promotionnels |
| Le cyan en accent sur fond navy | Du texte cyan clair sur blanc cassé (2,2:1) |
| Le score du quiz avec un libellé, une couleur et une icône | Le score signalé par la couleur seule |
| Des labels visibles et une erreur expliquée sous le champ | Les placeholders utilisés comme labels, ou « Champ invalide » |
| Un focus visible sur tous les éléments interactifs | `outline: none` sans remplacement |
| Les animations désactivées avec `prefers-reduced-motion` | Un compteur ou un radar animé en boucle |

---

## À côté

Ces références restent consultables. Leur détail utile, quand il y en a un, est cité dans le bloc concerné.

| # | Référence | Capture | Pourquoi à côté |
|---|---|---|---|
| 1 | [Huntress : Why Huntress](https://www.huntress.com/why-huntress), site réel (US) | [capture](captures/a-cote/01-huntress.jpg) | Hors du ton du brief (« rassurant et pédagogique », aucune image anxiogène) : fond quasi noir `#050707`, titre en capitales Archivo Black 56 px, photo de salle serveurs aux néons cyan et magenta. Il n'y a pas de chiffres sous le titre : « 285,000 businesses » n'apparaît que plus bas, et « déployé en moins de 20 minutes » dans un paragraphe. Seul détail utile : le bouton cyan `#00DBE5` à texte noir (11,8:1), voir « Palette ». |
| 2 | [Stoïk : Cybersécurité](https://www.stoik.com/cybersecurite), site réel (FR) | [capture](captures/a-cote/02-stoik-cybersecurite.jpg) | Hors de la marque du brief : grande carte bleu saturé `#1362DD`, titre fin Lazzer avec « 360° » en rose. Le premier bouton est « Devenir partenaire », avant « Se protéger », alors que le brief veut le test en CTA principal. Seul détail utile : « 24h/7j de surveillance par un SOC européen internalisé », voir bloc 1 (Rempart dira « en France »). |
| 3 | [Dattak : accueil](https://www.dattak.io/fr), site réel (FR) | [capture](captures/a-cote/03-dattak.jpg) | Contre-exemple. Le titre reste une catégorie (« Dattak réduit et assure les risques technologiques des entreprises ») alors que le brief veut un titre qui nomme le résultat pour le dirigeant. Bouton terracotta `#C4684A` à texte blanc : 3,9:1, sous le seuil AA du brief. Hero sombre, titre Inter 79 px. |
| 5 | [Stoïk : Assurance](https://www.stoik.com/assurance), site réel (FR) | [capture](captures/a-cote/05-stoik-assurance.jpg) | Contexte sectoriel seulement (assurance) : les deux boutons visent les courtiers, et la 2e ligne du titre est en rose, hors marque. Aucun scan gratuit sur cette page (les scans sont « inclus dans chaque police »). Seul détail utile : 3 chiffres en pastilles sous le hero (2 Md€, 10 M€, 150 M€). |
| 6 | [Coverall : estimateur](https://www.coverall.com/commercial-cleaning-services/janitorial/), site réel (US, nettoyage) | [capture](captures/a-cote/06-coverall.jpg) | Contre-exemple pour le simulateur : le bloc « Get an instant cleaning quote » est un formulaire de 10 champs (7 obligatoires, dont nom, e-mail, téléphone et code postal) avant toute fourchette, plus un reCAPTCHA. Le brief demande un prix sans coordonnées, des formulaires minimaux (RGPD) et pas de reCAPTCHA intrusif. Seul détail utile : la promesse écrite « fourchette instantanée selon la surface et la fréquence », voir bloc 7. |
| 12 | [Stoïk : prix d'une cyber assurance](https://www.stoik.com/prix-assurance-cyber), blog (FR) | [capture](captures/a-cote/12-stoik-prix.jpg) | Contexte sectoriel seulement (prix d'assurance, pas de SOC), article daté du 14 juin 2023, photo de banque d'images (le brief exclut la banque d'images pour l'équipe). Seul détail utile : des prix d'appel par secteur (de 115 à 172 € par mois) avec leurs hypothèses écrites, voir bloc 7. |
| 15 | [Arctic Wolf : Inside the SOC](https://arcticwolf.com/uk/inside-the-soc/), site réel (UK) | [capture](captures/a-cote/15-arcticwolf-soc.jpg) | Traitement anxiogène, contraire au brief : photo très assombrie, « SOC » en lettres géantes, boutons orange. Seul détail utile : une vraie photo d'analyste au casque à la place des hackers à capuche, voir « Preuves sans bloc dédié ». |
| 17 | [Advens : offres mySOC](https://www.advens.com/mysoc/offres/), site réel (FR) | [capture](captures/a-cote/17-advens-mysoc.jpg) | Ne sert pas le bloc Tarifs : pas de paliers nommés ni de prix, l'offre est une trajectoire en 3 phases (schéma en image), puis 3 valeurs (Efficient, Adaptatif, Collaboratif). Bandeau noir, titre bleu `#006BFF` en Space Grotesk 56 px. Seul détail utile : « un même plan de surveillance, un même analyste », voir bloc 3. |
| 22 | [Cybersecurity Landing Page (FleexStudio)](https://dribbble.com/shots/26361362-Cybersecurity-Landing-Page), Dribbble | [capture](captures/a-cote/22-dribbble-contre-exemple.jpg) | Contre-exemple : cadenas vert néon, main robotique, silhouette à capuche, fond noir. Il coche le premier interdit du brief (« jamais de hacker à capuche »). Il représente bien la recherche : environ trois quarts des vignettes « cybersecurity landing page » sont sombres. |
| mobile | [Stoïk : Cybersécurité, mobile](https://www.stoik.com/cybersecurite) | [capture](captures/a-cote/mobile-stoik.jpg) | Aucun numéro ni bouton d'urgence, alors que le brief exige un numéro joignable en 1 tap depuis n'importe quel écran mobile. Voir « Mobile ». |
| mobile | [Advens : offres mySOC, mobile](https://www.advens.com/mysoc/offres/) | [capture](captures/a-cote/mobile-advens.jpg) | Le bouton fixe « Assistance 24/7 » est au bon endroit, mais il fait 2,4:1 (brief : 4,5:1) et ne lance pas d'appel (aucun lien `tel:`). Voir « Mobile ». |
| mobile | [Arctic Wolf : How it works, mobile](https://arcticwolf.com/how-it-works/) | [capture](captures/a-cote/mobile-arcticwolf.jpg) | Le lien d'urgence disparaît dans le menu burger, alors que le brief veut le numéro trouvé en moins de 5 s. Seul détail utile : les chiffres en grille de 2 colonnes, voir « Mobile ». |

---

## Galeries : requêtes lancées

| Plateforme | Requêtes | Résultat |
|---|---|---|
| Behance | « cybersecurity landing page » | Inaccessible : la page renvoie « HTTP ERROR 400 » au navigateur automatisé. |
| Dribbble | « cybersecurity landing page », « risk score quiz », « pricing per seat », « security quiz », « managed security services website » | 4 retenues au départ (n° 19 à 22). Après tri : 3 inspirations, 1 à côté (n° 22). « security quiz » ne renvoie que des applis de formation sombres. |
| Dribbble (refonte, 2026-11-12) | « included not included pricing » | Inaccessible : une vérification « Let's confirm you are human » s'affiche. Non contournée. |
| Pinterest | « cybersecurity web design navy cyan » | Inaccessible sans compte : une fenêtre de connexion couvre les résultats et aucune URL d'épingle n'est exposée. Derrière, les vignettes sont presque toutes marine, avec boucliers et cadenas. |
| Awwwards | « cybersecurity », « security », « security saas » | 2 retenues (n° 23, 24). Beaucoup de sites primés ont changé ou ont disparu depuis. |
| Land-book | « security » | Inaccessible (protection anti-robots, challenge Cloudflare). |
| Lapa Ninja | « security », catégorie security | Inaccessible (protection anti-robots, « Sorry, you have been blocked »). |
| One Page Love | « security », « cyber », « insurance » | 2 retenues (n° 25, 26). « security » donne surtout des gabarits sombres (Retinax, œil en gros plan : contre-exemple). |
| One Page Love (refonte, 2026-11-12) | recherche « pricing », sections « Pricing Table » (338 exemples) et « Contact Form » (310 exemples), premiers écrans | Rien de retenu : pas d'encart « ce qui n'est pas inclus », et les formulaires de contact vus sont surtout des portfolios. |
| Godly | page d'accueil, « Websites » | Rien de retenu : pas de recherche ni de catégorie « security » sans compte, godly.website redirige vers recent.design et les fiches renvoient vers l'accueil. |

---

## Points à remonter au client

- **Témoignages et photo d'équipe sans bloc** : la section 5 du brief exige 3 témoignages et une photo réelle de l'équipe, mais l'arborescence (section 6) ne leur donne pas de place. Proposition : les placer dans le bloc 6, renommé « Preuves : équipe, certifications, témoignages », ou ajouter un bloc entre 6 et 7.
- **Rouge réservé à l'urgence** : appliquée à la lettre, la règle exclut le rouge des erreurs de formulaire et du niveau « élevé » du quiz, alors que c'est une convention que les visiteurs reconnaissent. Le bench applique la règle (rouille `#9A3412`, toujours avec icône et texte). À confirmer avec le client.
- **Statut de la transposition NIS2** : le brief attend la loi « Résilience » pour fin 2026. Le bench ne l'a pas vérifié. La mention « Transposition française en cours, mis à jour le [date] » et la checklist PDF sont à revérifier juste avant la mise en ligne.
