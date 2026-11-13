# Brief client : site vitrine Liasse

> **Document de démonstration.** Liasse est une entreprise FICTIVE créée pour illustrer la catégorie `vitrine-fintech-saas`. Le brief garde la forme d'une commande de Liasse à l'agence, mais personne ne le validera : l'agence décide de tout. Aucun chiffre n'est inventé. Liasse n'a ni taille d'équipe, ni nombre d'utilisateurs, ni levée, ni avis chiffrés, et ses prix de démonstration sont calés sur une grille publique sourcée (section 6). Chaque donnée chiffrée sur le marché ou la loi porte sa source, vue le 2026-11-13. Le nom est fictif et n'a fait l'objet d'aucun dépôt.

**Émetteur** : Liasse SAS (fictif), cofondatrice en charge du produit et du marketing
**Destinataire** : l'agence
**Date** : novembre 2026
**Version** : 1.0

---

## 1. Qui nous sommes

Liasse est l'application de facturation électronique et de trésorerie pensée pour les artisans et les TPE :
- **Facturer** : devis, acompte et facture conformes, créés depuis le téléphone, émis et reçus au format électronique.
- **Relancer** : relances automatiques et polies, avec un lien de paiement.
- **Voir venir** : la trésorerie projetée à 90 jours, à partir des factures émises, des factures reçues et du compte bancaire.
- **Transmettre** : export comptable et accès direct pour l'expert-comptable.

**Cadre de fiction** : dans l'histoire, Liasse est plateforme agréée. Comme elle n'existe pas, elle n'a pas de numéro d'immatriculation et n'apparaît pas sur la [liste officielle des plateformes agréées](https://www.impots.gouv.fr/je-consulte-la-liste-des-plateformes-agreees) (impots.gouv.fr, vu le 2026-11-13). Le site de démonstration n'affiche donc ni numéro ni logo officiel (voir section 7).

**Équipe** : une petite équipe basée à Nantes. **Utilisateurs** : des TPE, surtout des artisans du bâtiment. Aucun effectif ni volume n'est donné : ils seraient inventés.

**Qui sommes-nous, sur le site** : pas de bloc équipe ni de photo. Le pied de page dit en une phrase qui fait Liasse et d'où.

## 2. Contexte et déclencheur

- **Objectif** : gagner des utilisateurs avant l'échéance d'émission du 1er septembre 2027. Pas de levée ni d'objectif chiffré : ils seraient inventés.
- **Réforme** : toutes les entreprises assujetties à la TVA doivent pouvoir recevoir des factures électroniques depuis le 1er septembre 2026. Les PME, TPE et micro-entreprises doivent les émettre à partir du 1er septembre 2027 ([Moneyvox](https://www.moneyvox.fr/actu/110141/facturation-electronique-ce-qui-change-vraiment-a-partir-du-1er-septembre-2026), article du 28 août 2026, vu le 2026-11-13). Les mois qui séparent novembre 2026 de septembre 2027 sont la fenêtre d'acquisition.
- **Concurrence** : de nombreuses plateformes agréées ([liste officielle](https://www.impots.gouv.fr/je-consulte-la-liste-des-plateformes-agreees), impots.gouv.fr, vu le 2026-11-13), et une conformité gratuite chez plusieurs acteurs (voir l'étude de cas, section 1). Liasse doit gagner sur la **trésorerie**, les **relances** et le **ton artisan**.
- **Site actuel** : landing page de lancement. Le titre « Vos factures conformes 2026 » est dépassé, et le site ne parle ni de trésorerie ni aux experts-comptables.

**Affinement par rapport au README** : le hero passe de « Vos factures conformes 2026, en 2 minutes » à une formulation qui reste vraie après septembre 2026 et ne promet aucune durée chiffrée (voir UX copy). « Agrément PDP » devient « plateforme agréée (PA) », l'appellation officielle actuelle.

## 3. Objectifs business et indicateurs du site

Indicateurs à suivre dès la mise en ligne, sans cible chiffrée : une cible serait inventée, faute de site existant et de données réelles.

| Objectif | Indicateur suivi |
|---|---|
| Acquérir des essais | Taux d'inscription (visiteurs uniques vers e-mail envoyé) |
| Activer | Part des inscrits qui créent une première facture dans la semaine (mesuré côté produit) |
| Mobile | Part des inscriptions faites sur mobile |
| Prescription | Demandes de partenariat d'experts-comptables par mois |
| Réassurance | Clics vers l'échéancier de la réforme et la FAQ |
| SEO | Position sur « facture électronique artisan », « logiciel facturation artisan », « facturation électronique 2027 TPE » |
| Performance | LCP mobile, sous le seuil « bon » de 2,5 s des Core Web Vitals de Google (seuil public, pas une cible inventée) |

## 4. Cibles et personas

### Persona 1 : Mehdi, plombier-chauffagiste, à la tête d'une petite équipe
- **Job to be done** : « Quand je finis un chantier, je veux envoyer la facture depuis la camionnette et être payé sans courir après le client, pour ne pas faire la paperasse le soir. »
- **Situation** : devis et factures sur un tableur ou du papier carbone, beaucoup d'acomptes, des clients particuliers et des pros.
- **Attentes** : simple sur téléphone, devis transformé en facture en un geste, relances automatiques.
- **Freins** : « encore un abonnement », la peur de mal faire avec la réforme, aucune envie de lire du jargon.
- **Ce qu'il doit trouver** : des captures mobiles, la preuve que c'est rapide (la démo, pas une durée promise), un prix clair, et une réponse à « qu'est-ce que je dois faire et quand ? ».

### Persona 2 : Nathalie, gérante d'un salon de coiffure et d'une boutique, quelques salariés
- **Job to be done** : « Quand je regarde mon compte, je veux savoir si je pourrai payer mes fournisseurs et mes salaires dans 2 mois, pour décider sereinement d'un achat ou d'une embauche. »
- **Situation** : reçoit beaucoup de factures fournisseurs, en émet peu, et pilote sa trésorerie « au feeling ».
- **Attentes** : une vision de la trésorerie à 90 jours, la réception des e-factures centralisée.
- **Freins** : la sécurité des données bancaires, la peur de devoir tout ressaisir.
- **Ce qu'elle doit trouver** : l'aperçu de la courbe de trésorerie, la connexion bancaire expliquée, la sécurité (hébergement, chiffrement).

### Persona 3 : Julien, expert-comptable, cabinet qui suit de nombreuses TPE
- **Job to be done** : « Quand la réforme impose l'e-facture à mes clients, je veux leur recommander un outil fiable qui m'envoie des données propres, pour ne pas gérer toutes ces migrations à la main. »
- **Attentes** : export vers son logiciel de production, accès multi-clients, accompagnement.
- **Freins** : un outil de plus à maîtriser, la perte de la relation avec ses clients.
- **Ce qu'il doit trouver** : une section dédiée avec bénéfices, formats d'export, invitation des clients et contact partenaire.

## 5. Messages clés et preuves

| Message | Preuve attendue sur le site |
|---|---|
| « Une facture conforme depuis votre téléphone, sans repasser au bureau » | Boucle mobile du parcours devis, puis facture, puis envoi. Pas de chronomètre ni de durée promise |
| « Prêt pour l'émission de septembre 2027, dès aujourd'hui » | Échéancier par profil, daté et sourcé. Pas de numéro d'immatriculation (voir section 7) |
| « Les relances partent toutes seules » | La séquence de relances montrée telle qu'elle part : dates, texte, lien de paiement. Aucun délai moyen de paiement : Liasse n'en a pas |
| « Votre trésorerie à 90 jours, en un coup d'œil » | Aperçu de la courbe avec des montants animés |
| « Votre expert-comptable branché directement » | Formats d'export écrits en clair (FEC, CSV). Pas de logos de logiciels tiers : une compatibilité affichée serait fausse |
| « Vos données sont protégées » | Région d'hébergement, chiffrement et statut réglementaire du prestataire de connexion bancaire écrits en clair, sans nommer de prestataire réel (voir section 7) |

Ton : simple, chaleureux, rassurant. Tutoiement exclu, vouvoiement direct. Pas de peur ni d'amendes en rouge. Les mots « disruptif » et « révolution » sont interdits.

## 6. Arborescence et contenus attendus

One-page avec ancres.
1. **Hero** : titre, sous-titre, **champ e-mail** et bouton « Essai gratuit 30 jours » (durée calée sur l'essai public de Qonto, « Essayez Qonto gratuitement pendant 30 jours », [qonto.com/fr/pricing](https://qonto.com/fr/pricing), vu le 2026-11-13). Capture mobile en premier sur téléphone.
2. **Échéancier de la réforme** : frise 2026–2027 et sélecteur « Je suis : artisan, commerçant, profession libérale, société ». Affiche « Ce que vous devez faire » pour le profil choisi.
3. **Fonctionnalités** : facture, relance, trésorerie, export comptable (4 cartes).
4. **Aperçu de l'application** : captures mobile et desktop, micro-animations sur les montants.
5. **Pour les experts-comptables** : bénéfices, export, invitation des clients, contact partenaire.
6. **Sécurité** : plateforme agréée (sans numéro, voir section 7), hébergement, chiffrement, données bancaires.
7. **Tarifs** : 2 formules, Solo et Équipe, en HT et TTC, et un comparatif « Liasse et les autres » qui compare des catégories (logiciel gratuit, tableur, papier), jamais des marques. Prix de démonstration calés sur les deux premières formules publiques de Pennylane (Starter 7 € HT par mois, Basique 14 € HT par mois, [page facturation électronique](https://www.pennylane.com/fr/logiciel-facturation-electronique?so=1), vu le 2026-11-13), marqués « prix de démonstration » sur le site.
8. **FAQ et inscription** : FAQ de 8 à 10 questions, répétition du champ e-mail. Pas de bloc d'avis : une entreprise fictive n'a ni note ni verbatims, et en inventer reviendrait à publier de faux avis.

Pages satellites : `/mentions-legales`, `/confidentialite`, `/cookies`, `/cgu`, `/accessibilite`, `/experts-comptables` (version longue, phase 2).

## 7. Contraintes

- **Marque** : palette crème, violet profond, accent corail. Typo grotesque arrondie (DM Sans ou Outfit), chiffres tabulaires. Mockups soignés, micro-animations sur les montants.
- **Réglementaire** :
  - Plateforme agréée : la mention n'a de valeur qu'avec une immatriculation réelle, vérifiable sur la [liste officielle](https://www.impots.gouv.fr/je-consulte-la-liste-des-plateformes-agreees). Liasse n'en a pas. Le site de démonstration écrit « plateforme agréée » dans le texte, sans numéro, sans le logo officiel de la République française, avec la mention « entreprise fictive » en pied de page.
  - Avis en ligne : le Code de la consommation impose d'informer sur l'existence et le mode de contrôle des avis. Le site n'en publie pas (voir section 6).
  - Prix : HT et TTC lisibles. Conditions de l'essai écrites à côté du bouton : sans carte bancaire, sans engagement, pas de reconduction payante automatique.
  - Données bancaires : la connexion bancaire passe par un prestataire de services d'information sur les comptes, statut réglementaire écrit en clair. Aucun prestataire réel n'est nommé : Liasse est fictive et n'a pas de contrat. Ne pas laisser entendre que Liasse est une banque.
  - RGPD et cookies : consentement conforme aux recommandations de la CNIL.
- **Accessibilité** : WCAG 2.1 AA (RGAA 4.1). Le corail ne sert jamais au texte sur fond crème (2,54:1, sous le seuil de 4,5:1 de WCAG 2.1, calculé dans le bench), les animations de montants respectent `prefers-reduced-motion`, les cibles tactiles font au moins 44 px (WCAG 2.1, critère 2.5.5), la frise est lisible sans couleur.
- **SEO** : HTML indexable, FAQPage et SoftwareApplication en données structurées, contenu réforme daté et mis à jour.
- **Langues** : français uniquement.
- **Technique** : CMS éditable (FAQ, tarifs, dates de la réforme). Formulaire branché sur l'outil d'inscription produit (création de compte par lien magique).

## 8. Livrables

1. Atelier de cadrage et plateforme de messages.
2. Wireframes mobile d'abord, puis desktop.
3. Maquettes haute fidélité (Figma), avec mockups d'application et kit de composants.
4. Micro-animations : montants, facture « payée », courbe de trésorerie.
5. Rédaction web.
6. Intégration, CMS, formulaire, plan de taggage.
7. Recette : accessibilité, performance, navigateurs et mobiles.
8. Passation et formation.

## 9. Planning indicatif

| Semaine | Étape |
|---|---|
| S1 | Cadrage, contenus, messages |
| S2 | Wireframes mobile et desktop, tests de recherche utilisateur (voir section 13) |
| S3 à S4 | Maquettes haute fidélité, mockups d'application |
| S5 | Rédaction finale, micro-animations |
| S5 à S6 | Intégration, CMS, taggage |
| S7 | Recette, mise en ligne |

**Total : 7 semaines.** À produire : les maquettes de l'application (mobile et desktop) qui servent de captures, puisque Liasse n'a pas de produit réel.

## 10. Budget

Pas de chiffrage. Liasse est fictive et aucune grille tarifaire publique d'agence ou de freelance n'a été ouverte pour cette passe. Hors périmètre : abonnement CMS et hébergement. Pas de shooting photo : le site montre les maquettes de l'application, pas des photos d'artisans.

## 11. Critères de réussite

- Un artisan comprend en 5 secondes ce que fait Liasse et ce qu'il doit faire pour la réforme (test sur 5 personnes).
- Inscription possible en un champ et un tap sur mobile.
- Toutes les dates et tous les chiffres sont cohérents d'une section à l'autre, datés et justifiables.
- WCAG AA sans non-conformité bloquante, Lighthouse ≥ 90.
- Indicateurs de la section 3 mesurables dès le premier jour.

## 12. UX copy

### Titre du hero recommandé
> **Vos factures électroniques, faites depuis votre téléphone.**
> Sous-titre : Devis, facture, relance et trésorerie à 90 jours, depuis votre téléphone. Recevez dès aujourd'hui, émettez sereinement avant septembre 2027.

### Alternatives

| Option | Texte | Ton | Idéal pour |
|---|---|---|---|
| A, réforme rassurante | « La facture électronique, sans prise de tête. Vous êtes prêt pour 2027. » | Rassurant | Artisans inquiets de la réforme (Mehdi) |
| B, être payé | « Facturez depuis le chantier. Les relances font le reste. » | Direct, bénéfice | Artisans et TPE qui émettent beaucoup |
| C, trésorerie | « Votre compte dans 90 jours, dès aujourd'hui. » | Projectif, calme | Gérantes et gérants qui pilotent (Nathalie), campagnes trésorerie |

### Libellés des CTA

| Emplacement | Libellé |
|---|---|
| Hero (avec le champ e-mail) | **Essayer gratuitement 30 jours** |
| Sous le bouton | « Sans carte bancaire. Sans engagement. » (c'est la règle de l'essai, voir section 7) |
| Échéancier | **Voir ce que je dois faire** (après choix du profil) |
| Aperçu de l'application | **Voir l'application en 30 secondes** |
| Experts-comptables | **Devenir cabinet partenaire** |
| Tarifs (par formule) | **Essayer Solo** / **Essayer Équipe** |
| Pied de page | **Créer mon compte** |

À éviter : « S'inscrire », « En savoir plus », « Valider ».

### Messages du formulaire d'inscription
- **Succès** : « C'est parti ! Nous venons d'envoyer un lien de connexion à [email]. Ouvrez-le sur ce téléphone pour créer votre première facture. Rien reçu dans 2 minutes ? Regardez dans vos indésirables. »
- **Erreur, e-mail invalide** : « Cette adresse ne semble pas complète. Il manque le "@" ou la fin (par exemple : .fr). Corrigez-la puis réessayez. »
- **Erreur, compte existant** : « Vous avez déjà un compte avec cette adresse. Pas besoin d'en créer un deuxième : recevez un lien de connexion. » Bouton : **Recevoir mon lien**.
- **Erreur d'envoi** : « L'inscription n'est pas passée. La connexion a été coupée. Votre adresse est gardée : appuyez à nouveau sur "Essayer gratuitement 30 jours". »

## 13. Mini plan de recherche utilisateur

- **Objectif** : vérifier que les artisans comprennent la promesse et l'échéancier, et que la trésorerie à 90 jours est perçue comme une raison de payer.
- **Méthode** : 5 entretiens suivis d'un test sur maquette mobile (45 min), en présentiel sur le lieu de travail quand c'est possible. Profils : 3 artisans du bâtiment, 1 commerçant, 1 expert-comptable. Recrutement via une chambre de métiers locale et des réseaux d'artisans.
- **Mesures** : compréhension en 5 secondes, réussite de l'inscription, bonne lecture de l'échéancier, objections spontanées.

### Guide d'entretien

1. **Mise en route** (5 min)
   - « Parlez-moi de votre activité : métier, nombre de personnes, type de clients. »
   - « On teste un site, pas vous. Dites tout ce qui vous passe par la tête. »
2. **Contexte** (10 min)
   - « Montrez-moi comment vous avez fait votre dernière facture. »
   - « Comment savez-vous aujourd'hui s'il y aura assez sur le compte le mois prochain ? »
   - « Qu'avez-vous entendu sur la facture électronique ? Par qui ? »
3. **Approfondissement** (10 min)
   - « Qu'est-ce qui vous fait perdre le plus de temps ou d'argent dans la facturation ? »
   - « Quel rôle joue votre comptable dans le choix de vos outils ? »
   - « Qu'est-ce qui vous ferait payer un outil alors que d'autres sont gratuits ? »
4. **Réaction à la maquette** (15 min)
   - Test de 5 secondes sur le hero mobile : « Que propose ce site ? »
   - Échéancier : « Choisissez votre profil. Que devez-vous faire, et avant quand ? »
   - Tâche : « Vous voulez essayer, allez-y. » Puis : « Que montre cette courbe ? »
5. **Conclusion** (5 min)
   - « Sur 5, à quel point êtes-vous rassuré sur la réforme après ce site ? »
   - « Qu'est-ce qui manque pour que vous essayiez ce soir ? »
