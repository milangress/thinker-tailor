---
title: "Thinker"
layout: "doc"
---

# CSS Extended

- [CSS: Units](#css-units)
    - Colors
- [CSS: Backgrounds](#css-backgrounds)
    - Background color
    - Background images
    - Gradients
- [CSS: Basic typography](#css-basic-typography)
- [CSS: Effects](#css-effects)

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

#### Beispiel

<iframe height='425' scrolling='no' title='CSS: Responsive' src='//codepen.io/macky/embed/dQVxQw/?height=425&theme-id=35174&default-tab=css,result' frameborder='no' allowtransparency='true' allowfullscreen='true' style='width: 100%;'>
</iframe>