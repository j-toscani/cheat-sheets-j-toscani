# Cascading Style Sheets (CSS)

## Resources

1. [CSS - Tricks](https://css-tricks.com/)
1. [CSS - Spiel um Selektoren kennenzulernen](https://flukeout.github.io/)
1. [Hilfe um Farbschemata anzupassen](https://coolors.co/browser/best/1)
1. [Grid vs Flex](https://hackernoon.com/the-ultimate-css-battle-grid-vs-flexbox-d40da0449faf)
   1. [CSS Properties](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Properties_Reference)
   1. [CSS References](https://cssreference.io/)

## Allgemeines

### Vokabular

- Selector
- Properties
- Values

Schaubild

### CSS einbinden

- Externe CSS-Datei via Link
- Inline in die Tags
- In den Head via Style Tags

## CSS nutzen

### Selektoren

Selektoren werden verwendet um gezielt einzelne Elemente anzusteuern und diese Stylen zu können.

### Farben

[Farben für CSS](https://www.w3schools.com/colors/)

### Inline, Block und Inline-Block

- block: volle Breite des Elternelements, neuer Absatz
- inline: im Textfluss, zB. width, height werden nicht respektiert
- inline-block: im Textfluss, width, height werden respektiert

### Flexbox

Über Flexbox kann man in CSS responsive-Websites erstellen. Der Grundgedanke ist, dass man einen Bereich hat, in dem unterschiedliche, voneinander unterscheidbare Elemente sind die man ordnen will. Diese nennt man Items. Man hat die Möglichkeit, diese Elemente entweder horizontal oder vertikal anzuordnen.

Hier einmal Beispielhaft + Kommentaren:

```CSS
.flex-container {
  /* We first create a flex layout context */
  display: flex;

  /* Then we define the flow direction
     and if we allow the items to wrap
   * Remember this is the same as:
   * flex-direction: row;
   * flex-wrap: wrap;
   */
  flex-flow: row wrap;

  /* Then we define how is distributed the remaining space */
  justify-content: space-around;
}
```

#### Befehle um die Items anzuordnen

Dieser Befehl bezieht sich nur auf die horizontale Ebene!

`justify-content:`

| Command         | Use                                              |
| --------------- | ------------------------------------------------ |
| `flex-start`    | Setzt alle Elemente an den Anfang des Containers |
| `flex-end`      | Setzt alle Elemente an das Ende des Containers   |
| `center`        | Setzt alle Elemente in die Mitte des containers  |
| `space-between` | Gleicht die Abstände zwischen den items an       |
| `space-around`  | gleicht den Abstand um die items an              |

### Grid

| Command         | Use                                              |
| --------------- | ------------------------------------------------ |
| `flex-start`    | Setzt alle Elemente an den Anfang des Containers |
| `flex-end`      | Setzt alle Elemente an das Ende des Containers   |
| `center`        | Setzt alle Elemente in die Mitte des containers  |
| `space-between` | Gleicht die Abstände zwischen den items an       |
| `space-around`  | gleicht den Abstand um die items an              |

### Befehle um die Größen anzupassen

| Command          | Use                                                                                                                                                                                                      |
| ---------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `npx`            | n-pixel, absolute Größe                                                                                                                                                                                  |
| `nvh` oder `nvw` | n% der maximalen Höhe oder Breite des verwendeten Geräts (z.B. Smartphone oder Tablet)                                                                                                                   |
| `n%`             | legt die größe auf n% der größe des Elternelements fest                                                                                                                                                  |
| `n%`             | legt die größe auf n% der größe des Elternelements fest                                                                                                                                                  |
| `flex:n`         | gibt einem Element die n-te Menge des restlichen Platzes. Stehen sich zwei `flex`-attribute gegenüber, so wird der "Restplatz" im entsprechenden Verhältnis aufgeteilt. Ähnlich wie `col` bei Bootstrap. |

### Befehle für Schriftgrößen

| Command | Use                                                                                    |
| ------- | -------------------------------------------------------------------------------------- |
| `px`    | Absolute Schriftgröße                                                                  |
| `em`    | Relative Schriftgröße auf Basis der Schriftgröße die im Elternelement definiert wurde. |
| `rem`   | Relative Schriftgröße auf Basis der "Root-Schriftgröße"                                |

#### Befehle um

**Die interessantesten Befehle hier auflisten. Basis hierfür bildet das Spiel**

| Command              | Use                |
| -------------------- | ------------------ |
| `komplexere Befehle` | komplexerer Befehl |
