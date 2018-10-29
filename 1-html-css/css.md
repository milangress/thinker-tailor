## Kleine Einführung zu CSS


CSS steht für *Cascading Style Sheets*, mit der wir Elemente auf unserer Seite *Stylen* können. In CSS schreiben wir eigentlich Regeln nach denen sich der Browser richten muss um unsere Seite Anzuzeigen. 
Die Struktur dieser Regeln sieht so aus:

```
Selektor {
  Eigenschaft: wert;
  andere-eigenschaft: anderer-wert;
}
```

Der *Selektor* definiert welches Element wir verändern möchten und danach kommt eine Liste mit den Eigenschaften und dessen werten.

Weil Ein Computer nicht besonders schlau ist müssen wir dabei den Satzbau sehr genau befolgen. Um dem Computer zu sagen das Anna rote Haare haben soll würden wir also schreiben:

```
anna {
  haare: rot;
}
```

Aber wir wollen ja keine Menschen stylen sondern HTML tags. Wenn wir also die Hintergrundfarbe unsere Seite verändern wollen schreiben wir:

```
body {
  background-color: magenta;
}
```

In diesem fall wählen wir alle `<Body>` Elemente aus und setzten die Eigenschaft `background-color` auf „magenta“. Wir können auch mehr Eigenschaften hinzufügen:

```
body {
  background-color: magenta;
  font-family: Helvetica;
}
```

Jetzt wird der ganze Text zwischen `<body>` und `</body>` in Helvetica angezeigt.

Wie in HTML können wir Kommentare schreiben um unseren Code Lesbarer zu gestalten:

```
/* Diese CSS Regel verändert die Schriftgröße. 
Dabei ist "rem" eine Einheit die abhängt von der   
grundsätzlichen Schriftgröße. Wenn wir die noch nicht   
verändert haben bedeutet das normalerweise 16px   
(px bedeutet Pixel). 2rem währen dann also 2 x 16px = 32px */
body {
  background-color: magenta;
  font-size: 2rem;
}
```

Es gibt noch viele andere Selektoren neben HTML tags wie `<body>`. Du kannst auch Elemente mit einer bestimmten klasse oder id auswählen. Wenn wir also nur ein `<p>` Element zentrieren wollen können wir zuerst eine Klasse zuweisen:

```
<p class="wichtiger-text">Dieser Text wird Zentriert</p>
```

Jetzt kann ich dieses Element auswählen damit es nur diese Klasse verändert:

```
.wichtiger-text {
  text-align: center;
}
```

Wichtig:
id Selektoren werden nach einem `#` geschrieben während Class Selektoren nach einem Punkt geschrieben werden – `.`

### CSS Datei

CSS und HTML zu trennen macht es einfacher zu verstehen. Aber du musst daran denken dem Browser zu sagen wo die CSS Datei liegt.
Das machst du zwischen den `<head></head>` tags in deinem HTML Dokument:

```
<link rel="stylesheet" href="style.css" />
```


## Jetzt kennst du die Grundlagen zu CSS

[MDN's CSS Dokumentation](https://developer.mozilla.org/en-US/docs/Web/CSS) enthält eine umfassende Auflistung aller Eigenschaften und Werte.
Die Tutorials von Mozilla zu den [CSS Basics](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/CSS_basics) sind ein guter Einstig.