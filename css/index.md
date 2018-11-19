---
title: "Thinker"
layout: "doc"
---
# CSS Basics

## CSS Grid

Mit CSS Grids können wir Webseiten direkt mit CSS layouten und Elemente unabhänig von ihrer Reinfolge im HTML so plaziren wie wir möcheten. Das bedeutet wir können flexible Spalten und Reihen (grid rows und grid columns) anlegen und unsere Webseiten-Elemente dann komplett frei in diesem Grid platzieren.

### CSS Grid: Wichtige Begriffe

Um CSS Grid anzuwenden, benötigst du ein paar neue Begriffe, die ich hier einmal in einer kleinen Übersicht zusammen gefasst habe.

** Grid container **

Der Grid Container ist der äußerste Container, in dem das Grid gebaut wird. Die CSS-Klasse für dieses HTML-Element muss display: grid heißen.

** Grid item **

Ein Grid item ist jedes Element im Grid, das direkt im Container sitzt (also nicht die Child-Elemente innerhalb von Grid items).

** Grid line **

Es gibt zwei unterschiedliche Grid lines. Die vertikalen Grid-Linien werden „columns“ genannt, die horizontalen „rows“.

![](/img/grids1.png)

** Grid cell **

Grid cell werden alle einzelnen Zellen des Grids genannt.

![](/img/grids2.png)

** Grid area **

Mehrere Zellen zusammengenommen bilden eine Grid area.

![](/img/grids3.png)

** Grid track **

Grid tracks werden alle Spalten und Reihen des Grids genannt, also der Bereich zwischen zwei Column lines oder zwei Row lines.

![](/img/grids4.png)

** Grid gap **

Die Zwischenräume zwischen den Grid rows oder columns sind die Grid gaps (sie können z.B. einen festen Pixelwert von 15px haben). Diese Spalten werden auch auch gutter genannt. Die CSS-Werte sind grid-column-gap und grid-row-gap. Wichtig ist sich zu merken, dass die Zwischenräume nur innerhalb des Grids angelegt werden und nicht an den äußeren Grid lines (bzw. am Rand des Containers).

![](/img/grids5.png)

#### Der Wert "fr"

fr (steht für fraction) ist ein neuer Wert, der für CSS Grid eingeführt wurde. grid-container: 1fr bedeutet, das eine Fraktion des zur Verfügung stehenden Platzes genutzt wird.
Grid template column

Du kannst deine Grid-columns z.b. so anlegen:

```
grid-template-columns: 3fr 1fr 1fr;
```

Das würde in folgendes Grid-Layout resultieren: 

![](/img/grids6.png)

** Grid template rows **

„auto“ ist hier standard und bedeutet, dass der Inhalt die Höhe der grid-row bestimmt. Du kannst aber auch feste Pixel-Maße oder einen Prozentwert angeben.

grid-template-rows: 120px 25% auto;


# CSS Extended

## CSS: Units

```
* {
    /* absolute units */
    width: 100px;      /* pixels */

    /* physical units */
    /* (not suitable for screen display) */
    font-size: 12pt;   /* points */
    font-size: 1pc;    /* picas == 12pt */
    width: 5mm;        /* millimeters */
    width: 1.2cm;      /* centimeters */
    width: 0.5in;      /* inches */

    /* relative units */
    height: 20%;       /* percent of parent size */
    padding: 1.5em;    /* 1em == current font size */
    font-size: 1.5rem; /* root em: base font-size on body-level */
    height: 50vh;      /* % of the viewport height */
    width: 50vw;       /* % of the viewport width */

    /* unit-less */
    padding: 0;        /* if 0, no unit is needed */
    line-height: 1.5;  /* is the same as 150% or 1.5em in this case */
    opacity: 0.5;
}
```
### Unit: Colors

```
* {
    color: green;                     /* named color */
    color: rgb(255, 0, 0);            /* RGB values */
    color: rgb(255, 0, 0, 0.5);       /* RGB values + alpha */
    color: #FF0000;                   /* hexadecimal RGB */
    color: hsl(240, 100%, 50%);       /* hue, saturation, lightness */
    color: hsla(240, 100%, 50%, 0.5); /* HSL + alpha */
}
```

[MDN über Values und Units](https://developer.mozilla.org/en-US/Learn/CSS/Introduction_to_CSS/Values_and_units)

## CSS: Backgrounds

### Background color

```
* {
    background-color: rgb(255, 40, 0);
}
```

### Background images

```
* {
    background-image: url(http://lorempixel.com/1024/768/cats/);

    /* optionally, you can specify if the background image should
    repeat or not ... */
    background-repeat: no-repeat;

    /* ... and how it should be positioned */
    background-position: center center;
}
for fullscreen backgrounds you would do:

* {
    background-image: url(http://lorempixel.com/1024/768/cats/);
    background-repeat: cover; /* cover the entire ares of the element */
}

```


**relevant CSS properties:**

- background-image
- background-repeat
- background-position
- background-attachment

### Gradients

[CSS Gradients auf CSS Tricks](https://css-tricks.com/css3-gradients/)


<iframe height='300' scrolling='no' title='CSS: Background' src='//codepen.io/macky/embed/PxJrbQ/?height=300&theme-id=35174&default-tab=css,result' frameborder='no' allowtransparency='true' allowfullscreen='true' style='width: 100%;'>
</iframe>

## CSS: Basic typography

these are the most important typography-related CSS properties:

- color
- font-size
- font-style
- font-variant
- font-weight
- letter-spacing
- word-spacing
- line-height
- text-align
text-decoration
text-indent
text-transform

<iframe height='570' scrolling='no' title='CSS: Typography' src='//codepen.io/macky/embed/bQoJWG/?height=570&theme-id=35174&default-tab=css,result' frameborder='no' allowtransparency='true' allowfullscreen='true' style='width: 100%;'>
</iframe>
<iframe height='1447' scrolling='no' title='CSS: Typography paragraph' src='//codepen.io/macky/embed/WYZBNR/?height=1447&theme-id=35174&default-tab=css,result' frameborder='no' allowtransparency='true' allowfullscreen='true' style='width: 100%;'>
</iframe>

## CSS: Effects

### Drop shadows

<iframe height='300' scrolling='no' title='CSS: Box Shadow' src='//codepen.io/macky/embed/BGwXOy/?height=300&theme-id=35174&default-tab=css,result' frameborder='no' allowtransparency='true' allowfullscreen='true' style='width: 100%;'>
</iframe>

## CSS: Responsive

### Beispiel

<iframe height='425' scrolling='no' title='CSS: Responsive' src='//codepen.io/macky/embed/dQVxQw/?height=425&theme-id=35174&default-tab=css,result' frameborder='no' allowtransparency='true' allowfullscreen='true' style='width: 100%;'>
</iframe>