# CSS Extended

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