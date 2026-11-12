# Brief client : site vitrine Liasse

> **Document de démonstration.** Liasse est une entreprise FICTIVE créée pour illustrer la catégorie `vitrine-fintech-saas`. Ses chiffres, sa levée, son agrément, ses clients et ses personnes sont inventés. Le nom est provisoire : vérifier sa disponibilité à l'INPI avant toute réutilisation.

**Émetteur** : Liasse SAS (fictif), cofondatrice en charge du produit et du marketing
**Destinataire** : l'agence
**Date** : novembre 2026
**Version** : 1.0

---

## 1. Qui nous sommes

Liasse est l'application de facturation électronique et de trésorerie pensée pour les artisans et les TPE (de 0 à 10 salariés) :
- **Facturer** : devis, acompte et facture conformes, créés en 2 minutes depuis le téléphone, émis et reçus au format électronique.
- **Relancer** : relances automatiques et polies, avec un lien de paiement.
- **Voir venir** : la trésorerie projetée à 90 jours, à partir des factures émises, des factures reçues et du compte bancaire.
- **Transmettre** : export comptable et accès direct pour l'expert-comptable.

**Hypothèse de fiction** : Liasse est immatriculée plateforme agréée par la DGFiP. *Dans un vrai projet, cette mention n'est affichée qu'avec un numéro d'immatriculation réel.*

**Équipe** : 11 personnes à Nantes. **Utilisateurs** : 4 000 TPE, dont 60 % d'artisans du bâtiment (chiffres fictifs).

## 2. Contexte et déclencheur

- **Levée** : seed de 3,5 M€ en septembre 2026 (fictif), pour atteindre 40 000 utilisateurs avant l'échéance d'émission du 1er septembre 2027.
- **Réforme** : la réception des e-factures est obligatoire depuis le 1er septembre 2026. L'émission devient obligatoire pour les TPE le 1er septembre 2027. Les 10 prochains mois sont la fenêtre d'acquisition.
- **Concurrence** : plus de 100 plateformes agréées, et une conformité gratuite chez plusieurs acteurs (Abby, Indy, Tiime). Liasse doit gagner sur la **trésorerie**, les **relances** et le **ton artisan**.
- **Site actuel** : landing page de lancement. Le titre « Vos factures conformes 2026 » est dépassé, et le site ne parle ni de trésorerie ni aux experts-comptables.

**Affinement par rapport au README** : le hero passe de « Vos factures conformes 2026, en 2 minutes » à une formulation qui reste vraie après septembre 2026 (voir UX copy). « Agrément PDP » devient « plateforme agréée (PA) », l'appellation officielle actuelle.

## 3. Objectifs business et KPIs du site

| Objectif | KPI | Cible à 6 mois après la mise en ligne |
|---|---|---|
| Acquérir des essais | Taux d'inscription (visiteurs uniques vers e-mail envoyé) | ≥ 4 % (hypothèse à valider) |
| Activer | Part des inscrits qui créent une 1re facture sous 7 jours (mesuré côté produit) | ≥ 50 % |
| Mobile | Part des inscriptions faites sur mobile | ≥ 55 % |
| Prescription | Demandes de partenariat d'experts-comptables / mois | ≥ 20 |
| Réassurance | Clics vers l'échéancier de la réforme et la FAQ | Suivi, pas de cible |
| SEO | Top 10 sur « facture électronique artisan », « logiciel facturation artisan », « facturation électronique 2027 TPE » | 3 requêtes sur 5 |
| Performance | LCP mobile | < 2,5 s |

## 4. Cibles et personas

### Persona 1 : Mehdi, plombier-chauffagiste, 2 salariés
- **Job to be done** : « Quand je finis un chantier, je veux envoyer la facture depuis la camionnette et être payé sans courir après le client, pour ne pas faire la paperasse le soir. »
- **Situation** : devis et factures sur un tableur ou du papier carbone, beaucoup d'acomptes, des clients particuliers et des pros.
- **Attentes** : simple sur téléphone, devis transformé en facture en un geste, relances automatiques.
- **Freins** : « encore un abonnement », la peur de mal faire avec la réforme, aucune envie de lire du jargon.
- **Ce qu'il doit trouver** : des captures mobiles, « 2 minutes », un prix clair, et une réponse à « qu'est-ce que je dois faire et quand ? ».

### Persona 2 : Nathalie, gérante d'un salon de coiffure et d'une boutique, 6 salariés
- **Job to be done** : « Quand je regarde mon compte, je veux savoir si je pourrai payer mes fournisseurs et mes salaires dans 2 mois, pour décider sereinement d'un achat ou d'une embauche. »
- **Situation** : reçoit beaucoup de factures fournisseurs, en émet peu, et pilote sa trésorerie « au feeling ».
- **Attentes** : une vision de la trésorerie à 90 jours, la réception des e-factures centralisée.
- **Freins** : la sécurité des données bancaires, la peur de devoir tout ressaisir.
- **Ce qu'elle doit trouver** : l'aperçu de la courbe de trésorerie, la connexion bancaire expliquée, la sécurité (hébergement, chiffrement).

### Persona 3 : Julien, expert-comptable, cabinet de 12 personnes et 300 clients TPE
- **Job to be done** : « Quand la réforme impose l'e-facture à mes clients, je veux leur recommander un outil fiable qui m'envoie des données propres, pour ne pas gérer 300 migrations à la main. »
- **Attentes** : export vers son logiciel de production, accès multi-clients, accompagnement.
- **Freins** : un outil de plus à maîtriser, la perte de la relation avec ses clients.
- **Ce qu'il doit trouver** : une section dédiée avec bénéfices, formats d'export, invitation des clients et contact partenaire.

## 5. Messages clés et preuves

| Message | Preuve attendue sur le site |
|---|---|
| « Une facture conforme en 2 minutes, depuis votre téléphone » | Capture ou boucle mobile chronométrée |
| « Prêt pour l'émission de septembre 2027, dès aujourd'hui » | Échéancier par profil, numéro d'immatriculation PA (si réel) |
| « Payé plus vite » | Délai moyen de paiement avant et après les relances, avec périmètre et date |
| « Votre trésorerie à 90 jours, en un coup d'œil » | Aperçu de la courbe avec des montants animés |
| « Votre expert-comptable branché directement » | Formats d'export et logos des logiciels réellement compatibles |
| « Vos données sont protégées » | Hébergeur et région nommés, chiffrement, connexion bancaire via un agrégateur agréé (à préciser) |

Ton : simple, chaleureux, rassurant. Tutoiement exclu, vouvoiement direct. Pas de peur ni d'amendes en rouge. Les mots « disruptif » et « révolution » sont interdits.

## 6. Arborescence et contenus attendus

One-page avec ancres.
1. **Hero** : titre, sous-titre, **champ e-mail** et bouton « Essai gratuit 30 jours ». Capture mobile en premier sur téléphone.
2. **Échéancier de la réforme** : frise 2026–2027 et sélecteur « Je suis : artisan, commerçant, profession libérale, société ». Affiche « Ce que vous devez faire » pour le profil choisi.
3. **Fonctionnalités** : facture, relance, trésorerie, export comptable (4 cartes).
4. **Aperçu de l'application** : captures mobile et desktop, micro-animations sur les montants.
5. **Pour les experts-comptables** : bénéfices, export, invitation des clients, contact partenaire.
6. **Sécurité** : plateforme agréée (si réel), hébergement, chiffrement, données bancaires.
7. **Tarifs** : 2 ou 3 formules HT et TTC, et un comparatif « Liasse et les autres » factuel, sans nommer de concurrent sans vérification juridique.
8. **Avis clients, FAQ et inscription** : note moyenne, verbatims avec mention de leur mode de contrôle, FAQ de 8 à 10 questions, répétition du champ e-mail.

Pages satellites : `/mentions-legales`, `/confidentialite`, `/cookies`, `/cgu`, `/accessibilite`, `/experts-comptables` (version longue, phase 2).

## 7. Contraintes

- **Marque** : palette crème, violet profond, accent corail. Typo grotesque arrondie (DM Sans ou Outfit), chiffres tabulaires. Mockups soignés, micro-animations sur les montants.
- **Réglementaire** :
  - Mention « plateforme agréée » uniquement avec une immatriculation réelle, numéro affiché.
  - Avis en ligne : informer sur l'existence et le mode de contrôle des avis (Code de la consommation).
  - Prix : HT et TTC lisibles, conditions de l'essai (sans carte bancaire ? reconduction ?) écrites à côté du bouton.
  - Données bancaires : préciser le prestataire d'agrégation et son statut réglementaire. Ne pas laisser entendre que Liasse est une banque.
  - RGPD et cookies : consentement conforme aux recommandations de la CNIL.
- **Accessibilité** : WCAG 2.1 AA (RGAA 4.1). Le corail ne sert jamais au texte sur fond crème (contraste insuffisant probable), les animations de montants respectent `prefers-reduced-motion`, les cibles tactiles font au moins 44 px, la frise est lisible sans couleur.
- **SEO** : HTML indexable, FAQPage et SoftwareApplication en données structurées, contenu réforme daté et mis à jour.
- **Langues** : français uniquement.
- **Technique** : CMS éditable par l'équipe (FAQ, tarifs, avis, dates de la réforme). Formulaire branché sur l'outil d'inscription produit (création de compte par lien magique).

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

**Total : 7 semaines.** Point d'attention : les captures de l'application doivent refléter la version produit au moment de la mise en ligne.

## 10. Budget

| Prestataire | Périmètre | Fourchette HT |
|---|---|---|
| Freelance | One-page, mockups à partir des captures fournies, rédaction légère | 4 000 à 9 000 € |
| Petit studio | Périmètre complet | 10 000 à 22 000 € |
| Agence établie | Périmètre complet, page experts-comptables longue, motion avancé | 22 000 à 40 000 € |

Hors budget : abonnement CMS et hébergement, shooting photo d'artisans (2 000 à 4 000 € si réel).
**Enveloppe Liasse : 14 000 à 20 000 € HT.**

## 11. Critères de réussite

- Un artisan comprend en 5 secondes ce que fait Liasse et ce qu'il doit faire pour la réforme (test sur 5 personnes).
- Inscription possible en un champ et un tap sur mobile.
- Toutes les dates et tous les chiffres sont cohérents d'une section à l'autre, datés et justifiables.
- WCAG AA sans non-conformité bloquante, Lighthouse ≥ 90.
- KPIs mesurables dès le premier jour.

## 12. UX copy

### Titre du hero recommandé
> **Vos factures électroniques, prêtes en 2 minutes.**
> Sous-titre : Devis, facture, relance et trésorerie à 90 jours, depuis votre téléphone. Recevez dès aujourd'hui, émettez sereinement avant septembre 2027.

### Alternatives

| Option | Texte | Ton | Idéal pour |
|---|---|---|---|
| A, réforme rassurante | « La facture électronique, sans prise de tête. Vous êtes prêt pour 2027. » | Rassurant | Artisans inquiets de la réforme (Mehdi) |
| B, être payé | « Facturez en 2 minutes. Soyez payé plus vite. » | Direct, bénéfice | Artisans et TPE qui émettent beaucoup |
| C, trésorerie | « Votre compte dans 90 jours, dès aujourd'hui. » | Projectif, calme | Gérantes et gérants qui pilotent (Nathalie), campagnes trésorerie |

### Libellés des CTA

| Emplacement | Libellé |
|---|---|
| Hero (avec le champ e-mail) | **Essayer gratuitement 30 jours** |
| Sous le bouton | « Sans carte bancaire. Sans engagement. » (à confirmer) |
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
- **Méthode** : 5 entretiens suivis d'un test sur maquette mobile (45 min), en présentiel sur le lieu de travail quand c'est possible. Profils : 3 artisans du bâtiment, 1 commerçant, 1 expert-comptable. Recrutement via les utilisateurs actuels et une chambre de métiers locale.
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
