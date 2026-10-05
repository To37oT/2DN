---
layout: default
title: Blocs de contenu
permalink: /figma-blocs-de-contenu/
published: true
date: 2026
---

# TP 3 — Blocs de contenu

> Prérequis : avoir suivi le [TP 2 — Prise en main de Figma]({{site.baseurl}}/figma-decouverte/).
>
> Vous savez normalement :
> - Créer une équipe, un dossier et un document
> - Repérer les différents panneaux principaux de Figma
> - Créer une frame et une grille
> - Partager votre document en édition

## 1 — Nouveau document

✏ **Créer le fichier**

- Dans votre dossier `informatique`, créer un nouveau fichier Design nommé `tp03-nom-prenom`.
- Créer une frame **Desktop 1280**, nommée `accueil`.
- Ajouter une grille : **12 colonnes, centrée, largeur 80, gouttière 20**.
- Renommer la page en `blocs-de-contenu`.

► Ces manipulations ont été vues au TP 1 : à vous de les retrouver.

## 2 — Créer des formes

🔎 **L'outil forme**

- L'outil forme regroupe plusieurs possibilités : rectangle (`R`), ligne (`L`), flèche (`Maj + L`), ellipse (`O`), polygone, étoile.
- Le petit chevron à côté de l'icône permet de changer de forme.
- Toute forme peut recevoir un **remplissage** (Fill), un **contour** (Stroke) et des **effets**.

<img alt="Outil forme" src="{{ site.baseurl }}/assets/img/figma-tp2-formes.png" /><br>

## 3 — Remplir une forme

🔎 **Les types de remplissage (Fill)**

Le panneau **Fill** ne se limite pas à la couleur unie. En cliquant sur la vignette de couleur, vous accédez à :

- **Solid** : couleur unie
- **Gradient** : dégradé (linéaire, radial, angulaire, en losange)
- **Image** : une image vient remplir la forme
- **Video** : une vidéo vient remplir la forme

► Pour une image ou une vidéo, le mode d'affichage (**Fill / Fit / Crop / Tile**) détermine le cadrage.

✏ **Quatre blocs de contenu**

- En vous appuyant sur la grille, créer **4 rectangles de 280 × 200**.
- Rectangle 1 : une **couleur unie**
- Rectangle 2 : <a href="{{ site.baseurl }}/assets/img/figma-tp2-image.jpg">l'**image fournie**</a>
- Rectangle 3 : <a href="{{ site.baseurl }}/assets/img/figma-tp2-video.mp4">la **vidéo fournie**
- Rectangle 4 : un **dégradé**s
- Renommer chaque calque dans le panneau **Layers** (`bloc-couleur`, `bloc-image`…).

<img alt="Quatre blocs de contenu" src="{{ site.baseurl }}/assets/img/figma-tp2-blocs.png" /><br>

## 4 — Le panneau "Layers"

🔎 **Lire le panneau**

- Le panneau **Layers** contient tous vos éléments, dans leur **ordre d'empilement** (le plus haut recouvre les autres).
- L'**icône** à gauche de chaque ligne indique le type de contenu : forme, image, vidéo, texte, frame, groupe…
- Deux icônes apparaissent au survol, à droite :
  - 🔒 **Lock** : verrouille l'élément (il ne peut plus être sélectionné par erreur sur le canvas)
  - 👁 **Hide** : masque l'élément sans le supprimer
- Le triangle à gauche d'une frame ou d'un groupe permet de **déplier son contenu** : c'est ainsi que l'on visualise l'**imbrication**.

<img alt="Panneau Layers" src="{{ site.baseurl }}/assets/img/figma-tp2-layers.png" /><br>

► **Astuce** : `Ctrl + G`/`Cmd + G` permet de grouper plusieurs éléments sélectionnés.<br>
► **Astuce** : maintenir `Ctrl`/`Cmd` en cliquant sur le canvas permet de sélectionner directement un élément imbriqué, sans dérouler le panneau.

## 5 — Le texte

🔎 **L'outil texte**

- Outil texte : touche `T`.
- Deux façons de créer un bloc : **cliquer** (le bloc s'adapte au texte) ou **dessiner une zone** (le texte se répartit dans la zone définie).
- Le panneau **Typography** permet de régler police, graisse, taille, interlignage, interlettrage et alignement.
- **Vertical trim** supprime l'espace vertical superflu au-dessus et en dessous du texte : très utile pour aligner précisément un titre.

<img alt="Panneau Layers" src="{{ site.baseurl }}/assets/img/figma-tp2-texte.png" /><br>

🔎 **Les styles de texte**

- Un **style** enregistre un réglage typographique pour le réutiliser partout.
- Intérêt : modifier le style met à jour **tous** les textes qui l'utilisent — indispensable dès qu'un projet grandit.
- C'est l'ancêtre direct des **variables** et des classes CSS que vous écrirez plus tard.

✏ **Créer et appliquer des styles de texte**
 
- Créer trois blocs de texte : un **titre**, un **sous-titre**, un **paragraphe**, avec des réglages typographiques différents.
- Pour chacun : le sélectionner, puis dans le panneau **Typography**, cliquer sur l'icône **styles** (les quatre points) → **`+`** → nommer le style (`titre`, `sous-titre`, `corps`).
- Dupliquer les trois blocs **quatre fois** sur la frame.
- Modifier maintenant le style `titre` (taille ou couleur) depuis le panneau des styles : **tous** les titres se mettent à jour d'un coup.

► Imaginez la même modification à faire à la main sur un site de 20 pages : c'est tout l'intérêt des styles.

## 6 — Plugins et faux texte

🔎 **Les plugins**

- Les **plugins** sont des outils complémentaires, proposés par Figma et par la communauté.
- Accès : barre d'outils → icône plugins, ou **Quick actions** avec `Ctrl`/`Cmd` + `:` puis le nom du plugin.
- ⚠️ Un plugin peut disparaître ou cesser d'être maintenu : ne jamais rendre un projet dépendant d'un plugin.

🔎 **Le faux texte (Lorem Ipsum)**

- Le **Lorem Ipsum** est un texte de substitution : il permet de juger la mise en page sans être distrait par le contenu.
- Plusieurs plugins le génèrent (`Loremzer`, `Lorem Ipsum`…) : ils demandent un **nombre** et un **type** (mots, phrases, paragraphes,...).
- ⚠️ Il faut **éditer le bloc de texte** (double-clic) avant d'appliquer le plugin, sinon rien ne s'insère.

✏ **Générer du faux texte**
 
- Installer un plugin de Lorem Ipsum depuis la communauté Figma (`Loremzer`, `Lorem Ipsum`…).
- Créer un bloc de texte de **4 colonnes** de large, lui appliquer votre style `corps`.
- Double-cliquer dans le bloc pour l'**éditer**, puis lancer le plugin et générer **2 paragraphes**.
- Générer ensuite **5 mots** dans un second bloc, auquel vous appliquerez votre style `titre`.

► **À retenir pour le projet** : le faux texte sert à maquetter vite, mais un contenu réel change une mise en page. Un vrai titre est plus long qu'un « Lorem ipsum dolor » — anticipez.

## 7 — Personnaliser les blocs

🔎 **Les propriétés d'apparence**

| Propriété | Panneau | Équivalent CSS |
|---|---|---|
| Coins arrondis | Appearance → *corner radius* | `border-radius` |
| Opacité | Appearance ou Fill (%) | `opacity` |
| Contour / bordure | Stroke (inside, center, outside) | `border` |
| Ombre portée | Effects → *Drop shadow* | `box-shadow` |
| Flou | Effects → *Layer blur* | `filter: blur()` |

► L'opacité se règle à deux endroits : sur **le calque entier** (Appearance) ou sur **un remplissage seul** (Fill). Le résultat n'est pas le même.

✏ **Créer un bloc de texte sur un bloc de couleur**

- Typographie : **Urbanist**, taille **16px**, 2 paragraphes, aligné sur **4 colonnes**.
- ⚠️ La couleur de fond n'est **pas** sur le bloc de texte : il y a **deux blocs** superposés.
- Le texte doit conserver une **marge de 30px** avec le bloc de couleur (utiliser les tailles et les coordonnées).
- Utiliser **vertical trim** pour ajuster la hauteur de ligne.

<img alt="Bloc de texte sur bloc de couleur" src="{{ site.baseurl }}/assets/img/figma-tp2-lorem.png" /><br>

✏ **Créer un bloc personnalisé**

- Bloc sur **3 colonnes**
- Photo en arrière-plan (libre)
- Bordure de **17**, à l'intérieur
- Coins arrondis à **30**
- Ombre portée
- Opacité à **40%**

<img alt="Bloc personnalisé" src="{{ site.baseurl }}/assets/img/figma-tp2-bloc-perso.png" /><br>

## 8 — Modes de fusion (Blend modes)

🔎 **Principe**

- Un **mode de fusion** modifie la façon dont un calque interagit visuellement avec ceux situés **en dessous**.
- Accès : panneau **Appearance** → icône goutte 💧 (*Apply blend mode*).
- Les modes sont regroupés par famille : **assombrissants** (Darken, Multiply…), **éclaircissants** (Lighten, Screen…), **contrastants** (Overlay, Soft light…), **composants colorimétriques** (Hue, Saturation, Color, Luminosity).
- ⚠️ Sur une frame ou un groupe, **Pass through** est le réglage par défaut : le groupe laisse ses calques fusionner avec l'arrière-plan. En choisissant **Normal**, le groupe s'isole.

✏ **Reproduire l'image**

- Taille du carré : **200**
- Couleur du carré de fond : `FF0000`
- Couleur des autres carrés : `0900FF`
- Effets utilisés : **hue**, **exclusion**, **darken**, et aucun

<img alt="Cinq carrés identiques" src="{{ site.baseurl }}/assets/img/figma-tp2-fusion.png" /><br>

► Les cinq carrés sont **identiques** : seul le mode de fusion change. À vous de trouver lequel est appliqué à chacun.

## 9 — Les masques

🔎 **Principe**

- Un **masque** n'affiche que la partie d'un calque visible à travers une forme. Il agit comme une **fenêtre** : tout ce qui dépasse est masqué.
- Exemple : un cercle utilisé pour afficher une photo en rond.
- Mise en place : sélectionner la forme → clic droit → **Use as mask** (`Ctrl`/`Cmd` + `Alt` + `M`).
- Dans le panneau Layers, un **Mask group** apparaît : la forme masquante est **en bas**, et tout ce qui se trouve **au-dessus d'elle dans le groupe** est contraint par elle.

<img alt="Mask group" src="{{ site.baseurl }}/assets/img/figma-tp2-masque.png" /><br>

► Le masque ne détruit rien : masquer n'est pas rogner. On peut à tout moment déplacer le contenu à l'intérieur du masque, ou retirer le masque.

✏ **Créer un masque**

- Créer un carré de **200**
- Créer **3 barres verticales** rouge, verte, bleue, puis les pencher à **45°**
- Créer un masque avec le carré et placer les 3 barres à l'intérieur

<img alt="Masque avec barres" src="{{ site.baseurl }}/assets/img/figma-tp2-masque-2.png" /><br>

## 10 — Boolean groups / Pathfinder

🔎 **Combiner des formes**

Les opérations booléennes combinent plusieurs formes en une seule (comme le Pathfinder d'Illustrator) :

| Opération | Raccourci | Résultat |
|---|---|---|
| **Union** | `Alt + Maj + U` | fusionne les formes |
| **Subtract** | `Alt + Maj + S` | soustrait la forme du dessus |
| **Intersect** | `Alt + Maj + I` | ne garde que la zone commune |
| **Exclude** | `Alt + Maj + E` | ne garde que les zones non communes |
| **Flatten** | `Alt + Maj + F` | aplatit le résultat en un seul vecteur |

► Une opération booléenne reste **modifiable** : les formes d'origine sont conservées dans le groupe et peuvent être déplacées. **Flatten**, en revanche, est définitif.

► C'est ainsi que se fabriquent la plupart des **icônes** : quelques formes simples combinées, puis exportées en SVG.

✏ **Combiner des formes**

- Créer deux carrés qui se chevauchent et tester **les quatre opérations** (union, subtract, intersect, exclude).
- Nommer chaque résultat dans le panneau Layers.

<img alt="Masque avec barres" src="{{ site.baseurl }}/assets/img/figma-tp2-boolean.png" /><br>

## Rendu

- Renommer et organiser tous vos calques.
- Créer un point d'historique `rendu-tp02` (`Ctrl`/`Cmd` + `Alt` + `S`).
- Partager le fichier en édition (*Share → Share settings → Anyone → Edit → Save*) et déposer le lien sur itslearning.
- Vérifier éventuellement le lien avec un camarade avant de le déposer.
