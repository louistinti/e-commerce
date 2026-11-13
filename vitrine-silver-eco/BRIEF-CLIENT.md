# Brief client : site vitrine Les Jours Tranquilles

> **Entreprise fictive**, utilisée comme cas de démonstration par l'agence. Personne ne valide rien : l'agence décide tout. **Aucun chiffre n'est inventé** : toute donnée chiffrée cite sa source (nom, URL, date de consultation). Les valeurs de conception (px, contrastes, semaines, nombre de champs) sont des spécifications. Le nom n'est pas déposé : on ne le réutilise pas pour un vrai projet sans recherche INPI.

**Émetteur** : Les Jours Tranquilles (SAS, service d'aide à domicile prestataire), gérance et responsable de secteur
**Destinataire** : agence web
**Date** : novembre 2026
**Version** : 1.1

---

## 1. Présentation de l'entreprise

- **Activité** : aide à domicile pour personnes âgées (ménage, repas, courses, compagnie, aide au lever et au coucher), en mode **prestataire** : nous employons les auxiliaires, la famille n'a aucune démarche d'employeur.
- **Promesse** : une **auxiliaire attitrée** pour chaque personne accompagnée, et un **lien quotidien avec la famille** (compte-rendu de passage par SMS ou application).
- **Taille** : une agence locale, une équipe d'auxiliaires de vie salariées, une zone d'intervention autour d'une ville moyenne. Aucun effectif chiffré : l'entreprise est fictive.
- **Ville** : aucune ville réelle. La démo écrit « votre ville » dans le surtitre et les gabarits de requêtes, et montre une carte illustrée au trait avec des communes fictives.
- **Statut** : service d'aide et d'accompagnement à domicile (SAAD) autorisé par le conseil départemental, déclaration de services à la personne (SAP) ouvrant droit au crédit d'impôt. Sur la démo, les emplacements du n° d'autorisation et du n° SAP affichent « numéro de démonstration », jamais un numéro inventé.

## 2. Contexte et déclencheur

- Le site actuel est ancien, pas responsive, sans tarifs, avec un formulaire long : il ne génère presque aucune demande.
- La plupart de nos nouveaux clients arrivent par le bouche-à-oreille et les prescripteurs (assistantes sociales hospitalières, CCAS, médecins). Or les familles nous disent toutes « avoir regardé le site avant d'appeler ».
- **Déclencheurs** :
  1. Ouverture d'un second secteur géographique.
  2. Lancement du compte-rendu de passage par SMS pour les familles, notre différence clé.
  3. Concurrence accrue de réseaux nationaux bien référencés sur notre zone.

## 3. Objectifs business et indicateurs

Indicateurs à suivre, **sans cible chiffrée** : l'entreprise est fictive et aucun historique ne permet d'en fixer une.

| Objectif | Indicateur à suivre |
|---|---|
| Générer des demandes de rappel | Formulaires de rappel envoyés, par mois |
| Générer des appels | Clics sur le numéro (suivis en événement), par mois |
| Convertir | Part des demandes qui donnent lieu à une visite d'évaluation |
| Rassurer sur le prix | Part des visiteurs mobiles qui atteignent la section « Tarifs et aides » (scroll ou ancre) |
| Recruter des auxiliaires (secondaire) | Candidatures via la page dédiée, par mois |
| SEO local | Positions sur les requêtes « aide à domicile + ville » et « auxiliaire de vie + ville » |
| Accessibilité | Audit WCAG 2.2 AA : aucune non-conformité bloquante |

## 4. Cibles et personas

### Persona 1 : Nathalie, 54 ans, fille d'une mère de 84 ans qui vit seule à 40 km
- **Rôle** : acheteuse et décisionnaire de fait. Elle cherche sur son téléphone, souvent au travail ou le soir.
- **Job to be done** : « Quand ma mère ne peut plus tout gérer seule, je veux trouver vite une aide fiable dont je connais le coût réel, pour qu'elle reste chez elle et que je sois rassurée sans être sur place tous les jours. »
- **Déclencheur** : une chute, une sortie d'hôpital, un frigo vide découvert le dimanche.
- **Attentes** : savoir qui viendra (toujours la même personne ?), combien ça coûte vraiment après les aides, à quelle vitesse ça peut démarrer, et comment elle saura que tout s'est bien passé.
- **Freins** : la culpabilité, la peur de la rotation des intervenants, la peur de la paperasse, un prix opaque, et le refus de sa mère (« je n'ai besoin de personne »).
- **Ce qu'elle doit trouver** : la promesse, le téléphone, l'exemple de calcul, l'exemple de compte-rendu SMS et le formulaire de rappel en 2 champs.

### Persona 2 : Robert, 81 ans, veuf, autonome mais fatigué
- **Rôle** : bénéficiaire. Il lit le site sur la tablette offerte par son fils.
- **Job to be done** : « Quand les tâches du quotidien deviennent fatigantes, je veux être aidé sans perdre la main sur mes habitudes, pour continuer à vivre chez moi comme je l'entends. »
- **Attentes** : être respecté, garder la main sur ses habitudes, savoir qui entre chez lui.
- **Freins** : la perte d'autonomie perçue comme une humiliation, la méfiance envers les inconnus, la difficulté de lecture.
- **Ce qu'il doit trouver** : un ton qui lui parle d'égal à égal, le principe d'une auxiliaire attitrée qu'on lui présente avant le premier passage, un grand numéro de téléphone, aucun jargon.

### Persona 3 : Karima, 42 ans, assistante sociale au service de soins de suite de l'hôpital
- **Rôle** : prescriptrice. Elle oriente les familles à la sortie.
- **Job to be done** : « Quand un patient âgé sort d'hospitalisation, je veux orienter sa famille vers un service qui rappelle et démarre vite, pour sécuriser la sortie. »
- **Attentes** : des délais de mise en place, la zone couverte, le type d'aides acceptées (APA, caisses de retraite, mutuelles), un interlocuteur direct.
- **Freins** : des services qui ne rappellent pas, des délais non tenus.
- **Ce qu'elle doit trouver** : la zone d'intervention, le bloc « sortie d'hôpital » et une ligne directe ou un e-mail professionnel.

## 5. Messages clés et preuves

| Message | Preuve |
|---|---|
| « Vos parents chez eux, bien entourés » | Promesse globale (hero) |
| « La même auxiliaire, semaine après semaine » | Remplaçante présentée à l'avance. Aucun taux de continuité affiché : il n'existe pas de chiffre réel |
| « Vous savez comment s'est passée la visite » | Exemple de compte-rendu rédigé par nous, marqué « exemple » |
| « Le vrai prix, aides déduites » | Exemple de calcul sur un tarif de démonstration sourcé (section 6, bloc 5) ; lien vers la fiche Service Public |
| « Des auxiliaires formées et accompagnées » | Diplômes nommés (DEAES, titre ADVF) et formation continue, sans volume horaire inventé |
| « On vous rappelle aujourd'hui » | Formulaire de rappel en 2 champs et bloc sortie d'hôpital. Aucun délai chiffré |
| « Les familles en parlent » | Bloc avis au format vérifiable (source, période de collecte, modération), rempli d'avis d'exemple marqués comme tels, sans note ni nombre |
| « Service autorisé par le Département » | Emplacements du n° d'autorisation et du n° SAP, marqués « numéro de démonstration » |

**Ton** : chaleureux, humain, respectueux. Toujours « vous », « votre père », « votre mère ». **Interdits** : « nos aînés », « nos petits vieux », « mamie », « dépendant » employé comme étiquette, pathos sur la solitude, promesses de santé.

## 6. Arborescence et contenus attendus

One-page avec ancres, plus des pages annexes.

1. **Hero** : illustration au trait chaleureuse (une auxiliaire et une personne âgée qui cuisinent ensemble), le titre « Vos parents chez eux, bien entourés », le CTA « Être rappelé aujourd'hui » et le téléphone en grand.
2. **Les services** : 6 cartes simples (ménage et linge, repas, courses et sorties, compagnie, lever et coucher et toilette, présence de nuit). Chaque carte : une icône, un titre, une phrase.
3. **Comment ça se passe** : 1. premier appel, 2. visite d'évaluation gratuite à domicile, 3. présentation de l'auxiliaire attitrée, 4. premier passage, puis un premier point avec la famille.
4. **Le lien avec la famille** : maquette de téléphone avec un exemple de compte-rendu, marqué « exemple » (« Passage de 9 h à 11 h. Repas préparé, courses faites. Mme D. était en forme, elle a parlé de son petit-fils. »), choix entre SMS et application.
5. **Tarifs et aides** : un tarif horaire TTC de démonstration, marqué « tarif d'exemple » : **35,50 € TTC de l'heure**, calé sur le tarif public d'une aide à domicile jusqu'à 25 h par semaine à l'agence [Petits-fils Bordeaux Chartrons](https://www.petits-fils.com/nos-agences/agence-aide-a-domicile-bordeaux-chartrons/#tarifs) (vu le 2026-11-13 ; réseau mandataire, cité comme repère public et non comme notre prix). Exemple de calcul : 10 h par semaine, soit 355 € TTC, ou 177,50 € après le crédit d'impôt de 50 %, hors APA. Puis les explications sur l'APA, le crédit d'impôt et l'avance immédiate, les liens vers les sources officielles et le CTA « Recevoir un devis gratuit ».
6. **Qui sommes-nous** : un bloc court, sans photo, avec le logo. Texte : « Les Jours Tranquilles est un service d'aide à domicile de proximité. Nous employons nos auxiliaires de vie, formées et accompagnées par une responsable de secteur. Chaque personne a son auxiliaire attitrée, et sa famille reçoit des nouvelles après chaque passage. »
7. **Avis des familles** : 3 à 5 avis d'exemple, marqués « avis d'exemple », avec l'emplacement de la source et de la période de collecte. Pas de note globale ni de nombre d'avis.
8. **Zone d'intervention et contact** : carte illustrée au trait et liste de communes fictives, téléphone en très grand (« 0X XX XX XX XX » sur la démo, pour ne jamais tomber sur un vrai abonné), formulaire de rappel (nom, téléphone), horaires et adresse de l'agence marqués « démonstration ».

**Bloc transverse** : « Votre parent sort de l'hôpital ? », placé entre les sections 3 et 4 et repris dans le pied de page.

**Pages annexes** : « Nous rejoindre » (recrutement d'auxiliaires), mentions légales (avec les emplacements des numéros d'autorisation et de SAP), tarifs détaillés (document téléchargeable), confidentialité, cookies, déclaration d'accessibilité, modération des avis.

**À produire par l'agence** : toute la rédaction, l'exemple de compte-rendu, les avis d'exemple, le bloc tarif sourcé, les icônes, l'illustration du hero, le logo, la carte illustrée de la zone, le SEO local.

## 7. Contraintes

### Marque et direction artistique (reprend le README)
- Palette crème, terracotta douce et vert olive. Typo serif douce pour les titres (Lora) et sans-serif très lisible (Atkinson Hyperlegible) en **18 px minimum**.
- Visuels : aucune photo de personne (Unsplash et Pexels ont bloqué la recherche de photos, voir le bench). Illustrations au trait, personnes actives (en train de cuisiner, de discuter, de marcher), jamais de gros plans sur des mains ridées, ni canne, ni fauteuil roulant, ni blouse médicale.

### Réglementaire (services à la personne)
- **Information préalable sur les prix** : on affiche les prix TTC des prestations et on annonce un devis personnalisé gratuit, comme le prévoit l'arrêté du 17 mars 2015.
- **Crédit d'impôt** : on présente le mécanisme tel que l'affiche la [fiche F12 de Service Public](https://www.service-public.gouv.fr/particuliers/vosdroits/F12) (fiche vérifiée le 15 avril 2026, onglet « Emploi en 2025 », vu le 2026-11-13) : 50 % des dépenses, retenues dans la limite de 12 000 € par an, plafond majoré de 1 500 € par membre du foyer ou ascendant de plus de 65 ans, sans dépasser 15 000 € au total. Les aides reçues, dont l'APA, se déduisent des dépenses. Lien vers la fiche et mention « sous réserve de la législation en vigueur ».
- **Avance immédiate** : on présente le mécanisme de l'Urssaf et on précise qu'il est réservé aux services inscrits. La démo ne prétend pas que Les Jours Tranquilles y est inscrite.
- **Mentions** : emplacements des numéros d'autorisation du conseil départemental et de déclaration SAP dans les mentions légales et le pied de page, marqués « numéro de démonstration ».
- **Avis en ligne** : la page de modération dit si les avis sont contrôlés et comment (Code de la consommation, art. L111-7-2). Sur la démo, elle précise que les avis affichés sont des avis d'exemple.
- **RGPD** : formulaire minimal (nom, téléphone), finalité claire (rappel), durée de conservation, aucune donnée de santé collectée via le site. Bandeau cookies conforme aux lignes directrices de la CNIL.
- **Droit à l'image** : sans objet, la démo n'utilise aucune photo de personne.

### Accessibilité
- Cible : WCAG 2.2 AA, et plus : contraste ≥ 7:1 pour le corps de texte (niveau AAA, critère 1.4.6), cibles tactiles ≥ 48 px (valeur de conception, au-dessus des 44 px du critère 2.5.5), texte zoomable à 200 % sans perte (critère 1.4.4).
- Numéro de téléphone cliquable (`tel:`) **en haut de chaque écran**, en barre fixe sur mobile.
- Pas de carrousel automatique, pas de texte sur image sans voile, pas d'information par la seule couleur.
- Test de lecture auprès de 3 personnes de plus de 75 ans et de 3 enfants adultes.

### SEO
- SEO local prioritaire : données structurées `LocalBusiness` adaptées, NAP cohérent partout. La fiche Google Business Profile est rédigée mais jamais publiée : l'entreprise est fictive.
- Gabarits de requêtes : « aide à domicile + ville », « auxiliaire de vie + ville », « aide à domicile personne âgée + département », « sortie d'hôpital aide à domicile ».
- Une page par secteur géographique seulement si le contenu est réellement différent (pas de pages-villes générées en masse).

### Langues
- Français uniquement.

## 8. Plan de recherche utilisateur (mini)

- **Objectif** : vérifier que (1) l'enfant adulte trouve le prix réel et le moyen d'être rappelé en moins de 30 secondes, (2) le ton est perçu comme respectueux par les seniors, (3) le compte-rendu de passage est compris comme rassurant et non intrusif.
- **Méthode** : **5 entretiens suivis d'un test sur maquette** (fin S4) : 3 enfants adultes de 45 à 60 ans ayant un parent aidé ou sur le point de l'être (à distance, sur leur téléphone) et 2 seniors de plus de 75 ans (à domicile, sur tablette). 45 minutes, consentement écrit, enregistrement audio.
- **Recrutement** : via un CCAS et des associations d'aidants.
- **Mesures** : réussite des tâches (« Combien paierez-vous pour 10 h par semaine ? », « Demandez à être rappelé »), temps, verbatims, mots qui gênent.

### Guide d'entretien en 5 temps

1. **Mise en route (5 min)**
   - « Pouvez-vous vous présenter, et me dire qui vous aidez ou qui vous aide ? »
   - « Quel appareil utilisez-vous le plus pour chercher une information ? »
2. **Contexte (10 min)**
   - Enfants : « Racontez-moi le moment où vous vous êtes dit qu'il fallait de l'aide pour votre parent. »
   - Seniors : « Comment se passe une journée type chez vous ? Qu'est-ce qui est devenu plus difficile ? »
   - « Comment avez-vous cherché, ou comment chercheriez-vous, un service d'aide ? »
3. **Approfondissement (10 min)**
   - « Qu'est-ce qui vous inquiète le plus quand quelqu'un vient à domicile ? »
   - « Qu'est-ce qui vous ferait choisir un service plutôt qu'un autre ? »
   - Seniors : « Quels mots ou quelles images vous agacent dans les publicités pour les seniors ? »
4. **Réaction à la maquette (15 min)**
   - « Regardez cette page 5 secondes. De quoi s'agit-il, et pour qui ? »
   - Tâches : trouver le prix pour 10 h par semaine, demander à être rappelé, trouver si sa commune est desservie.
   - « Voici un exemple de message envoyé après une visite. Qu'en pensez-vous ? Rassurant, intrusif ? »
5. **Conclusion (5 min)**
   - « Qu'est-ce qui vous donnerait envie d'appeler ? Et qu'est-ce qui vous retiendrait ? »
   - « Si vous deviez changer une seule chose, ce serait quoi ? »

## 9. UX copy

### Titre du hero

**Recommandé** : « Vos parents chez eux, bien entourés »
*Sous-titre* : « Une auxiliaire attitrée pour le ménage, les repas, les courses et la compagnie, et un message à la famille après chaque passage. »

| Option | Texte | Ton | Idéal pour |
|---|---|---|---|
| A | « La même auxiliaire chaque semaine, et des nouvelles après chaque visite » | Concret, factuel | Familles qui comparent plusieurs services |
| B | « Rester chez soi, avec quelqu'un sur qui compter » | Chaleureux, du point de vue du senior | Seniors lecteurs, campagne locale (presse, affichage) |
| C | « Votre parent sort de l'hôpital ? On s'organise avec vous dès cette semaine. » | Urgent et rassurant | Landing sortie d'hôpital, prescripteurs |

### Libellés des CTA

| Emplacement | Libellé |
|---|---|
| Hero | « Être rappelé aujourd'hui » |
| Barre mobile | « Appeler le 0X XX XX XX XX » |
| Services | « Voir comment ça se passe » |
| Tarifs et aides | « Recevoir un devis gratuit » |
| Bloc sortie d'hôpital | « Organiser une aide dès cette semaine » |
| Zone d'intervention | « Vérifier si ma commune est desservie » |
| Page recrutement | « Postuler comme auxiliaire de vie » |

### Messages du formulaire de rappel

**Succès** : « C'est noté, [Nom]. Nous vous rappelons aujourd'hui au [numéro saisi], ou le jour ouvré suivant si votre demande arrive après la fermeture. Si c'est urgent, appelez-nous directement au 0X XX XX XX XX. »

**Erreurs** (structure : ce qui s'est passé, pourquoi, comment corriger)

| Cas | Message |
|---|---|
| Téléphone incomplet | « Ce numéro semble incomplet : il contient 9 chiffres au lieu de 10. Vérifiez-le, par exemple 06 12 34 56 78. » |
| Nom vide | « Votre nom est manquant. Nous en avons besoin pour savoir qui demander au téléphone. Indiquez-le pour continuer. » |
| Échec d'envoi | « Votre demande n'a pas pu être envoyée, car la connexion a été interrompue. Votre nom et votre numéro sont conservés : appuyez à nouveau sur « Être rappelé aujourd'hui », ou appelez-nous au 0X XX XX XX XX. » |

Règles : texte d'erreur en 18 px sous le champ, icône et couleur `color-error`, annoncé aux lecteurs d'écran (`aria-live="polite"`), aucune donnée effacée en cas d'erreur.

## 10. Livrables

1. Atelier de cadrage (2 h) et arborescence.
2. Wireframes mobile d'abord, puis desktop.
3. Maquettes UI (Figma) : home, recrutement, mentions.
4. Kit de composants : boutons, cartes de service, bloc tarif, bloc avis, barre d'appel mobile.
5. Illustrations au trait (hero, carte de la zone) et logo pour le bloc « Qui sommes-nous ».
6. Intégration responsive (WordPress ou Webflow), formulaire de rappel relié à l'e-mail et au CRM, suivi des clics sur le téléphone.
7. Contenu de la fiche Google Business Profile, rédigé et non publié (entreprise fictive).
8. Audit d'accessibilité et déclaration, recette, mise en ligne, formation (1 h).

## 11. Planning indicatif

| Semaine | Étape |
|---|---|
| S1 | Cadrage, rédaction des contenus de démonstration (tarif sourcé, avis d'exemple, compte-rendu) |
| S2 | Arborescence, wireframes, rédaction |
| S3-S4 | Maquettes UI, illustrations |
| S5-S6 | Intégration, formulaire, suivi |
| S7 | Tests d'accessibilité et utilisateurs, corrections, SEO local |
| S8 | Recette, mise en ligne |

Durée : **6 à 8 semaines**.

## 12. Budget

Pas de budget chiffré. L'entreprise est fictive et aucune grille tarifaire publique n'a été ouverte pour ce dossier : toute fourchette serait inventée.

## 13. Critères de réussite

- Une fille ou un fils trouve le prix réel après les aides **en moins de 30 secondes** sur mobile (test sur maquette).
- Une personne de plus de 75 ans lit le hero et la section services sans zoomer, et trouve le numéro immédiatement (3 testeurs sur 3).
- Le formulaire de rappel s'envoie en moins de 20 secondes.
- Les indicateurs de la section 3 sont suivis dès la mise en ligne (événements du formulaire et des clics sur le numéro).
- Aucune photo de personne ; les illustrations respectent les interdits de la section 5 et de la section 7.
- Audit AA sans non-conformité bloquante ; corps de texte ≥ 18 px partout.
- Les mentions réglementaires suivent les textes cités en section 7 : arrêté du 17 mars 2015 (prix TTC, devis gratuit), fiche Service Public F12 (crédit d'impôt), art. L111-7-2 du Code de la consommation (avis).
