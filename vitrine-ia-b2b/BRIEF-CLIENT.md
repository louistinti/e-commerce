# Brief client : site vitrine Ordo

> **Document de démonstration.** Ordo est une entreprise FICTIVE, créée pour illustrer la catégorie `vitrine-ia-b2b`. Le brief garde la forme d'une demande d'Ordo à l'agence, mais il n'y a pas de client derrière : toutes les décisions sont prises ici. Aucun chiffre n'est inventé : toute donnée chiffrée réelle porte sa source, vue le 2026-11-13. Les personnes citées sont fictives. Le nom Ordo n'est pas déposé et ne sert qu'à cette démonstration.

**Émetteur** : Ordo SAS (fictif), direction marketing
**Destinataire** : l'agence
**Date** : novembre 2026
**Version** : 1.1

---

## 1. Qui nous sommes

Ordo déploie des agents IA qui traitent les factures fournisseurs des PME de bout en bout :
- **lecture** de la facture (PDF, e-mail ou facture électronique reçue via la plateforme agréée du client) ;
- **rapprochement** avec le bon de commande et le bon de livraison, avec détection des écarts ;
- **préparation** de l'écriture dans l'outil comptable ;
- **relance** du fournisseur quand une pièce manque ou qu'un montant ne colle pas.

Ordo se branche sur Pennylane, Sage et Qonto. L'humain garde la main : rien n'est payé ni comptabilisé sans validation, sauf si le client définit lui-même des règles (par exemple, un fournisseur récurrent sous un certain montant).

**Équipe** : à Paris et à Lyon. **Cible** : PME de 20 à 250 salariés. Le plafond suit la définition de la PME par l'Insee, « moins de 250 personnes » ([Insee](https://www.insee.fr/fr/metadonnees/definition/c1962), vu le 2026-11-13). Le plancher de 20 salariés est un choix de positionnement d'Ordo.

## 2. Contexte et déclencheur

- **Levée** : Ordo vient de boucler sa seed (montant non communiqué). Elle finance le recrutement et l'acquisition de clients.
- **Réforme** : depuis le 1er septembre 2026, toutes les entreprises assujetties à la TVA établies en France doivent pouvoir recevoir des factures électroniques ([Moneyvox](https://www.moneyvox.fr/votre-argent/actualites/110141/facturation-electronique-ce-qui-change-vraiment-a-partir-du-1er-septembre-2026), vu le 2026-11-13). Nos prospects reçoivent donc des données structurées. C'est le bon moment pour leur proposer de les traiter automatiquement.
- **Site actuel** : une page Notion et un formulaire Typeform. Il ne tient pas face aux concurrents (Yooz, Libeo désormais chez Shine, Ramp à l'international) et ne sert ni le recrutement ni la relation avec les investisseurs.

## 3. Objectifs business et indicateurs du site

| Objectif | Indicateur suivi |
|---|---|
| Générer des démos qualifiées | Taux de demande de démo (visiteurs uniques vers formulaire envoyé) |
| Qualifier | Part des demandes dans la cible (PME de 20 à 250 salariés, outil compatible) |
| Prouver la valeur produit | Part des visiteurs qui voient la démo jusqu'au bout |
| Recruter | Candidatures venant du site, par mois |
| Être trouvé | Position Google sur « automatisation factures fournisseurs PME » et « rapprochement factures bons de commande » |
| Performance | LCP mobile sous 2,5 s, seuil « bon » des Core Web Vitals de Google |

Pas de cible chiffrée : Ordo est fictive et n'a aucun historique de trafic. On suit l'évolution de chaque indicateur après la mise en ligne. Seul le LCP a un seuil, parce que c'est une norme publique.

Ces indicateurs supposent un suivi d'événements en place dès la mise en ligne : clic CTA, envoi de formulaire, lecture de la démo à 25, 50 et 100 %, clic sur les tarifs.

## 4. Cibles et personas

### Persona 1 : Claire, DAF d'une PME industrielle
- **Job to be done** : « Quand la clôture approche, je veux que les factures fournisseurs soient déjà rapprochées et justifiées, pour clôturer dans les délais sans heures supplémentaires pour mon équipe. »
- **Situation** : un gros volume de factures fournisseurs chaque mois, une petite équipe de comptables fournisseurs, une clôture mensuelle sous tension.
- **Attentes** : voir ce qui est automatisé et ce qui ne l'est pas, la compatibilité avec Sage, une piste d'audit, et des arguments qu'elle peut défendre devant son DG.
- **Freins** : « l'IA va se tromper et je ne le verrai pas », un projet d'intégration trop long, la peur de déstabiliser son équipe.
- **Ce qu'elle doit trouver** : une démo sur une vraie facture, le parcours d'une facture en cas d'écart, les étapes de mise en route, des cas d'usage proches du sien.

### Persona 2 : Karim, dirigeant d'une PME de services
- **Job to be done** : « Quand les factures s'accumulent, je veux qu'elles soient vérifiées et prêtes pour ma validation en un clic, pour ne plus y passer mes dimanches. »
- **Situation** : il fait lui-même la validation des factures le dimanche soir, sur Pennylane et Qonto.
- **Attentes** : du temps gagné, rien à installer, un prix lisible.
- **Freins** : le coût, la peur d'un outil de plus, et « est-ce que mes données servent à entraîner une IA ? ».
- **Ce qu'il doit trouver** : un prix sans prise de rendez-vous, la phrase « pas d'entraînement sur vos données », une démo courte sur mobile.

### Persona 3 : Sophie, expert-comptable associée dans un cabinet
- **Job to be done** : « Quand un client PME m'envoie ses pièces, je veux recevoir une saisie fournisseurs propre et rapprochée, pour consacrer mon temps au conseil plutôt qu'à la correction. »
- **Situation** : elle prescrit des outils à ses clients PME.
- **Attentes** : une saisie fournisseurs propre en amont, l'export vers ses outils, et une offre ou un contact partenaire.
- **Freins** : la responsabilité en cas d'erreur, et la peur d'être court-circuitée auprès de son client.
- **Ce qu'elle doit trouver** : une mention claire du rôle de l'expert-comptable, la compatibilité avec ses outils, un contact partenaire (lien dans la FAQ et le pied de page à ce stade).

## 5. Messages clés et preuves

| Message | Preuve sur le site |
|---|---|
| « Chaque facture rapprochée avec sa commande » | Démo : facture, bon de commande, écart signalé |
| « Vous validez, Ordo exécute » | Écran de validation dans la démo, journal des actions |
| « Vos factures fournisseurs prêtes pour votre validation » | Démo : la facture arrive, Ordo la traite, elle attend votre accord |
| « Branché sur Pennylane, Sage et Qonto » | Logos des connecteurs disponibles, connecteurs en cours marqués comme tels, étapes de mise en route |
| « Vos données restent en France et ne servent jamais à entraîner un modèle » | Hébergeur et région nommés, DPA téléchargeable, sous-traitants listés |
| « Un prix lisible » | 3 paliers publics, prix d'entrée affiché |

Le message chiffré de la version précédente (un gain de temps hebdomadaire) est retiré : le chiffre était inventé, et Ordo n'a rien mesuré.

Ton : précis, sobre, sans superlatif. Les mots « révolutionner », « magique » et « disruptif » sont interdits. Phrases courtes, verbes d'action. Aucun chiffre sans source.

## 6. Arborescence et contenus attendus

**One-page** (ancres), plus quelques pages satellites.

1. **Hero** : titre sans chiffre (voir UX copy), sous-titre en une phrase, CTA « Réserver une démo » et lien secondaire « Voir les tarifs ». Sous la ligne de flottaison : les logos des outils connectés (Pennylane, Sage, Qonto), pas de logos clients.
2. **Démo produit** : boucle muette de 20 secondes environ, en HTML/CSS animé ou en vidéo, sur une facture anonymisée. Sur mobile : version verticale.
3. **Comment ça marche** : 3 étapes (connecter vos outils, Ordo traite, vous validez).
4. **Intégrations** : Pennylane, Sage et Qonto, plus deux connecteurs en cours (Cegid et Odoo), marqués « bientôt ».
5. **Preuves et témoignages** : 3 engagements que la démo montre (chaque facture rapprochée, chaque écart signalé avant validation, chaque action journalisée), sans chiffre. Puis 2 ou 3 témoignages de clients fictifs (nom, fonction, entreprise), sans chiffre ni photo : un monogramme d'initiales à la place du portrait.
6. **Sécurité et données** : RGPD, hébergement en France, pas d'entraînement sur les données clients, chiffrement, droits d'accès, lien vers une page `/securite`.
7. **Tarifs** : 3 paliers (Essentiel, Équipe, Sur mesure) fondés sur un volume de factures par mois, avec ce qui est inclus. Essentiel affiche « à partir de 99 € HT par mois » : prix de démo calé sur le prix d'entrée public de Yooz, « À partir de 99 € » pour un abonnement mensuel ([Yooz, tarifs](https://www.getyooz.com/fr/tarifs), vu le 2026-11-13). Équipe et Sur mesure affichent « Prix selon votre volume ».
8. **Qui sommes-nous et on recrute** : un bloc « Qui sommes-nous » court, sans photo, avec le logo (texte ci-dessous), puis 3 à 5 postes et un lien vers la page carrières (Welcome to the Jungle ou équivalent).
9. **FAQ et formulaire de démo** : 8 questions maximum, formulaire à 4 champs (e-mail pro, entreprise, outil comptable, volume mensuel de factures).

Texte du bloc « Qui sommes-nous » :
> Ordo réunit des profils produit, ingénierie et comptabilité, à Paris et à Lyon. Nous construisons des agents qui traitent les factures fournisseurs des PME, avec une règle simple : rien n'est payé ni comptabilisé sans votre validation.

Les photos d'équipe ont été cherchées en banque d'images le 2026-11-13 (Unsplash, puis Pexels). Les deux sites ont bloqué le navigateur automatisé : le bloc reste sans photo.

**Pages satellites** : `/securite`, `/mentions-legales`, `/confidentialite`, `/cookies`, `/carrieres` (ou lien externe), `/accessibilite`.

**Contenus à produire par l'agence** : rédaction web, scénario et réalisation de la démo animée, facture d'exemple anonymisée, iconographie, logo vectoriel, témoignages fictifs, offres d'emploi fictives, contenu des paliers, page `/securite` avec un hébergeur nommé, un DPA type et la liste des sous-traitants. Aucun chiffre client : Ordo n'en a pas.

Le pied de page porte la mention « Ordo est une entreprise fictive. Site de démonstration. »

## 7. Contraintes

- **Marque** : nom et logo de démonstration, non déposés. Palette : fond presque blanc, encre bleu nuit, un seul accent vert électrique réservé aux états « traité ». Typo : Inter Tight ou Geist, avec une mono pour les chiffres. Une seule animation forte.
- **Réglementaire** :
  - RGPD : bandeau cookies conforme aux recommandations de la CNIL (refuser aussi simple qu'accepter), formulaire avec information sur le traitement.
  - AI Act : le site dit clairement que la lecture, le rapprochement et la relance sont faits par IA, avec validation humaine (mention près de la démo et dans la FAQ). Il ne revendique aucune certification ni conformité qu'Ordo n'a pas.
  - Allégations : aucun chiffre de résultat sur le site, puisqu'Ordo n'a rien mesuré. Un chiffre n'apparaît que s'il vient d'une source publique nommée (par exemple la date de la réforme), avec le lien.
- **Accessibilité** : viser WCAG 2.1 AA (référentiel RGAA 4.1). Contrastes vérifiés, en particulier le vert sur fond clair, à réserver aux pastilles et aux fonds, jamais au texte courant. Démo avec contrôle pause, respect de `prefers-reduced-motion`, navigation clavier complète, formulaire étiqueté.
- **SEO** : contenu servi en HTML (pas de texte seulement dans la vidéo), balises title et meta par section ou page, données structurées Organization, SoftwareApplication et FAQPage. Mots-clés : automatisation factures fournisseurs, rapprochement factures commandes, IA comptabilité PME, facture électronique réception.
- **Langues** : français au lancement. Anglais dans un second temps, pour les investisseurs et le recrutement : la structure i18n est prévue dès le départ.
- **Technique** : site statique (Astro), parce qu'il sert le contenu en HTML pour le SEO et tient la cible Lighthouse sans extension. Textes, postes et FAQ sont dans des fichiers de contenu séparés, modifiables sans toucher au code.
- **Performance** : poids de la démo < 1,5 Mo sur mobile, Lighthouse ≥ 90 sur les quatre axes.

## 8. Livrables

1. Atelier de cadrage (une demi-journée) et plateforme de messages.
2. Wireframes desktop et mobile.
3. Maquettes haute fidélité (Figma) : one-page, `/securite`, états du formulaire.
4. Scénario et réalisation de la démo animée.
5. Rédaction web en français.
6. Intégration, contenus éditables, formulaire branché sur le CRM (HubSpot).
7. Plan de taggage et tableau de bord dans Plausible, retenu parce qu'il mesure l'audience sans cookie.
8. Recette : accessibilité, performance, navigateurs.
9. Passation : documentation et formation de 1 h.

## 9. Planning indicatif

| Semaine | Étape |
|---|---|
| S1 | Cadrage, plateforme de messages, liste des contenus à produire |
| S2 | Wireframes, scénario de la démo |
| S3 à S4 | Maquettes haute fidélité, 2 allers-retours |
| S4 à S5 | Rédaction finale, production de la démo |
| S5 à S7 | Intégration, contenus éditables, formulaire, taggage |
| S8 | Recette, corrections, mise en ligne |

**Total : 8 semaines.** Le chemin critique est la démo animée : scénario en S2, production en S4 et S5. La section Démo et l'indicateur de lecture en dépendent.

## 10. Budget

Aucun montant. Ordo est fictive, et aucune grille tarifaire publique d'agence ou de freelance n'a été ouverte pour ce périmètre : les fourchettes et l'enveloppe de la version précédente sont retirées. Hors périmètre : abonnement d'hébergement, traduction anglaise.

## 11. Critères de réussite

- Un visiteur comprend ce que fait Ordo en moins de 5 secondes. Test : 5 personnes de la cible reformulent la promesse sans aide.
- La démo montre une facture traitée de bout en bout en moins de 25 secondes.
- Les indicateurs de la section 3 sont mesurables dès le premier jour.
- Score RGAA ou WCAG AA sans non-conformité bloquante, Lighthouse ≥ 90.
- Un poste ou une question de FAQ se met à jour en moins de 10 minutes, sans développeur.
- Aucun chiffre ni logo affiché sans source publique nommée.

## 12. UX copy

### Titre du hero recommandé
> **Chaque facture rapprochée avec sa commande. Avant que vous la validiez.**
> Sous-titre : Ordo lit chaque facture, la rapproche de la commande et prépare l'écriture dans Pennylane, Sage ou Qonto. Vous validez.

Le titre chiffré de la version précédente est retiré : le chiffre était inventé.

### Alternatives

| Option | Texte | Ton | Idéal pour |
|---|---|---|---|
| A, bénéfice temps | « Vos factures fournisseurs, prêtes pour votre validation en un clic. » | Direct | Dirigeants de PME (Karim) |
| B, contrôle (recommandée) | « Chaque facture rapprochée avec sa commande. Avant que vous la validiez. » | Rassurant, précis | DAF (Claire), qui craint les erreurs |
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
- **Succès** : « C'est noté, [Prénom]. Vous allez recevoir un e-mail pour choisir votre créneau. Préparez une ou deux factures fournisseurs récentes : nous les traiterons ensemble pendant la démo. »
- **Erreur, e-mail invalide** : « Cette adresse e-mail semble incomplète. Il manque le "@" ou le domaine. Vérifiez-la, par exemple : prenom@entreprise.fr. »
- **Erreur, e-mail personnel** (si filtré) : « Nous n'avons pas pu enregistrer une adresse Gmail ou Outlook. Les démos sont réservées aux entreprises. Utilisez votre adresse professionnelle, ou écrivez-nous à [contact] si vous n'en avez pas. »
- **Erreur d'envoi (serveur)** : « Votre demande n'est pas partie. La connexion a été interrompue. Vos informations sont conservées : cliquez à nouveau sur "Réserver une démo de 20 min". »

## 13. Mini plan de recherche utilisateur

- **Objectif** : vérifier que la promesse, la démo et la section sécurité lèvent les freins des DAF et des dirigeants de PME, et que le parcours mène à la demande de démo.
- **Méthode** : 5 tests d'usabilité modérés à distance (45 min) sur la maquette haute fidélité, en fin de semaine S3. Profils : 2 DAF, 2 dirigeants de PME, 1 expert-comptable, recrutés par un panel de testeurs.
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
