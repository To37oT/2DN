---
layout: default
title: Auto layout
permalink: /figma-auto-layout/
published: true
date: 2026
---

# TP 4 — Auto layout

> Prérequis : avoir suivi le [TP 3 — Blocs de contenu]({{site.baseurl}}/figma-blocs-de-contenu/).
>
> Vous savez normalement :
> - Créer des formes et des blocs de texte
> - Utiliser le panneau **Layers** et comprendre l'imbrication
> - Créer et appliquer des styles de texte

## 1 — Nouveau document

✏ **Créer le fichier**

- Dans votre dossier `informatique`, créer un nouveau fichier Design nommé `tp03-nom-prenom`.
- Renommer la page en `auto-layout`.

► Ces manipulations ont été vues aux TP précédents : à vous de les retrouver.

## 2 — L'exemple du bouton

🔎 **Une taille qui s'adapte au contenu**

- La taille d'un bouton doit souvent **s'adapter à son contenu** : un bouton « GO ! » n'a pas besoin de la même largeur qu'un bouton « En savoir plus… ».
- Avec une largeur fixe, les boutons au texte court paraissent **trop larges**, et ceux au texte long débordent.
- L'**auto layout** permet au bloc de se redimensionner automatiquement quand son contenu change.

<img alt="Taille adaptée ou trop large" src="{{ site.baseurl }}/assets/img/figma-tp3-bouton.png" /><br>

## 3 — Créer un bloc adaptable

✏ **Ajouter un auto layout**

- Créer un bloc de texte avec un mot de votre choix.
- Le sélectionner, puis clic droit → **Add auto layout** (`Maj + A`).

<img alt="Add auto layout" src="{{ site.baseurl }}/assets/img/figma-tp3-add-auto-layout.png" /><br>

- Un bloc **Frame** s'est créé dans le panneau Layers : il **contient** votre calque de texte initial.

<img alt="Frame créée dans les calques" src="{{ site.baseurl }}/assets/img/figma-tp3-calque-frame.png" /><br>

► On retrouve ici l'**imbrication** vue au TP 1 : l'auto layout est une propriété de la frame parente, qui organise les éléments qu'elle contient.

- Sélectionner la **Frame** pour afficher, dans le panneau de droite, les options **Auto layout**.

## 4 — Le panneau "Auto layout"

🔎 **Lire le panneau**

<img alt="Panneau Auto layout" src="{{ site.baseurl }}/assets/img/figma-tp3-panneau.png" /><br>

- **Organisation des éléments** : sens de disposition (vertical, horizontal, en grille…).
- **Taille du bloc** (`W` / `H`) : la façon dont le bloc s'adapte (voir ci-dessous).
- **Alignement du contenu** et **espace entre les éléments** (*gap*), avec des paramètres avancés.
- **Padding** : la marge intérieure du bloc.
- **Clip content** : masque le contenu qui dépasse du bloc.
- L'icône en haut à droite permet de **supprimer l'auto layout** du bloc.

🔎 **Les options de taille**

Dans les options de taille du bloc (`W` et `H`), il est possible de définir :

- **Hug** : le bloc s'adapte à son contenu.
- **Fill** : le bloc remplit tout l'espace disponible dans son parent (uniquement si l'élément est lui-même dans un parent en auto layout).
- **Une taille fixe** : ⚠️ tout redimensionnement manuel passe le bloc en taille fixe et supprime les deux options précédentes.
- **Des valeurs minimum et/ou maximum** (largeur ou hauteur).

► **À retenir pour plus tard** : retenez bien les mots *padding*, *gap*, *min / max*. Vous les retrouverez quand vous créerez des pages web : l'auto layout reprend la logique de mise en page utilisée par les navigateurs.

## 5 — Un bouton qui s'adapte

✏ **Paramétrer le bloc**

- Mettre une **couleur de fond** sur la frame en auto layout qui contient le texte.
- Régler sa largeur sur **Hug**.
- Modifier le texte : la taille du bloc doit désormais **changer automatiquement**.

✏ **Pour aller plus loin**

- Changer les paddings : **20** en largeur (gauche et droite).
- Mettre une **largeur minimum de 80** (ou une autre valeur, suivant votre taille initiale).
- Dupliquer le bouton et reproduire l'exemple : `GO !`, `Soldes`, `En savoir plus…`.

► Testez un texte d'une seule lettre : la largeur minimum évite d'obtenir un bouton presque carré.

## Rendu

- Renommer et organiser tous vos calques (`btn-go`, `btn-soldes`…).
- Créer un point d'historique `rendu-tp03` (`Ctrl`/`Cmd` + `Alt` + `S`).
- Partager le fichier en édition (*Share → Share settings → Anyone → Edit → Save*) et déposer le lien sur itslearning.

