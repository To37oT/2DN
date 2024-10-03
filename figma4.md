---
layout: default
title: Champs, variables et calculs
permalink: /figma4/
published: true
date: 2024
---

# Variables et affichage

## PARTIE 1 : Réaliser une liste déroulante

### Créer un composant avec 7 variantes
![image](https://github.com/user-attachments/assets/93ea4c7f-1fbe-4aba-b051-9424f66d6fcd)

### Ajouter un changement de variante au clic pour les listes fermées
![image](https://github.com/user-attachments/assets/228c2d74-d8bc-4f42-ac75-81ff0e0fa26a)

### Créer un composant qui servira à créer l'effet visuel du survol
<p>Ce composant possède 2 états : normal et survolé. Etat normal, opacité de 0% et état survolé, opacité de 50%</p>

![image](https://github.com/user-attachments/assets/bc44c398-4821-4dd5-a8c3-2625182fc0a7)<br>

![image](https://github.com/user-attachments/assets/3cfdc528-a36d-47c9-860b-f75b68a7fca9)<br>

![image](https://github.com/user-attachments/assets/920f215a-082a-4ac0-a71d-525974400e60)

### Venir placer ce composant sur les éléments de la liste déroulée
<p>il est possible de changer l'opacité le temps de placer l'éléments</p>

![image](https://github.com/user-attachments/assets/059a8246-243f-4f08-af13-1e3b27595e77)<br>
![image](https://github.com/user-attachments/assets/6acf199f-b9e1-4b93-8841-a9ff893e5075)

### Sur chaque éléments ainsi placé, fabriquer l'interraction de retour.
![image](https://github.com/user-attachments/assets/435094d1-32d8-4425-bb6d-02658174b493)

### Tester la liste déroulante
![image](https://github.com/user-attachments/assets/979415da-1125-4174-a4dd-fedd5dbd8902)

## Partie 2 : Ajouter une variable mouvante

### Créer une variables sur les champs
<p>Ici une variable val sur le premier nombre (le composant au dessus)<br>
La variable s'ajoute sur l'évènement "clic" (il y a déjà une interraction au clic, on ajoute l'effet sur la variable en plus)</p>

![image](https://github.com/user-attachments/assets/aa197a05-79f5-4bc3-927e-9f41c21bafd8)

Ajuster la valeur de la variable en fonction de la valeur cliquée (2 si on clique sur le nombre 2, 3 si on clique sur le nombre 3,...)

Attention, on ne recréé pas de variable une fois **val** créé, on modifie sa valeur.


