*Projet YDays · Rythme B · Tristan Gerber (porteur), Jérémy et Paul · mis à jour le 18 novembre 2026*

# Sillage

> Sillage est un SaaS qui aide les entreprises à comprendre leur site web. Une IA analyse les pages et les données Google pour proposer des améliorations SEO, et un tracking anonyme suit le parcours des visiteurs jusqu’à leur demande de contact.

1. [Le problème et la solution](#1-le-problème-et-la-solution)
2. [Objectifs](#2-objectifs)
3. [Comment ça marche](#3-comment-ça-marche)
4. [Cible et segmentation](#4-cible-et-segmentation)
5. [Concurrence](#5-concurrence)
6. [Modèle économique](#6-modèle-économique)
7. [Budget et acquisition client](#7-budget-et-acquisition-client)
8. [Leviers forts](#8-leviers-forts)
9. [Équipe et rôles](#9-équipe-et-rôles)
10. [Planning des 11 séances](#10-planning-des-11-séances)
11. [Feuille de route](#11-feuille-de-route)
12. [Risques et points ouverts](#12-risques-et-points-ouverts)

---

## 1. Le problème et la solution

**Le problème.** Une entreprise dont une demande de contact vaut cher (une agence immobilière, un artisan haut de gamme, un cabinet) ne sait pas d’où viennent ses demandes ni ce qu’elles deviennent. Elle paie des portails, des annuaires ou une agence SEO (souvent 800 à 2 000 € HT par mois pour une PME) sans savoir ce qui lui rapporte des clients.

**La solution.** L’entreprise connecte son site, et Sillage travaille pour elle en continu :

- **Il suit chaque visiteur, de façon anonyme :** d’où il vient (Google, réseaux sociaux, recommandation, QR code, IA), ce qu’il fait (pages vues, parcours, formulaires abandonnés) et ce que ça donne, jusqu’à la demande de contact et à l’affaire signée.
- **Il améliore le site chaque mois :** son IA croise les pages avec Google Search Console, Bing et la vitesse réelle du site, puis prépare des améliorations concrètes (corrections techniques, titres et descriptions Google, liens entre les pages, FAQ tirées des vraies questions des clients, nouveaux contenus). Une personne valide avant publication.
- **Il montre les résultats :** un tableau de bord et un rapport mensuel avec les demandes par source, les actions livrées et l’évolution de la visibilité.

---

## 2. Objectifs

Deux objectifs, dans cet ordre :

1. **Analyser les leads.** Savoir, pour chaque demande, d’où elle vient et ce qu’elle devient (qualifiée, rendez-vous, affaire signée, perdue).
2. **Développer les leads.** S’appuyer sur cette analyse pour en obtenir plus : améliorations SEO préparées par l’IA, pages qui convertissent mieux, budget déplacé vers les sources qui rapportent.

Concrètement, pour le projet YDays :

- comprendre les visiteurs ;
- automatiser les optimisations SEO et techniques avec l’IA ;
- suivre le tunnel de conversion jusqu’à l’action (prise de contact, vente).

**Livrables attendus :** un dashboard KPI et une démo visuelle, sur le site de D&P.

**Ce qu’on mesure chez D&P :** la part des demandes qui ont une source (objectif : 100 %), le délai entre la demande et le premier contact, les demandes et affaires par source, les indicateurs SEO (pages indexées, impressions, recherches de la marque), et le coût réel par mois (IA et temps de validation).

---

## 3. Comment ça marche

Une boucle mensuelle en quatre étapes :

| Étape | Ce que fait Sillage |
| --- | --- |
| **Mesurer** | Enregistre chaque demande avec sa source et suit ce qu’elle devient. Compte les visites de façon anonyme, sans cookie. |
| **Analyser** | Croise les pages du site avec Search Console, Bing et la vitesse réelle du site. |
| **Agir** | L’IA prépare des améliorations en brouillon ; une personne les valide avant publication. |
| **Prouver** | Le rapport du mois montre les demandes et affaires par source, les actions livrées et l’évolution de la visibilité. |

↻ Le mois suivant, on mesure l’effet des actions publiées.

**Validation humaine.** Google accepte le contenu produit avec l’IA, mais demande une vérification humaine avant publication et sanctionne les contenus en masse. Chaque proposition de Sillage est donc validée par une personne, et cette validation est tracée.

**Statistiques anonymes.** Par défaut, Sillage mesure sans cookie et sans donnée personnelle, dans le cadre de l’exemption de consentement de la CNIL. Le suivi complet d’un visiteur sur plusieurs visites n’est activé qu’avec son accord. L’IA ne reçoit jamais de donnée personnelle.

**Technique.** Next.js et Payload pour le site et l’administration, MongoDB, l’API Claude pour l’analyse, les API gratuites de Google et Bing pour les données. En V1, Sillage est branché sur le site de D&P (sous Payload) ; en V2, un simple script permettra de le brancher sur n’importe quel site.

---

## 4. Cible et segmentation

### Cible de test : les agences immobilières

On teste sur l’immobilier parce qu’un client, **D&P (Dwell & Prestige)**, est prêt à intégrer l’outil : son site est en production et l’équipe en maîtrise le code. C’est aussi un bon secteur pour prouver la valeur de Sillage :

- **une demande vaut cher :** un mandat vendeur rapporte environ 10 000 à 15 000 € d’honoraires (estimation) ;
- **le parcours se mesure :** demande → estimation → mandat → vente, avec des dates et des montants.

### Local ou national ?

**On vend partout en France, on optimise en local.** La vente, l’installation et le suivi se font à distance. Mais le SEO de chaque agence reste local : sa ville, ses quartiers, sa fiche Google, ses biens. La prospection peut partir d’une région test avant de couvrir toute la France.

### Segments dans l’immobilier

| Segment | Besoin principal | Priorité |
| --- | --- | --- |
| **Agences haut de gamme et internationales** (type D&P) | Clientèle étrangère, recommandations, plusieurs langues | 1 · client test |
| **Agences indépendantes** (1 à 3 agences) | Mandats vendeurs, visibilité locale face aux portails | 1 · décision rapide du gérant |
| **Agences franchisées** (Orpi, Century 21, Laforêt…) | Se démarquer des autres agences du réseau | 2 · site imposé par le réseau |
| **Sièges de réseaux nationaux** | Piloter des centaines d’agences | Plus tard, avec des résultats chiffrés |

### Ensuite : une cible plus large (V2)

Une fois le cas D&P chiffré, Sillage s’ouvre à toutes les entreprises dont une demande de contact vaut cher et se transforme en affaire plus tard : rénovation et artisans haut de gamme, services premium, services B2B (cabinets de conseil, ESN, organismes de formation). Le point commun : le parcours demande → devis ou rendez-vous → affaire signée.

---

## 5. Concurrence

| Outil | Ce qu’il fait | Prix | Ce qui lui manque |
| --- | --- | ---: | --- |
| **DataFast** | Relie les ventes en ligne à leur source | 9–19 $/mois | Ne suit pas une demande de contact jusqu’à l’affaire |
| **WhatConverts, CallRail** | Suivent formulaires et appels | 30–195 $/mois | Pas d’amélioration du site, pas de suivi jusqu’à l’affaire |
| **Ruler Analytics** | Relie les demandes au chiffre d’affaires | 309–1 739 €/mois | Cher, sans SEO |
| **Agence SEO** | Fait le travail SEO à la main | 800–2 000 €/mois | Peu de preuves sur les demandes réellement obtenues |

**Notre différence :** Sillage réunit les deux. Il améliore le site comme une agence SEO, et il prouve chaque mois combien de demandes et d’affaires chaque source a rapportées.

---

## 6. Modèle économique

Abonnement mensuel, en trois paliers :

| Palier | Prix | Contenu |
| --- | ---: | --- |
| **Mesurer** | 490 € HT/mois | Suivi des demandes et alertes, statistiques anonymes, audit technique mensuel, rapport d’une page |
| **Croissance** | 890 € HT/mois | Tout Mesurer, analyse IA avec Search Console, 2 contenus validés par mois, suivi jusqu’à l’affaire signée, appel mensuel |
| **Premium** | 1 500 € HT/mois | Tout Croissance, site en plusieurs langues, 4 contenus par mois, SEO local sur plusieurs villes, revue trimestrielle |

Engagement de 6 mois, puis mensuel. La création d’un site est proposée en option. Les garanties portent sur les livrables (correctifs, contenus, date du rapport), jamais sur les positions Google. Prix à tester pendant les pilotes.

---

## 7. Budget et acquisition client

### Budget du projet

**Budget estimé : environ 150 à 350 € sur la durée des YDays, hors relecture juridique (estimation).**

| Poste | Estimation | Justification |
| --- | --- | --- |
| API Claude | 20 à 50 €/mois | Une analyse ciblée coûte environ 3 à 4 $, un audit complet 9 à 15 $ |
| Hébergement | 0 € | Le serveur de D&P, déjà payé, accueille le pilote |
| Nom de domaine | 10 à 20 €/an | Pour le site de Sillage |
| API Google et Bing | 0 € | Gratuites |
| Outils (GitHub, Figma, e-mails) | 0 € | Offres gratuites ou étudiantes |
| Relecture juridique RGPD | Devis à demander | À faire avant de vendre la promesse « sans bannière de cookies » |

Le vrai coût est le temps de l’équipe, et, une fois en service, le temps de validation humaine par client.

### Coût par client

L’IA coûte 5 à 15 $ par client et par mois, soit moins de 4 % de l’abonnement le moins cher. La marge dépend surtout du temps passé à valider les propositions : c’est l’indicateur à mesurer pendant le pilote.

### Comment trouver des clients

| Canal | Coût | Rôle |
| --- | --- | --- |
| **Cas D&P chiffré** | 0 € | La preuve sur laquelle repose tout le reste |
| **Audit gratuit du site** | 3 à 15 $ par audit | On montre un problème réel avant de vendre |
| **Prospection directe** (LinkedIn, e-mail, téléphone) | Temps | Premier canal, auprès des gérants d’agences d’une région test |
| **SEO de Sillage lui-même** | Temps | On applique le produit à notre propre site |
| **Salons de l’immobilier** | Entrée visiteur | Rencontrer des gérants d’agences |

**Règle :** un client doit coûter moins de 3 mois de son abonnement à acquérir, soit environ 1 500 € au palier Mesurer. Pas de publicité payante avant d’avoir mesuré ce coût sur les premiers clients.

### Ce que Sillage optimise pour ses clients

Une agence paie déjà pour trouver des clients : portails, annuaires, publicité. Le rapport Sillage lui montre, pour chaque source, les demandes et les affaires obtenues, et leur valeur. Elle peut alors déplacer son budget vers ce qui marche. C’est le service d’optimisation de l’acquisition, et c’est ce qui justifie le prix face à un simple outil de statistiques.

---

## 8. Leviers forts

1. **Le seul outil qui suit une demande jusqu’à l’affaire signée.** Les autres comptent des pages vues ou des formulaires.
2. **Un client prêt dès le départ.** D&P intègre l’outil, sur un site que l’équipe connaît déjà.
3. **L’IA fait le travail, une personne valide.** Conforme aux règles de Google, pour moins de 4 % du prix de l’abonnement.
4. **Des statistiques anonymes par défaut.** Pas de bannière de cookies au niveau de base, aucune donnée personnelle envoyée à l’IA.
5. **Un marché national, un SEO local.** Vente à distance dans toute la France, optimisation ville par ville.
6. **Un abonnement simple.** Des livrables chiffrés et un rapport chaque mois.
7. **Une feuille de route claire.** Cible plus large en V2, réseaux sociaux en V3.

---

## 9. Équipe et rôles

Trois développeurs, Tristan Gerber (porteur de projet), Jérémy et Paul, qui travaillent en parallèle sur l’ensemble du projet.

**Organisation :** une revue de 30 minutes chaque semaine, un tableau de tâches partagé, et chaque fonctionnalité relue par un autre développeur avant d’être intégrée.

---

## 10. Planning des 11 séances

| Séance | Objectif | Travail de l’équipe | Sortie |
| --- | --- | --- | --- |
| **1** | Étude de marché et business model | Cible, prix, budget ; analyse du site D&P, des outils IA et des API | Ce dossier |
| **2** | Spécifications fonctionnelles et techniques | Parcours utilisateur, contenu du rapport, modèle de données des demandes, specs du tracking et du moteur IA | Specs validées |
| **3** | Charte graphique et maquettes de l’interface | Maquettes du tableau de bord et du rapport ; préparation du site D&P (correctifs SEO, cookies, alertes) ; accès Search Console et Bing | Maquettes ; D&P prêt à mesurer |
| **4** | Moteur IA et tracking anonyme (phase 1) | Squelette du tableau de bord, enregistrement des demandes et alertes, extraction des données Google | Toutes les demandes D&P enregistrées |
| **5** | Moteur IA et tracking anonyme (phase 2) | Vue des demandes et du tunnel, tracking anonyme avec la source de chaque formulaire, première analyse IA automatique | Sources visibles ; coût d’une analyse mesuré |
| **6** | Moteur IA et tracking anonyme (finalisation) | Liens et QR codes de recommandation, clics téléphone et WhatsApp, propositions en brouillon et validation | Boucle complète de bout en bout |
| **7** | Tableau de bord utilisateur | Vues KPI, données des demandes et indicateurs SEO dans le tableau de bord | **Livrable : dashboard KPI** |
| **8** | Rapports mensuels automatisés | Mise en page du rapport, demandes et affaires par source, actions livrées | Premier rapport envoyé à D&P |
| **9** | Tests et debug | Tests avec D&P, tests RGPD et de charge, tests du moteur IA et mesure des coûts | Bugs corrigés |
| **10** | Démo visuelle et pitch deck | Pitch deck, démo en direct sur D&P, chiffres de la démo | **Livrable : démo visuelle** |
| **11** | Bilan et présentation finale | Bilan technique et des coûts, présentation | Présentation finale |

---

## 11. Feuille de route

| Version | Contenu |
| --- | --- |
| **V1 (YDays)** | Suivi des demandes, tracking anonyme, analyse IA mensuelle, tableau de bord et rapport, chez D&P |
| **V2** | Script pour brancher Sillage sur n’importe quel site ; ouverture à une cible plus large que l’immobilier |
| **V3** | Analyse des réseaux sociaux, pour toucher une cible plus communautaire |

Après les YDays : 3 à 5 entretiens avec des gérants d’agences, puis 2 ou 3 pilotes payants.

---

## 12. Risques et points ouverts

| Risque | Réponse |
| --- | --- |
| **RGPD :** la mesure sans bannière doit rester dans le cadre de l’exemption CNIL | Relecture par un juriste avant de vendre |
| **Temps de validation humaine** trop élevé par client | Mesuré pendant le pilote D&P ; il fixe la marge |
| **Sites des agences** souvent fournis par leur logiciel métier, difficiles à équiper | Script prévu en V2 ; à tester sur 2 ou 3 sites |
| **Prix** non confirmés | Testés pendant les pilotes |
| **Peu de trafic** chez D&P | Le rapport liste les demandes une par une plutôt que des pourcentages |

---

*La recherche complète (analyse des outils, architecture technique, RGPD détaillé, sources) est dans [annexe-recherche-sillage.md](annexe-recherche-sillage.md).*
