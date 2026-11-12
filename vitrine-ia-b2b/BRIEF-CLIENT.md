# Brief client : site vitrine Ordo

> **Document de démonstration.** Ordo est une entreprise FICTIVE créée pour illustrer la catégorie `vitrine-ia-b2b`. Ses chiffres, sa levée, ses clients et ses personnes sont inventés. Le nom est provisoire : vérifier sa disponibilité à l'INPI avant toute réutilisation.

**Émetteur** : Ordo SAS (fictif), direction marketing
**Destinataire** : l'agence
**Date** : novembre 2026
**Version** : 1.0

---

## 1. Qui nous sommes

Ordo déploie des agents IA qui traitent les factures fournisseurs des PME de bout en bout :
- **lecture** de la facture (PDF, e-mail ou facture électronique reçue via la plateforme agréée du client) ;
- **rapprochement** avec le bon de commande et le bon de livraison, avec détection des écarts ;
- **préparation** de l'écriture dans l'outil comptable ;
- **relance** du fournisseur quand une pièce manque ou qu'un montant ne colle pas.

Ordo se branche sur Pennylane, Sage et Qonto. L'humain garde la main : rien n'est payé ni comptabilisé sans validation, sauf si le client définit lui-même des règles (par exemple, un fournisseur récurrent sous un certain montant).

**Équipe** : 14 personnes à Paris et Lyon. **Clients** : 120 PME en production, de 20 à 250 salariés (chiffres fictifs).

## 2. Contexte et déclencheur

- **Levée** : seed de 6 M€ bouclée en octobre 2026 (fictif). Objectif : passer de 120 à 600 clients en 18 mois et recruter 15 personnes.
- **Réforme** : depuis le 1er septembre 2026, toutes les entreprises doivent pouvoir recevoir des factures électroniques. Nos prospects reçoivent donc des données structurées. C'est le bon moment pour leur proposer de les traiter automatiquement.
- **Site actuel** : une page Notion et un formulaire Typeform. Il ne tient pas face aux concurrents (Yooz, Libeo désormais chez Shine, Ramp à l'international) et ne sert ni le recrutement ni la relation avec les investisseurs.

## 3. Objectifs business et KPIs du site

| Objectif | KPI | Cible à 6 mois après la mise en ligne |
|---|---|---|
| Générer des démos qualifiées | Taux de demande de démo (visiteurs uniques vers formulaire envoyé) | ≥ 2,5 % (hypothèse à valider avec les données actuelles) |
| Qualifier | Part des demandes dans la cible (PME de 20 à 250 salariés, outil compatible) | ≥ 60 % |
| Prouver la valeur produit | Part des visiteurs qui voient la démo jusqu'au bout | ≥ 40 % |
| Recruter | Candidatures venant du site / mois | ≥ 30 |
| Être trouvé | Position Google sur « automatisation factures fournisseurs PME » et « rapprochement factures bons de commande » | Top 10 |
| Performance | LCP mobile | < 2,5 s |

Ces KPIs supposent un suivi d'événements en place dès la mise en ligne : clic CTA, envoi de formulaire, lecture de la démo à 25, 50 et 100 %, clic sur les tarifs.

## 4. Cibles et personas

### Persona 1 : Claire, DAF d'une PME industrielle (140 salariés)
- **Job to be done** : « Quand la clôture approche, je veux que les factures fournisseurs soient déjà rapprochées et justifiées, pour clôturer à J+5 sans heures supplémentaires pour mon équipe. »
- **Situation** : 900 factures fournisseurs par mois, 2 comptables fournisseurs, clôture mensuelle sous tension.
- **Attentes** : un taux d'automatisation réel, la compatibilité avec Sage, une piste d'audit, et un ROI qu'elle peut défendre devant son DG.
- **Freins** : « l'IA va se tromper et je ne le verrai pas », un projet d'intégration trop long, la peur de déstabiliser son équipe.
- **Ce qu'elle doit trouver** : une démo sur une vraie facture, le parcours d'une facture en cas d'écart, le délai de mise en route (en jours), des cas clients de taille comparable.

### Persona 2 : Karim, dirigeant d'une PME de services (35 salariés)
- **Job to be done** : « Quand les factures s'accumulent, je veux qu'elles soient vérifiées et prêtes à valider en un clic, pour ne plus y passer mes dimanches. »
- **Situation** : il fait lui-même la validation des factures le dimanche soir, sur Pennylane et Qonto.
- **Attentes** : du temps gagné, rien à installer, un prix lisible.
- **Freins** : le coût, la peur d'un outil de plus, et « est-ce que mes données servent à entraîner une IA ? ».
- **Ce qu'il doit trouver** : les tarifs sans prise de rendez-vous, la phrase « pas d'entraînement sur vos données », une démo courte sur mobile.

### Persona 3 : Sophie, expert-comptable associée (cabinet de 25 personnes)
- **Job to be done** : « Quand un client PME m'envoie ses pièces, je veux recevoir une saisie fournisseurs propre et rapprochée, pour consacrer mon temps au conseil plutôt qu'à la correction. »
- **Situation** : elle prescrit des outils à ses clients PME.
- **Attentes** : une saisie fournisseurs propre en amont, l'export vers ses outils, et une offre ou un contact partenaire.
- **Freins** : la responsabilité en cas d'erreur, et la peur d'être court-circuitée auprès de son client.
- **Ce qu'elle doit trouver** : une mention claire du rôle de l'expert-comptable, la compatibilité avec ses outils, un contact partenaire (lien dans la FAQ et le pied de page à ce stade).

## 5. Messages clés et preuves

| Message | Preuve attendue sur le site |
|---|---|
| « 4 h gagnées par semaine sur la compta fournisseurs » | Moyenne mesurée sur les clients actifs, avec périmètre et date (à fournir par Ordo) |
| « Chaque facture rapprochée avec sa commande » | Démo : facture, bon de commande, écart signalé |
| « Vous validez, Ordo exécute » | Écran de validation dans la démo, journal des actions |
| « Branché sur vos outils en une journée » | Logos de connecteurs réellement disponibles, délai moyen de mise en route |
| « Vos données restent en France et ne servent jamais à entraîner un modèle » | Nom de l'hébergeur et région, DPA téléchargeable, sous-traitants listés |
| « Un prix lisible » | 3 paliers publics |

Ton : précis, sobre, sans superlatif. Les mots « révolutionner », « magique » et « disruptif » sont interdits. Phrases courtes, verbes d'action, chiffres avec unité.

## 6. Arborescence et contenus attendus

**One-page** (ancres), plus quelques pages satellites.

1. **Hero** : titre avec le chiffre héros, sous-titre en une phrase, CTA « Réserver une démo » et lien secondaire « Voir les tarifs ». Logos clients ou mention « 120 PME » sous la ligne de flottaison.
2. **Démo produit** : boucle muette de 20 secondes environ, en HTML/CSS animé ou en vidéo, sur une facture anonymisée. Sur mobile : version verticale.
3. **Comment ça marche** : 3 étapes (connecter vos outils, Ordo traite, vous validez).
4. **Intégrations** : Pennylane, Sage, Qonto, plus les connecteurs en cours, marqués comme tels.
5. **Résultats clients** : 3 chiffres et 2 ou 3 témoignages (nom, fonction, entreprise, photo, avec accord écrit).
6. **Sécurité et données** : RGPD, hébergement en France, pas d'entraînement sur les données clients, chiffrement, droits d'accès, lien vers une page `/securite`.
7. **Tarifs** : 3 paliers (par exemple Essentiel, Équipe, Sur mesure) fondés sur un volume de factures par mois, HT, avec ce qui est inclus.
8. **On recrute** : 3 à 5 postes, lien vers la page carrières (Welcome to the Jungle ou équivalent).
9. **FAQ et formulaire de démo** : 8 questions maximum, formulaire à 4 champs (e-mail pro, entreprise, outil comptable, volume mensuel de factures).

**Pages satellites** : `/securite`, `/mentions-legales`, `/confidentialite`, `/cookies`, `/carrieres` (ou lien externe), `/accessibilite`.

**Contenus fournis par Ordo** : chiffres clients validés, témoignages signés, liste des connecteurs, grille tarifaire, DPA, captures produit en haute définition, offres d'emploi, logo vectoriel.
**Contenus produits par l'agence** : rédaction web, scénario et réalisation de la démo animée, iconographie.

## 7. Contraintes

- **Marque** : nom et logo provisoires (vérification INPI en cours). Palette : fond presque blanc, encre bleu nuit, un seul accent vert électrique réservé aux états « traité ». Typo : Inter Tight ou Geist, avec une mono pour les chiffres. Une seule animation forte.
- **Réglementaire** :
  - RGPD : bandeau cookies conforme aux recommandations de la CNIL (refuser aussi simple qu'accepter), formulaire avec information sur le traitement.
  - AI Act : informer clairement que des traitements sont faits par IA. La qualification exacte du système relève du juridique d'Ordo. Le site ne doit rien promettre qui excède cette qualification.
  - Allégations : tout chiffre affiché doit être sourcé en interne (date, périmètre) et pouvoir être justifié.
- **Accessibilité** : viser WCAG 2.1 AA (référentiel RGAA 4.1). Contrastes vérifiés, en particulier le vert sur fond clair, à réserver aux pastilles et aux fonds, jamais au texte courant. Démo avec contrôle pause, respect de `prefers-reduced-motion`, navigation clavier complète, formulaire étiqueté.
- **SEO** : contenu servi en HTML (pas de texte seulement dans la vidéo), balises title et meta par section ou page, données structurées Organization, SoftwareApplication et FAQPage. Mots-clés : automatisation factures fournisseurs, rapprochement factures commandes, IA comptabilité PME, facture électronique réception.
- **Langues** : français au lancement. Anglais prévu à 6 mois pour les investisseurs et le recrutement : prévoir la structure i18n dès le départ.
- **Technique** : Webflow, Framer ou statique (Astro), au choix de l'agence et argumenté. Ordo doit pouvoir modifier les textes, les postes et la FAQ sans développeur.
- **Performance** : poids de la démo < 1,5 Mo sur mobile, Lighthouse ≥ 90 sur les quatre axes.

## 8. Livrables

1. Atelier de cadrage (une demi-journée) et plateforme de messages.
2. Wireframes desktop et mobile.
3. Maquettes haute fidélité (Figma) : one-page, `/securite`, états du formulaire.
4. Scénario et réalisation de la démo animée.
5. Rédaction web en français.
6. Intégration, CMS, formulaire branché sur le CRM (HubSpot).
7. Plan de taggage et tableau de bord (Plausible ou GA4 avec consentement).
8. Recette : accessibilité, performance, navigateurs.
9. Passation : documentation et formation de 1 h.

## 9. Planning indicatif

| Semaine | Étape |
|---|---|
| S1 | Cadrage, collecte des contenus, plateforme de messages |
| S2 | Wireframes, scénario de la démo |
| S3 à S4 | Maquettes haute fidélité, 2 allers-retours |
| S4 à S5 | Rédaction finale, production de la démo |
| S5 à S7 | Intégration, CMS, formulaire, taggage |
| S8 | Recette, corrections, mise en ligne |

**Total : 8 semaines.** Le chemin critique, ce sont les contenus côté Ordo : chiffres clients et témoignages à fournir avant la fin de S3.

## 10. Budget

Fourchettes indicatives du marché français, à confirmer par devis :

| Prestataire | Périmètre | Fourchette HT |
|---|---|---|
| Freelance (designer et dev no-code) | One-page, démo en motion simple, rédaction fournie par Ordo | 5 000 à 10 000 € |
| Petit studio (2 à 5 personnes) | Périmètre complet ci-dessus | 12 000 à 25 000 € |
| Agence établie | Périmètre complet, démo en motion avancée, version EN | 25 000 à 45 000 € |

Hors budget : abonnement CMS et hébergement (environ 30 à 80 €/mois), shooting photo de l'équipe, traduction anglaise si elle est faite plus tard.
**Enveloppe Ordo : 18 000 à 24 000 € HT.**

## 11. Critères de réussite

- Un visiteur comprend ce que fait Ordo en moins de 5 secondes. Test : 5 personnes de la cible reformulent la promesse sans aide.
- La démo montre une facture traitée de bout en bout en moins de 25 secondes.
- Les KPIs de la section 3 sont mesurables dès le premier jour.
- Score RGAA ou WCAG AA sans non-conformité bloquante, Lighthouse ≥ 90.
- L'équipe Ordo met à jour un poste ou une question de FAQ seule, en moins de 10 minutes.
- Aucun chiffre ni logo affiché sans justification documentée.

## 12. UX copy

### Titre du hero recommandé
> **4 h gagnées chaque semaine sur vos factures fournisseurs.**
> Sous-titre : Ordo lit chaque facture, la rapproche de la commande et prépare l'écriture dans Pennylane, Sage ou Qonto. Vous validez.
> Ligne de périmètre, sous le chiffre : *Moyenne mesurée sur nos clients PME actifs, [mois année].*

### Alternatives

| Option | Texte | Ton | Idéal pour |
|---|---|---|---|
| A, bénéfice temps | « 4 h gagnées chaque semaine sur vos factures fournisseurs. » | Direct, chiffré | Dirigeants de PME (Karim) |
| B, contrôle | « Chaque facture rapprochée avec sa commande. Avant que vous la validiez. » | Rassurant, précis | DAF (Claire), qui craint les erreurs |
| C, réforme | « Vous recevez des factures électroniques. Ordo les traite pour vous. » | Factuel, d'actualité | Campagnes et SEO liés à la réforme |

### Libellés des CTA

| Emplacement | Libellé | Remarque |
|---|---|---|
| Hero, principal | **Réserver une démo de 20 min** | Durée explicite, ce qui réduit l'engagement perçu |
| Hero, secondaire | **Voir les tarifs** | Ancre vers la section Tarifs |
| Démo | **Voir une facture traitée** | Relance la boucle ou ouvre la démo en plein écran |
| Intégrations | **Vérifier la compatibilité de mon outil** | Ancre vers le formulaire, avec le champ outil prérempli |
| Tarifs (par palier) | **Démarrer avec Essentiel** / **Démarrer avec Équipe** / **Parler à un expert** | Verbe d'action et nom du palier |
| Jobs | **Voir les postes ouverts** | |
| Mobile, barre fixe | **Réserver une démo** | Court, en une ligne |

À éviter : « En savoir plus », « Commencer », « Envoyer ».

### Messages du formulaire de démo
- **Succès** : « C'est noté, [Prénom]. Vous recevez dans 2 minutes un e-mail pour choisir votre créneau. Préparez une ou deux factures fournisseurs récentes : nous les traiterons ensemble pendant la démo. »
- **Erreur, e-mail invalide** : « Cette adresse e-mail semble incomplète. Il manque le "@" ou le domaine. Vérifiez-la, par exemple : prenom@entreprise.fr. »
- **Erreur, e-mail personnel** (si filtré) : « Nous n'avons pas pu enregistrer une adresse Gmail ou Outlook. Les démos sont réservées aux entreprises. Utilisez votre adresse professionnelle, ou écrivez-nous à [contact] si vous n'en avez pas. »
- **Erreur d'envoi (serveur)** : « Votre demande n'est pas partie. La connexion a été interrompue. Vos informations sont conservées : cliquez à nouveau sur "Réserver une démo de 20 min". »

## 13. Mini plan de recherche utilisateur

- **Objectif** : vérifier que la promesse, la démo et la section sécurité lèvent les freins des DAF et des dirigeants de PME, et que le parcours mène à la demande de démo.
- **Méthode** : 5 tests d'usabilité modérés à distance (45 min) sur la maquette haute fidélité, en fin de semaine S3. Profils : 2 DAF, 2 dirigeants de PME, 1 expert-comptable. Recrutement parmi les prospects et le réseau de clients d'Ordo.
- **Mesures** : compréhension de la promesse en 5 secondes, réussite de la tâche « demander une démo », objections spontanées, note de confiance de 1 à 5.

### Guide d'entretien

1. **Mise en route** (5 min)
   - « Présentez-vous en deux mots : votre rôle, la taille de l'entreprise. »
   - « Il n'y a pas de bonne ou de mauvaise réponse : c'est le site qu'on teste, pas vous. »
2. **Contexte** (10 min)
   - « Racontez-moi la dernière fois que vous avez traité une pile de factures fournisseurs. Combien de temps, avec quels outils ? »
   - « Qu'est-ce qui vous fait le plus perdre de temps ou vous inquiète dans ce processus ? »
   - « Avez-vous déjà testé un outil d'automatisation ? Qu'est-ce qui s'est passé ? »
3. **Approfondissement** (10 min)
   - « Qu'attendriez-vous d'un outil qui traite les factures à votre place ? Qu'est-ce qui vous ferait refuser ? »
   - « Qui d'autre doit dire oui dans votre entreprise ? »
   - « Que doit-il se passer avec vos données pour que vous soyez tranquille ? »
4. **Réaction à la maquette** (15 min)
   - Test de 5 secondes sur le hero : « Que fait cette entreprise, pour qui ? »
   - Après la démo : « Qu'avez-vous vu se passer ? Qu'est-ce qui vous rassure ou vous gêne ? »
   - Tâche : « Vous voulez savoir si Ordo marche avec votre outil, puis demander une démo. Allez-y. »
5. **Conclusion** (5 min)
   - « Sur 5, quelle confiance accordez-vous à ce site ? Pourquoi pas plus ? »
   - « Si vous ne deviez changer qu'une chose, ce serait quoi ? »
