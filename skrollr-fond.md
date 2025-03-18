---
layout: default
title: SkrollR - Faire bouger un fond
permalink: /skrollr-fond/
published: true
date: 2024
---

# SkrollR - Faire bouger un fond

## ETAPE 1

- Créer une structure HTML
- Connecter un fichier CSS
- Connecter le fichier JS et l'avoir activé (lignes du bas)
- Avoir une image (un fond ici)

![image](https://github.com/user-attachments/assets/06c59634-9970-4d7b-9cdb-de7e3b8e3804)

**Voici le code du HTML, nous pouvons y retrouver le lien CSS, le JS. Nous reviendrons sur le code dans la balise ```<body>```.**

```html
<!doctype html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport"
          content="width=device-width, user-scalable=no, initial-scale=1.0, maximum-scale=1.0, minimum-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
    <link rel="stylesheet" href="style.css">
</head>
<body data-0="background-position-X:0px" data-3000="background-position-X:-3000px">


<script src="js/skrollr.js"></script>
<script type="text/javascript">
    var s = skrollr.init();
</script>

</body>
</html>
```

**Voici le code CSS, il ne contient que l'image en background.**

```css
body { background-image: url("fond.jpg")}
```

Nous obtenons pour le moment ceci lorsque nous utilisons la souris : 

![1](fond1.webp)

**Revenons sur le code précédent :**

Le CSS permet de mettre une image en arrière plan du ```body```

La ligne :

```<body data-0="background-position-X:0px" data-3000="background-position-X:-3000px">```

Permet de spécifier que le fond se sera déplacer de ```-3000px``` lorsque nous aurons "scrollé" 3000px (data-3000) (les valeurs sont choisies ici globalement au hasard).

Cependant, le fond subit également le déplacement vertical "classique", ce qui donne cet effet de déplacement vertical ET horizontal.

Pour régler ce problème, nous allons spécifier que notre fond est "fixe".

**Modifier le CSS pour obtenir :** 

```css
body { background-image: url("fond.jpg"); background-attachment: fixed}
```
