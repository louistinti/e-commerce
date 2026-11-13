# Étude de cas : site vitrine d'une fintech ou d'un SaaS de gestion pour TPE

> Catégorie `vitrine-fintech-saas`. Entreprise de démonstration : **Liasse**, entreprise FICTIVE (facturation électronique et trésorerie pour artisans et TPE). Aucun chiffre n'est inventé : chaque donnée chiffrée porte sa source.
> Recherche documentaire de novembre 2026. Les sites ont été ouverts avec un vrai navigateur le 2026-11-12 (voir le [bench](BENCH.md)), et les chiffres de marché revus sur leur source le 2026-11-13. Voir les **Notes de méthode**.

## Executive summary

La réforme de la facturation électronique a fait émerger plus d'une centaine de solutions agréées. La facturation conforme est désormais gratuite chez plusieurs acteurs (Abby, Indy, Tiime) ou incluse dans les forfaits (Qonto) : la conformité ne différencie plus. Les 6 sites analysés parlent tous de la réforme, mais peu s'adressent vraiment aux artisans, et plusieurs se contredisent sur leurs prix ou leurs chiffres. Pour Liasse, l'opportunité est de vendre la **trésorerie à 90 jours** et les relances automatiques aux artisans, avec un calendrier à jour (émission en septembre 2027) et des chiffres cohérents et sourcés.

---

## 1. Le marché en 5 lignes

- **Calendrier** : toutes les entreprises assujetties à la TVA doivent pouvoir recevoir des factures électroniques depuis le 1er septembre 2026. Les PME, TPE et micro-entreprises devront les émettre à partir du 1er septembre 2027 ([Moneyvox](https://www.moneyvox.fr/actu/110141/facturation-electronique-ce-qui-change-vraiment-a-partir-du-1er-septembre-2026), article du 28 août 2026, vu le 2026-11-13).
- **Offre pléthorique** : « 118 solutions sont d'ores et déjà agréées par la DGFIP » en janvier 2026 ([Moneyvox](https://www.moneyvox.fr/banque-pro/actualites/107100/compte-pro-qonto-officiellement-agreee-comme-plateforme-de-facturation-electronique), article du 14 janvier 2026, vu le 2026-11-13). La liste officielle est publiée sur [impots.gouv.fr](https://www.impots.gouv.fr/je-consulte-la-liste-des-plateformes-agreees) (vu le 2026-11-13).
- **Levées et consolidation** : Pennylane a levé 75 M€ ([FrenchWeb](https://www.frenchweb.fr/pennylane-leve-75-millions-deuros-pour-simposer-dans-la-facturation-electronique/453106), 7 avril 2025, vu le 2026-11-13), Abby 3 M€ ([Le Journal des entreprises](https://www.lejournaldesentreprises.com/article/avec-un-nouveau-tour-de-table-abby-consolide-ses-positions-avant-la-generalisation-de-la-facture-2126878), 22 septembre 2025, vu le 2026-11-13). Libeo a rejoint Shine (groupe Cegid) ([FrenchWeb](https://www.frenchweb.fr/specialiste-de-la-gestion-et-du-paiement-des-factures-fournisseurs-libeo-rejoint-shine-cegid/463715), 28 septembre 2026, vu le 2026-11-13).
- **La conformité devient gratuite** : « Plateforme Agréée Tiime gratuite » ([tiime.fr](https://www.tiime.fr/), vu le 2026-11-13) ; « Un socle gratuit avec tous les essentiels » chez Indy ([indy.fr/artisan](https://www.indy.fr/artisan/), vu le 2026-11-13) ; module de facturation électronique « inclus dans le plan gratuit » d'Abby (Le Journal des entreprises, lien ci-dessus) ; facturation électronique conforme incluse dans l'offre Basic de Qonto, 9 € HT par mois en abonnement annuel ([qonto.com/fr/pricing](https://qonto.com/fr/pricing), vu le 2026-11-13). Bpifrance propose aussi un prêt dédié à la transition ([Bpifrance Création](https://bpifrance-creation.fr/entrepreneur/actualites/financez-votre-transition-facturation-electronique)).
- **Conséquence pour le site** : en novembre 2026, le visiteur ne veut plus savoir que « la réforme arrive ». Il veut savoir quoi faire avant septembre 2027 et ce que l'outil lui apporte (relances, trésorerie).

---

## 2. Critique de 6 sites réels

> Grille : première impression (2 s), usabilité, hiérarchie visuelle, accessibilité, ce qui marche, recommandations. Les observations viennent du bench (pages ouvertes le 2026-11-12) ou d'une page rouverte le 2026-11-13. *[non vu]* signale un point issu de la presse ou de descriptions, sur un site qui n'a pas pu être ouvert.

### 2.1 Pennylane : https://www.pennylane.com/fr/logiciel-facturation-electronique?so=1
Compta et finance pour PME et experts-comptables. Facturation électronique « incluse dans tous nos plans », formules « À partir de » 7, 14 et 24 € par mois HT, « 15 jours d'essai gratuit, sans engagement » (page ci-dessus, vu le 2026-11-13).
- **Première impression** : entrée par cible en onglets (« Indépendants et TPE », « PME et ETI », « Cabinet expertise comptable »). On sait vite si on est concerné.
- **Usabilité** : navigation riche, mais longue pour un artisan qui cherche juste à facturer. En mobile (390 px), les onglets de cible sont tronqués (bench).
- **Hiérarchie** : la conformité d'abord, avec un échéancier en 3 cartes datées, puis le reste de la plateforme.
- **Accessibilité** : prix en vert `#00BD57` sur blanc, à 2,5:1, sous le seuil de 4,5:1 de WCAG 2.1 (mesuré dans le bench, n° 21). Échéancier lisible sans couleur.
- **Ce qui marche** : un vrai parcours pour les experts-comptables, le prescripteur clé, et le logo officiel « Plateforme agréée » dans le hero.
- **Recommandations** : 1) retirer « Évitez les amendes » de l'échéancier et mettre à jour l'onglet du navigateur qui dit encore « préparez-vous pour 2026 » (bench, n° 6) ; 2) afficher le numéro d'immatriculation à côté du logo « Plateforme agréée ».

### 2.2 Abby : https://abby.fr/facturation-electronique
Facturation pour les indépendants. Le site renvoie une erreur 403 à un navigateur automatisé (bench le 2026-11-12, nouvel essai le 2026-11-13). Ce qui suit vient de la presse : la facturation électronique est « incluse dans le plan gratuit », Abby figure dans la liste des plateformes reconnues par l'État et revendique « plus de 100 000 » utilisateurs ([Le Journal des entreprises](https://www.lejournaldesentreprises.com/article/avec-un-nouveau-tour-de-table-abby-consolide-ses-positions-avant-la-generalisation-de-la-facture-2126878), 22 septembre 2025, chiffre déclaré par l'entreprise).
- **Première impression** : la gratuité et la conformité comme message principal *[non vu]*.
- **Usabilité** : pages par profil ([micro-entreprise](https://abby.fr/pour-qui/micro-entreprise), [freelance](https://abby.fr/pour-qui/freelance)) et calendrier de la réforme *[non vu]*.
- **Hiérarchie** : non observée.
- **Accessibilité** : non observable.
- **Ce qui marche** : d'après la presse, une pédagogie de la réforme et un ton accessible. C'est sans doute le concurrent le plus proche de Liasse en ton.
- **Recommandations** : 1) contenus propres aux artisans (devis, acomptes, chantier) ; 2) donner plus de place à la trésorerie.

### 2.3 Indy : https://www.indy.fr/artisan/
Compta, facturation et compte pro pour les indépendants, « Conforme à la réforme de la facturation électronique », expert-comptable en option (page ci-dessus, vu le 2026-11-13).
- **Première impression** : pastille « + de 10 000 Artisans déjà clients ! », titre « L'application tout-en-un des artisans », hero crème `#FEF7EC` avec une photo d'artisan et une carte « Facture électronique · Payée » (bench, n° 16).
- **Usabilité** : une page par statut (artisan, profession libérale, auto-entrepreneur), avec des pages [prix](https://www.indy.fr/prix/) et [témoignages](https://www.indy.fr/temoignages/?ae=1120). En mobile, 2 boutons pleine largeur de 48 px.
- **Hiérarchie** : promesse, puis notes (Trustpilot 4,8 et « +16 000 avis »), puis offre.
- **Accessibilité** : bouton rose `#FA5D89` à texte blanc, à 3,0:1, sous 4,5:1 (mesuré dans le bench).
- **Ce qui marche** : une page artisans dédiée, un découpage par statut, des notes avec leur source et leur volume.
- **Recommandations** : 1) aligner le prix du hero (« A partir de 12€ /mois ») et « Un socle gratuit avec tous les essentiels » annoncé plus bas sur la même page ; 2) dater les chiffres.

### 2.4 Qonto : https://qonto.com/fr?tp=1 et https://qonto.com/fr/accountants/for-your-clients
Compte pro avec facturation électronique conforme incluse, dès l'offre Basic à 9 € HT par mois en abonnement annuel ([tarifs](https://qonto.com/fr/pricing), vu le 2026-11-13). Agréée par la DGFiP comme plateforme de facturation électronique en janvier 2026 ([Moneyvox](https://www.moneyvox.fr/banque-pro/actualites/107100/compte-pro-qonto-officiellement-agreee-comme-plateforme-de-facturation-electronique), vu le 2026-11-13).
- **Première impression** : carte bancaire noire en 3D sur fond noir, titre « Compte pro. Financement. Facturation électronique. » : la facturation arrive en troisième (bench, n° 2).
- **Usabilité** : CTA d'ouverture de compte, espace experts-comptables complet (invitation des clients « en un clic », bouton « Parler à un conseiller »).
- **Hiérarchie** : compte, puis financement, puis facturation. Bon pour une néobanque, moins lisible pour qui cherche « facture conforme ».
- **Accessibilité** : non mesurée.
- **Ce qui marche** : les numéros réglementaires écrits en pied de page (ACPR, ORIAS, RCS). L'espace experts-comptables est un modèle.
- **Recommandations** : 1) afficher le numéro d'immatriculation de plateforme agréée, absent des 3 pages ouvertes dans le bench, à côté de « Certifié Plateforme Agréée » ; 2) un seul nombre de clients sur toutes les pages (« 600 000 entreprises » sur la page experts-comptables, « 750 000 » sur l'accueil, bench).

### 2.5 Agicap : https://agicap.com/fr/
Trésorerie pour PME et ETI : « Plus de 8 000 directions financières de PME et ETI utilisent Agicap » ([agicap.com/fr](https://agicap.com/fr/), vu le 2026-11-13). Prévisions de trésorerie, facturation électronique, paiements, recouvrement.
- **Première impression** : courbe de trésorerie et logos d'entreprises *[non vu]*. Cible PME et ETI explicite.
- **Usabilité** : pages par taille ([PME](https://agicap.com/fr/entreprise/pme-large/)), ressources expertes.
- **Hiérarchie** : produit (prévision), puis preuves, puis contenus.
- **Accessibilité** : non observable.
- **Ce qui marche** : la projection de trésorerie montrée visuellement. C'est la référence pour la section « 90 jours » de Liasse.
- **Recommandations** (si l'on visait les TPE) : 1) remplacer le jargon (« atterrissages de trésorerie », « DSO », vus sur l'accueil le 2026-11-13) par des mots du quotidien ; 2) un horizon simple (« dans 30, 60, 90 jours »).

### 2.6 Mercury : mercury.com (États-Unis, référence)
Analyses : [SaaS Landing Page](https://saaslandingpage.com/mercury/), [Landing Doctors](https://landingdoctors.com/teardowns/mercury-com), [Swipefile](https://swipefile.com/ai-powered-finance-orchestration-built-into-accounts), [UX Planet](https://uxplanet.org/captivating-design-of-the-mercury-fintech-app-d472bc0288bb).
- **Première impression** : photo d'ambiance pleine page, un champ « Enter your email » puis deux boutons, « Open account » et « Launch demo » (bench, n° 1).
- **Usabilité** : inscription en un champ, démo tôt dans la page, « Apply online in 10 minutes » ([mercury.com](https://mercury.com/), vu le 2026-11-13).
- **Hiérarchie** : une action principale, mais un second bouton qui lui fait concurrence. La mention « Mercury is a fintech company, not an FDIC-insured bank » reste épinglée en bas du hero.
- **Accessibilité** : bouton `#5266EB` à texte blanc, à 4,71:1. En mobile, champ de 38 px et boutons de 40 px, sous 44 px, et pas de label visible (mesuré dans le bench).
- **Ce qui marche** : le champ e-mail dans le hero, qui correspond exactement à la consigne mobile de Liasse, et la mention « pas une banque ».
- **Recommandations** (à transposer, pas à copier) : 1) garder le champ unique, sur fond clair et chaud, avec un seul bouton et un label visible ; 2) remplacer la photo d'ambiance par des captures d'usage artisan.

---

## 3. Thèmes clés

### Thème 1 : la réforme comme accroche
- **Prévalence** : 4 sites sur 6 (Pennylane, Abby d'après la presse, Indy, Qonto).
- **Observations** : échéancier daté (Pennylane), « Conforme à la réforme de la facturation électronique » (Indy), « Facturation électronique » dans le titre du hero (Qonto).
- **Interprétation** : l'accroche est saturée et vieillit vite. Une fois septembre 2026 passé, le message utile devient « préparez l'émission de 2027 ».

### Thème 2 : le gratuit comme norme
- **Prévalence** : 2 sites sur 6 mettent en avant une offre gratuite (Abby, Indy). Hors panel, Tiime aussi.
- **Interprétation** : Liasse ne peut pas se battre sur le prix de la conformité. Il faut vendre une valeur au-delà (trésorerie, relances) et un essai de 30 jours clair.

### Thème 3 : des chiffres incohérents
- **Prévalence** : 3 sites sur 6 (Indy pour le prix, Pennylane pour les dates, Qonto pour le nombre de clients).
- **Interprétation** : dans un secteur qui vend la conformité, l'incohérence coûte cher en confiance. Être cohérent est une différenciation à coût nul.

### Thème 4 : l'expert-comptable comme prescripteur
- **Prévalence** : 3 sites sur 6 ont un parcours dédié (Pennylane, Qonto, Indy avec l'expert-comptable en option).
- **Interprétation** : la section « Pour les experts-comptables » du README est justifiée. Elle doit contenir des bénéfices concrets, pas un simple logo.

### Thème 5 : la trésorerie, peu présente chez les acteurs TPE
- **Prévalence** : 1 site sur 6 en fait le cœur (Agicap, qui vise les PME et ETI).
- **Interprétation** : c'est l'espace libre pour Liasse, la trésorerie expliquée simplement à un artisan.

### Thème 6 : des artisans peu adressés
- **Prévalence** : 1 site sur 6 a une page artisans dédiée (Indy).
- **Interprétation** : le vocabulaire de chantier (devis, acompte, situation de travaux) est une opportunité.

---

## 4. Insights et opportunités

| Insight | Opportunité | Impact | Effort |
|---|---|---|---|
| L'accroche « réforme 2026 » est saturée et datée | Hero recalé : « émettez sereinement avant septembre 2027 » et échéancier personnalisé par statut | H | B |
| La conformité est gratuite chez plusieurs acteurs | Vendre la trésorerie à 90 jours et les relances automatiques | H | M |
| Les artisans sont peu adressés | Vocabulaire de chantier, captures mobiles de devis et d'acompte | H | M |
| Les chiffres sont incohérents chez les concurrents | Une seule source de chiffres, datée, réutilisée partout | M | B |
| L'expert-comptable prescrit | Section dédiée : invitation des clients, export, contact partenaire | M | M |
| Mercury met un champ e-mail unique dans le hero | Inscription en un champ, en desktop comme en mobile | M | B |
| Aucun site vu n'affiche de numéro d'immatriculation de plateforme agréée (Qonto, Pennylane) | Expliquer ce que veut dire « plateforme agréée » et renvoyer vers la liste officielle. Liasse, fictive, n'affiche aucun numéro | M | B |
| Les montants sont statiques sur les sites vus | Micro-animation des montants (facture payée, trésorerie qui remonte) | M | M |

---

## 5. Conventions et erreurs à éviter

**Conventions** : badge « Plateforme agréée », gratuit ou essai gratuit, téléphone et tableau de bord en perspective, frise de la réforme, notes et nombre d'utilisateurs, pages par statut, espace experts-comptables, FAQ réforme longue.

**Erreurs à éviter** :
- Faire peur avec la réforme (amendes en rouge, compte à rebours).
- Afficher « Plateforme agréée » ou « PDP » sans immatriculation réelle. Le terme officiel est désormais « plateforme agréée » (PA).
- Laisser des dates ou des chiffres contradictoires d'une page à l'autre.
- Afficher un prix d'appel qui n'inclut pas l'essentiel.
- Montrer un tableau de bord de DAF à un artisan.
- Demander plus d'un champ à l'inscription.
- Publier des avis sans indiquer s'ils sont contrôlés et comment (Code de la consommation), ou des avis inventés.

---

## 6. Conclusion appliquée à Liasse (fictif)

- **Recaler le hero** : « Vos factures conformes 2026 » est dépassé. Titre retenu : « Vos factures électroniques, faites depuis votre téléphone », avec en sous-titre « Recevez dès aujourd'hui, émettez sereinement avant septembre 2027 ». Aucune durée promise.
- **Différenciateur** : la trésorerie à 90 jours (courbe, montants tabulaires animés) et la relance automatique.
- **Artisans d'abord** : vocabulaire de chantier, captures mobiles en premier, inscription en un champ.
- **Experts-comptables** : une section concrète.
- **Confiance vérifiable** : renvoi vers la liste officielle des plateformes agréées, région d'hébergement et chiffrement écrits, dates sourcées, aucun avis inventé.
- **Forme** : crème, violet profond, accent corail, grotesque arrondie.

---

## 7. Questions pour la recherche utilisateur

1. En novembre 2026, les artisans savent-ils qu'ils doivent déjà pouvoir recevoir des e-factures, et qu'ils devront émettre en septembre 2027 ?
2. Qu'est-ce qui les fait passer à l'acte : la peur de la non-conformité, être payé plus vite, ou la visibilité sur leur trésorerie ?
3. « Trésorerie à 90 jours » est-il compris, ou faut-il dire « votre compte dans 3 mois » ?
4. Un essai de 30 jours face à des concurrents gratuits : quel argument justifie de payer ensuite ?
5. Quel rôle joue l'expert-comptable dans le choix de l'outil, et l'artisan suit-il sa recommandation ?
6. Les avis clients et la mention « plateforme agréée » sont-ils regardés, ou le bouche-à-oreille suffit-il ?

## 8. Notes de méthode

- **Sources** : recherches web de novembre 2026. Presse (Moneyvox, FrenchWeb, Le Journal des entreprises), pages des éditeurs, analyses de landing pages (SaaS Landing Page, Landing Doctors, Swipefile, UX Planet). Chaque chiffre de marché a été rouvert sur sa source le 2026-11-13 ; ceux qui n'ont pas pu l'être ont été retirés.
- **Vérification** : Pennylane, Indy, Qonto et Mercury ont été ouverts avec un vrai navigateur le 2026-11-12 (captures et mesures dans le [bench](BENCH.md)). Agicap a été ouvert le 2026-11-13 pour le texte seulement.
- **Limites** :
  - Abby reste inaccessible (erreur 403) : sa fiche repose sur la presse (*[non vu]*).
  - L'accessibilité n'a été mesurée que sur les éléments cités dans le bench.
  - Une partie des informations vient des éditeurs eux-mêmes (nombre de clients, notes).
  - Le décompte de 118 solutions agréées date de janvier 2026 (Moneyvox). La liste officielle n'a pas été recomptée.
  - 6 sites : prévalences indicatives.
