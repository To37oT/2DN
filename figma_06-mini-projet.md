---
layout: default
title: Mini projet — L'appli du Repair Café
permalink: /figma-mini-projet/
published: true
date: 2026
---

# Mini projet — L'appli du Repair Café

> Prérequis : avoir suivi le [TP 4 — Composants et variantes]({{site.baseurl}}/figma-composants/).
>
> Vous savez normalement :
> - Créer et appliquer des styles de texte
> - Utiliser l'auto layout (**Hug**, **Fill**, padding, gap)
> - Créer des composants, des instances et des variantes

## Le sujet

🔎 **La demande**

- Un **Repair Café**, c'est un atelier gratuit où des bénévoles aident les habitants à **réparer leurs objets** (grille-pain, vélo, vêtement, lampe…) au lieu de les jeter.
- Le Repair Café de votre ville veut une **petite application mobile** pour annoncer ses **prochains ateliers** et permettre de **réserver une place**.
- Vous dessinez **l'écran d'accueil** de cette application.

🔎 **Ce que contient l'écran d'accueil**

- **En haut** : le nom du Repair Café et une phrase d'accroche.
- **Une phrase chiffrée**, par exemple « 1 240 objets sauvés de la poubelle cette année ».
- **3 ateliers à venir**, présentés l'un sous l'autre. Chaque atelier est présenté dans un **bloc atelier**, c'est-à-dire un rectangle qui regroupe :
  - une photo ;
  - la date et le lieu ;
  - le **type de réparation** écrit dans un petit rectangle coloré (`Vélo`, `Couture`, `Électroménager`…) : on l'appellera la **pastille** ;
  - un bouton `Réserver`.
- **En bas** : un **menu** avec 4 rubriques : `Accueil`, `Ateliers`, `Mes objets`, `Profil`.

🔎 **La règle du projet**

- Tout ce qui se répète (bouton, pastille, bloc atelier, menu) doit être un **composant**. L'écran est ensuite construit **uniquement avec des instances**.
- Votre fichier doit pouvoir être **repris par quelqu'un d'autre** : en dernière séance, un ou une camarade ajoutera un atelier sur votre écran, sans vous poser de question.

## Le calendrier

| Quand | Durée | Ce que vous faites |
|---|---|---|
| Vacances | 2 à 3 h maximum | Recherche graphique + photos + bouton |
| Séance 1 | 2 h | Les composants + leur mode d'emploi |
| Séance 2 | 2 h | L'écran + l'échange avec un camarade + le rendu |

## 1 — Pendant les vacances (2 à 3 h)

✏ **Créer le fichier**

- Dans votre dossier `informatique`, créer un fichier Design nommé `projet-repair-nom-prenom`.
- Créer quatre pages : `recherche`, `composants`, `mode-emploi`, `ecran`.

✏ **Page `recherche`**

- **3 à 5 images de référence** : applis, sites ou affiches dont l'ambiance vous semble juste pour un Repair Café.
- Une **palette de 3 à 5 couleurs**, chacune enregistrée comme **style de couleur**.
- **3 styles de texte** minimum (ex. `titre`, `sous-titre`, `texte`).
- Un **croquis** de votre écran d'accueil (photo d'un dessin papier acceptée).

✏ **Choisir les photos des ateliers**

- Trouver **4 photos** d'objets en réparation (sites libres de droits : Unsplash, Pexels…) ou les prendre vous-même.
- Les placer sur la page `recherche`.

► Choisissez des photos **de bonne qualité** : nettes, bien cadrées, assez grandes pour ne pas être pixelisées une fois placées dans l'écran.

✏ **Page `composants` : le bouton**

- Reprendre votre bouton du TP 4 et l'adapter à vos couleurs : propriété `Etat` avec `normal`, `actif`, `non actif`.

✏ **Point d'étape**

- Créer un point d'historique `vacances` (`Ctrl`/`Cmd` + `Alt` + `S`).

► Pas besoin d'aller plus loin : la suite se fait en cours.

## 2 — Séance 1 : les composants (2 h)

✏ **Créer 3 nouveaux composants**, sur la page `composants` :

- **La pastille** (`pastille`) : le type de réparation, dans un bloc en auto layout (**Hug**). Propriété `Type` avec au moins **3 valeurs** (`velo`, `couture`, `electromenager`…), chacune avec sa couleur.
- **Le bloc atelier** (`bloc-atelier`) : photo + date + lieu + une **instance** de la pastille + une **instance** du bouton. Auto layout vertical : si le lieu est écrit sur deux lignes, le bloc doit s'agrandir sans rien casser.
- **Le menu** (`menu`) : les 4 rubriques, avec une propriété `Actif` qui indique la rubrique sélectionnée.

► Testez chaque composant **avant** de passer au suivant : posez une instance, changez le texte (très court puis très long), changez la variante. Si quelque chose s'étire ou déborde, corrigez le composant maître.

✏ **Page `mode-emploi`**

Pour chaque composant, poser une instance et écrire à côté :
- son **nom** et **à quoi il sert** (une phrase) ;
- ses **propriétés** et leurs **valeurs** ;
- **ce qu'on peut modifier** dans une instance et **ce qu'on ne doit pas toucher**.

► Écrivez pour quelqu'un qui découvre votre fichier : en séance 2, c'est un ou une camarade qui lira cette page.

✏ **Point d'étape**

- Point d'historique `seance-1`.

## 3 — Séance 2 : l'écran et l'échange (2 h)

✏ **Construire l'écran d'accueil** (environ 50 min)

- Sur la page `ecran`, créer une frame **iPhone** (ou équivalent mobile).
- Construire l'écran avec des **instances** de vos composants et vos photos.
- Aucune instance ne doit être **détachée** (*Detach instance*).
- Point d'historique `ecran`.

✏ **Échange avec un camarade** (environ 30 min)

- Échanger votre lien avec votre voisin ou voisine.
- Dans le fichier de l'autre, ajouter un **4ᵉ atelier** sur son écran, avec sa 4ᵉ photo et un autre type de réparation, **en utilisant uniquement ses composants et sa page `mode-emploi`**, sans lui poser de question.
- Laisser ensuite **2 commentaires** Figma (touche `C`) : une chose **claire**, une chose qui vous a **fait hésiter**.

✏ **Corriger et finaliser** (environ 40 min)

- Corriger vos composants ou votre mode d'emploi si un commentaire le justifie, et répondre aux commentaires en une ligne.
- Vérifier que tout est rangé et renommé (voir Rendu).

## Rendu

- Calques, composants, propriétés et variantes **renommés** (pas de `Frame 12`, `Property 1`, `Variant2`…).
- Points d'historique : `vacances`, `seance-1`, `ecran`, `rendu-projet`.
- Partager le fichier en édition (*Share → Share settings → Anyone → Edit → Save*) et déposer le lien sur itslearning **avant la date indiquée**.

## Évaluation

Cette grille d'évaluation expose les principaux critères retenus. Certains éléments, bien que non mentionnés explicitement ici, peuvent être pris en compte s'ils sont en lien avec les compétences travaillées en cours. Un entretien oral individuel peut également, dans certains cas, compléter cette évaluation.

### C1.1 — Utiliser les outils numériques de référence

*Utiliser les outils numériques de référence et les règles de sécurité informatique pour acquérir, traiter, produire et diffuser de l'information ainsi que pour collaborer en interne et en externe.*

- **Très bonne maîtrise** : l'écran d'accueil est complet et Figma est utilisé de manière cohérente et pertinente (composants, variantes, auto layout, styles), avec des utilisations multiples et maîtrisées. L'élève exploite le potentiel de l'outil au-delà des exercices (variantes supplémentaires, propriétés bien pensées, idées personnelles). Les photos sont de très bonne qualité et bien intégrées.
- **Maîtrise satisfaisante** : l'écran d'accueil est complet et construit avec des instances. Les composants demandés existent, s'adaptent à leur contenu et leurs variantes fonctionnent. L'élève sait réexploiter les exercices (bouton du TP 4 adapté ou amélioré). Les photos sont nettes et bien cadrées.
- **Maîtrise fragile** : l'écran d'accueil est fait, mais l'outil ne semble pas parfaitement maîtrisé : instances détachées, composants qui s'étirent ou débordent, copie des exercices sans adaptation, photos floues, pixelisées ou déformées, ou pas assez de contenu pour évaluer sereinement.
- **Maîtrise insuffisante** : l'écran d'accueil n'est pas fait, ou peu de composants sont créés.

### C10.5 — Veiller au respect des échéances et au contrôle technique

*Veiller au respect des échéances et au contrôle technique et artistique selon les règles du métier.*

- **Très bonne maîtrise** :
  - le fichier s'ouvre et fonctionne correctement dès son lancement ;
  - le lien est éditable ;
  - le lien est déposé à l'endroit défini dans les consignes ;
  - le rendu est fait avant la date limite (le dernier jour n'est pas inclus).
- **Maîtrise satisfaisante** : un des critères précédents n'a pas été respecté, mais l'élève a su corriger son erreur après relance. Le projet reste transmis dans les délais.
- **Maîtrise fragile** : retard inférieur à 7 jours, ou lien éditable jamais transmis.
- **Maîtrise insuffisante** : rendu avec plus de 7 jours de retard, ou lien éditable jamais transmis et projet trop simple pour permettre une évaluation complète.

### C11.5 — Planifier et gérer les étapes d'un projet

*Planifier et gérer les différentes étapes d'un projet jusqu'à son rendu et sa validation en prenant en compte l'environnement de réalisation, de production et de diffusion et les pratiques de développement durable.*

Quatre critères sont observés :

1. **Les pages** : les 4 pages existent, chacune contient ce qui est attendu, et les points d'historique montrent que les étapes ont été suivies.
2. **L'organisation** : les éléments sont rangés clairement dans les pages (composants alignés et regroupés, rien qui traîne hors des frames).
3. **Les noms** : calques, composants, propriétés et variantes ont des noms pertinents et cohérents.
4. **La maintenabilité** : le fichier peut être repris par quelqu'un d'autre. Les bonnes pratiques sont respectées (styles de couleur et de texte appliqués, une seule source pour chaque composant), le mode d'emploi est clair et le camarade a pu ajouter son atelier.

- **Très bonne maîtrise** : les quatre critères sont respectés.
- **Maîtrise satisfaisante** : un des critères n'est pas respecté, ou il y a de petites erreurs dans plusieurs critères.
- **Maîtrise fragile** : deux critères ne sont pas respectés, ou il y a de petites erreurs dans tous les critères.
- **Maîtrise insuffisante** : trois critères ou plus ne sont pas respectés.
