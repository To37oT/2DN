---
layout: default
title: Composants et variantes
permalink: /figma-composants/
published: true
date: 2026
---

# TP 5 — Composants et variantes

> Prérequis : avoir suivi le [TP 4 — Auto layout]({{site.baseurl}}/figma-auto-layout/).
>
> Vous savez normalement :
> - Créer des masques et des formes personnalisées
> - Ajouter un auto layout à un bloc
> - Régler la taille d'un bloc en **Hug**, **Fill** ou taille fixe
> - Régler les paddings d'un bloc

## 1 — Nouveau document

✏ **Créer le fichier**

- Dans votre dossier `informatique`, créer un nouveau fichier Design nommé `tp05-nom-prenom`.
- Créer deux pages : `composants` et `maquette`.

► Ces manipulations ont été vues aux TP précédents : à vous de les retrouver.

## 2 — Les composants

🔎 **Définition**

- Un **composant** (*component*) est un élément graphique **réutilisable**, composé d'un ou plusieurs éléments.
- Il y a toujours un **composant maître** (*main component*) et ses **instances** (les copies).

<img alt="Composant maître et instances" src="{{ site.baseurl }}/assets/img/figma-tp4-definition.png" /><br>

🔎 **Création**

- On organise ses composants maîtres sur une **page dédiée**.
- Créer un élément, le sélectionner, puis cliquer sur l'icône **Create component** dans la barre d'outils (4 losanges), ou passer par le clic droit (`Ctrl`/`Cmd` + `Alt` + `K`).
- Dans le panneau Layers, l'icône du calque devient **violette** : c'est désormais un composant.

<img alt="Créer un composant" src="{{ site.baseurl }}/assets/img/figma-tp4-creation.png" /><br>

🔎 **Utilisation**

- L'onglet **Assets** (panneau de gauche) donne accès à tous les composants créés : il suffit de les cliquer-glisser sur le canvas pour créer une **instance**.
- Les modifications du **composant maître** s'appliquent à **toutes** les instances.
- Les modifications faites sur **une instance** ne s'appliquent qu'à **celle-ci**.
- Il est possible de choisir un **état** pour ce composant : une **variante** (voir plus bas).

<img alt="Panneau Assets" src="{{ site.baseurl }}/assets/img/figma-tp4-assets.png" /><br>

► On retrouve la logique des **styles de texte** du TP 2 : une seule source, mise à jour partout.

## 3 — Créer un bouton composant

✏ **Analyser le composant**

Le composant suivant est composé de :
- **2 rectangles** inclinés à **45°**
- **1 texte**, avec son bloc en **auto layout** (**Hug**)

<img alt="Composant bouton" src="{{ site.baseurl }}/assets/img/figma-tp4-bouton.png" /><br>

✏ **Le reproduire**

- Retrouver les paramètres permettant de créer ce bouton (padding, masque…) et le transformer en composant nommé `bouton`, sur la page `composants`.
- Ajouter des **instances** du composant sur la page `maquette` (image ci-dessous).
- Dans cet exercice, **UNIQUEMENT le texte** doit être modifié dans les instances.

<img alt="Instances du composant" src="{{ site.baseurl }}/assets/img/figma-tp4-instances.png" /><br>

► Observez la structure dans le panneau Layers : le masque, les rectangles et la frame en auto layout sont **imbriqués** dans le composant. Si le bouton s'élargit avec le texte, les rayures doivent rester en place.

## 4 — Les variantes

🔎 **Définition**

- Un même composant peut parfois prendre **plusieurs affichages différents** (normal, survolé, désactivé…) : cela peut être ajouté dans le composant en tant que **paramètre**.
- Modifications possibles dans une variante : texte, couleur, taille, forme, effets…

🔎 **Créer une variante**

- Créer et sélectionner un composant.
- Cliquer sur l'icône **Add variant** (losange avec un `+`).
- Changer le design de la nouvelle variante.
- Bien **renommer** la propriété et les variantes pour faciliter l'organisation.

<img alt="Créer une variante" src="{{ site.baseurl }}/assets/img/figma-tp4-variante-creation.png" /><br>

## 5 — Organiser ses variantes

🔎 **Propriétés et valeurs**

- Sur chaque **composant**, vous pouvez définir des **propriétés**.
- Sur chaque **variante**, vous pouvez choisir la **valeur** de ces propriétés.
- Par défaut, les noms ne sont pas optimisés (`Property 1`, `Default`, `Variant2`, `Variant3`…).

<img alt="Propriétés par défaut" src="{{ site.baseurl }}/assets/img/figma-tp4-proprietes.png" /><br>

- Lorsque l'on sélectionne le composant (l'ensemble des variantes), on obtient ceci :

<img alt="Propriétés du composant" src="{{ site.baseurl }}/assets/img/figma-tp4-composant-selectionne.png" /><br>

✏ **Renommer les propriétés**

- Cliquer sur le bouton **réglage** à côté de la propriété pour la renommer, ainsi que ses valeurs.
- Exemple : la propriété `Etat`, avec les valeurs `normal`, `actif` et `non actif`.

<img alt="Renommer la propriété" src="{{ site.baseurl }}/assets/img/figma-tp4-renommer.png" /><br>

🔎 **Choisir la variante d'une instance**

- Sur vos instances de composant, vous pouvez choisir la **variante utilisée** dans le panneau de droite.

<img alt="Choisir la variante" src="{{ site.baseurl }}/assets/img/figma-tp4-choix-variante.png" /><br>

## 6 — Un exemple complet

🔎 **Un bouton à 110 variantes**

- Cet exemple utilise aussi des **variables** (vues plus tard).
- Le lien vers le fichier Figma est normalement accessible sur l'ENT.
- Il permet de créer **un seul composant bouton** et de choisir plus facilement son design ensuite : taille, couleur, style, interaction, icône, texte…

<img alt="Bouton à 110 variantes" src="{{ site.baseurl }}/assets/img/figma-tp4-110-variantes.png" /><br>

► Une bibliothèque de composants bien construite, c'est le cœur d'un **design system**.

## 7 — Exercice

✏ **Créer un composant avec variantes**

- À l'aide des explications précédentes, transformer votre composant `bouton` en un bouton à **3 variantes** : `normal`, `actif`, `non actif`.
- Renommer la propriété (`Etat`) et ses valeurs.
- Sur la page `maquette`, utiliser au moins une instance de chaque variante.

<img alt="Bouton à 3 variantes" src="{{ site.baseurl }}/assets/img/figma-tp4-exercice-variantes.png" /><br>

## Rendu

- Renommer et organiser tous vos calques, composants et variantes.
- Créer un point d'historique `rendu-tp04` (`Ctrl`/`Cmd` + `Alt` + `S`).
- Partager le fichier en édition (*Share → Share settings → Anyone → Edit → Save*) et déposer le lien sur itslearning.

