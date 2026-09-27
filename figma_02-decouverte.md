---
layout: default
title: Découverte de l'interface
permalink: /figma-decouverte/
published: true
date: 2026
---

# TP 1 — Prise en main de Figma

> Prérequis : avoir un compte Figma (idéalement Éducation validé) — voir [Introduction à Figma]({{site.baseurl}}/figma-introduction/).

## 1 — Premier projet

✏ **01 — Créer une nouvelle équipe** (Dnmade)<br>
<img alt="Nouvelle équipe" src="{{ site.baseurl }}/assets/img/figma-tp1-equipe.png" />

✏ **02 — Renommer le dossier par défaut** (`informatique`)<br>
<img alt="Renommer dossier" src="{{ site.baseurl }}/assets/img/figma-tp1-dossier.png" />

✏ **03 — Créer un fichier "Design"** et le nommer immédiatement : `tp01-nom-prenom`<br>
<img alt="Design file" src="{{ site.baseurl }}/assets/img/figma-tp1-design.png" />

## 2 — Interface "Design"
<br>
<img alt="Interface  figma" src="{{ site.baseurl }}/assets/img/figma-interface.png" />
<br>
🔎 **Le nommage, tout de suite**

► Il est important de nommer **rapidement** chaque nouvel élément, page, fichier…

- C'est une pratique qui devient très vite automatique et peu contraignante.
- Elle facilite la compréhension d'un projet et rend le designer plus efficace.
- Il est toujours plus rapide de nommer chaque élément **à sa création** que de tout renommer à la fin.

## 3 — Frames

🔎 **Qu'est-ce qu'une frame ?**

- Elle sert à définir la **zone visible** d'un design.
- Elle peut contenir d'autres éléments : texte, images, composants, etc.
- Format libre ou prédéfini (presets Desktop, Phone, Tablet…).
- Elle peut être redimensionnée à tout moment.

✏ **Créer une frame**

- Créer une frame au format **"Desktop"** (outil Frame : touche `F`, puis choisir le preset dans le panneau de droite).

## 4 — Taille de la frame

🔎 **Les tailles d'écran**

- Les tailles d'écran et de fenêtre sont une notion à prendre en compte dans vos créations.
- Elles évoluent avec l'époque et les technologies.
- Site de référence : [gs.statcounter.com](https://gs.statcounter.com/screen-resolution-stats/desktop/worldwide)
- Ce n'est **pas la résolution la plus utilisée** qu'il faut prendre comme référence, mais celle qui permet au plus grand nombre de personne **d’accéder à votre contenu** (cela vous amènera à choisir la plus petite taille en largeur parmi votre cible.
- Ne pas oublier l'impact de la **barre de scroll verticale**.
- Le **responsive** vous permettra d'avoir **des contenu flexibles** aux écrans.

✏ **Adapter la taille**

- Régler la **largeur de la frame à 1280** (panneau de droite, champ `W`).

## 5 — Couleurs et grilles

🔎 **Rappel sur les couleurs numériques**

► **RGB / RVB**
- Couleur composée de 3 valeurs : rouge, vert, bleu (entre 0 et 255).
  
► **Hex**
- Couleur RGB écrite au format hexadécimal (ex. `#CCCCCC`).

► **HSL et HSB**
- Couleur composée de 3 valeurs : teinte, saturation, luminosité.
- Nuance : le L de HSL (*Lightness*) et le B de HSB (*Brightness*) ne se calculent pas de la même façon — Figma propose les deux dans son sélecteur de couleur.

✏ **Arrière-plan de la frame**

- La propriété **"Fill"** permet de paramétrer l'arrière-plan.
- Mettre l'arrière-plan à `CCCCCC`.

🔎 **Grilles**

- Les grilles aident à **aligner** les éléments.
- Elles favorisent l'adaptation de la mise en page pour différents écrans.

✏ **Créer une grille**

- Sur la frame, ajouter un **Layout grid** : 12 colonnes, **centrée**, largeur de colonne **80**, gouttière **20**.

► **Selon vous, pourquoi n'utilise-t-on pas toute la largeur de la frame ?**

## 6 — Contenu et partage

🔎 **Créer / insérer du contenu**

- La barre d'outils permet d'ajouter différents types de contenu (formes, texte, images…) que vous pourrez aligner sur la grille précédemment créée.

🔎 **Partager son projet**

- Pendant ou à la fin d'un projet, vous aurez besoin de partager votre projet, cela se fait avec le lien "share", il faut bien paramétrer la gestion des droits de l'utilisateur (lecture ou édition).

- Pour un partage simple en édition (ce que vous aurez besoin de faire pour les rendus) :
  - Il faut choisir "Anyone" dans la liste déroulante des cibles
  - Choisir "Edit" dans ce qu'ils peuvent faire
  - Vous pouvez sécuriser avec un mot de passe si nécessaire (à transmettre avec les rendus dans ce cas)
  - Sauvegarder la configuration
  - Sur la fenêtre de partage, désormais le lien (accessible avec "Copy link") permettra d’accéder à votre projet et d'y faire des modifications.

<img alt="droits de partage" src="{{ site.baseurl }}/assets/img/figma-tp1-canedit.png"><br>
<img alt="Lien de partage" src="{{ site.baseurl }}/assets/img/figma-tp1-canedit-2.png"><br>

**N'hésitez pas à tester cette manipulation avec un camarade de confiance**

🔎 **Notification**

- Les notifications peuvent être subtiles si vous ne consultez pas régulièrement l'adresse mail reliée à votre compte. Pensez à regarder la cloche de notification si vous avez un point rouge.
(si vous oubliez de me donner le droit d'édition, c'est ici que vous aurez ma demande de droit).

<img alt="Notifications" src="{{ site.baseurl }}/assets/img/figma-tp1-notifications.png"><br>

## 7 — Organiser son contenu

🔎 **Layers**

Afin d'organiser votre projet, Figma possède 2 types d'organisation : les **layers** et les **pages**.

<img alt="Layers et pages" src="{{ site.baseurl }}/assets/img/figma-tp1-layers.png"><br>

L'organisation des layers fonctionne comme pour les calques, nous allons pouvoir imbriquer des éléments dans d'autres éléments et gérer leur ordre d'empilement : dans la liste, l'élément le plus haut recouvre les autres.

**L'imbrication est un concept essentiel à comprendre, cela permettra de fabriquer certains mécanismes et facilitera les modifications** 

🔎 **Pages**

Les pages permettent d'organiser le projet en sous-parties de manière très efficace. Chaque page est un nouvel espace de travail vide, mais les pages d'un même fichier partagent les composants, styles et variables. Le prototypage ne relie que les frames d'une même page.

*À noter pour plus tard : le prototypage (liens interactifs entre écrans) ne relie que les frames d'une même page.*

✏ Organiser ses pages
- Renommer la page actuelle en "maquette-desktop"
- Créer une seconde page "brouillon"

## 8 — Mini projet (45min)

Les valeurs demandées sont volontairement différentes de celles du TP : à vous de retrouver les manipulations et d'adapter les paramètres.

Afin d'appliquer les précédentes méthodes, vous allez réaliser un mini projet de page web dans Figma : 
- Une seule page d'accueil à réaliser : au minimum un bandeau avec un titre, une image, deux blocs de texte, un bouton — le tout aligné sur la grille, le thème est libre
- Format de la frame : 1200px × 800px
- Une grille (layout grid) de 16 colonnes, largeur 50px, centrée, gouttière 20px

<img alt="Frame de départ" src="{{ site.baseurl }}/assets/img/figma-tp1-projet-1.png"><br>

- Tentez de mettre des bords arrondis à la bannière (facultatif)
- Ce projet sera à partager en écriture via l'espace de rendu sur itslearning (transmettre le lien)
- Créer un point d'historique avant le rendu.



## Grille d'évaluation indicative

> Cette grille indicative expose les principaux critères évalués sur ce mini projet. D'autres éléments en lien avec les compétences travaillées en cours peuvent être pris en compte. Un entretien oral individuel peut, dans certains cas, compléter cette évaluation.

### C1.1 — Utiliser les outils numériques de référence
*(ici : les fonctions de base de Figma)*

| Niveau | Critères |
|---|---|
| **Très bonne maîtrise** | La page est réalisée avec les outils vus en cours (frame aux bonnes dimensions, grille conforme, contenus variés alignés sur la grille) et l'élève va au-delà de la simple réutilisation : mise en page personnelle, découverte d'outils non vus en cours. |
| **Maîtrise satisfaisante** | La page respecte les consignes techniques (frame, grille, contenu minimal) en réutilisant correctement les manipulations du TP. |
| **Maîtrise fragile** | Les consignes techniques sont partiellement respectées (grille absente ou mal paramétrée, dimensions incorrectes) ou le contenu est trop pauvre pour évaluer la maîtrise. |
| **Maîtrise insuffisante** | L'objectif n'est pas atteint : frame vide ou quasi vide, aucune consigne technique respectée. |

### C10.5 — Respect des échéances et contrôle du rendu

| Niveau | Critères |
|---|---|
| **Très bonne maîtrise** | Le lien est éditable et fonctionnel dès le premier essai, déposé au bon endroit sur itslearning, **AVANT** la date limite. |
| **Maîtrise satisfaisante** | Un critère non respecté (lien non éditable, mauvais emplacement…) mais corrigé après relance, dans les délais. |
| **Maîtrise fragile** | Rendu en retard (moins de 7 jours), **ou** lien éditable jamais transmis mais le projet visible témoigne d'un travail suffisant. |
| **Maîtrise insuffisante** | Retard de plus de 7 jours, **ou** lien éditable jamais transmis **et** projet trop simple : la quantité de travail visible ne permet pas une évaluation. |

### C11.5 — Organisation du projet

| Niveau | Critères |
|---|---|
| **Très bonne maîtrise** | Fichier, frame et calques nommés de façon pertinente et cohérente (conventions vues en cours) ; imbrication logique des éléments ; un point d'historique créé avant le rendu. |
| **Maîtrise satisfaisante** | L'organisation est globalement là, avec de petites erreurs : quelques noms par défaut type "Frame 12", imbrication approximative, ou point d'historique oublié. |
| **Maîtrise fragile** | Une démarche d'organisation est visible mais incomplète : nommage partiel ou incohérent et imbrication désordonnée. |
| **Maîtrise insuffisante** | Aucune démarche d'organisation : tout est laissé par défaut (noms automatiques, éléments en vrac). |

