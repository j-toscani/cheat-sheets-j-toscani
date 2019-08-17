# Bootstrap

## Was ist Bootstrap?

Bootstrap ist eine einfache Art Design und Strukturen in Webseiten einzubauen ohne Kenntnisse über CSS und Javascript. Es liefert einen grundlegenden Rahmen und viele Beispiele über die eine Webseite schnell und relativ unkompliziert designed werden kann. Sowohl farben, Bereiche und auch Designelemente sind enthalten. Zudem liefert es ein System Webseiten "responsive" aufzubauen und für unterschiedliche Geräte unterschiedliche zu strukturieren.

## Wie funktioniert Bootstrap?

### First things first:

Damit Bootstrap in einem HTML-Dokument nutzbar wird muss folgendes Code-Snippet in das Dokument kopiert werden:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <!-- Required meta tags -->
    <meta charset="utf-8" />
    <meta
      name="viewport"
      content="width=device-width, initial-scale=1, shrink-to-fit=no"
    />

    <!-- Bootstrap CSS -->
    <link
      rel="stylesheet"
      href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css"
      integrity="sha384-ggOyR0iXCbMQv3Xipma34MD+dH/1fQ784/j6cY/iJTQUOhcWr7x9JvoRxT2MZw1T"
      crossorigin="anonymous"
    />

    <title>Hello, world!</title>
  </head>
  <body>
    <h1>Hello, world!</h1>

    <!-- Optional JavaScript -->
    <!-- jQuery first, then Popper.js, then Bootstrap JS -->
    <script
      src="https://code.jquery.com/jquery-3.3.1.slim.min.js"
      integrity="sha384-q8i/X+965DzO0rT7abK41JStQIAqVgRVzpbzo5smXKp4YfRvH+8abtTE1Pi6jizo"
      crossorigin="anonymous"
    ></script>
    <script
      src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.7/umd/popper.min.js"
      integrity="sha384-UO2eT0CpHqdSJQ6hJty5KVphtPhzWj9WO1clHTMGa3JDZwrnQq4sF86dIHNDz0W1"
      crossorigin="anonymous"
    ></script>
    <script
      src="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/js/bootstrap.min.js"
      integrity="sha384-JjSmVgyd0p3pXB1rRibZUAYoIIy6OrQ6VrjIEaFf/nJGzIxFDsf4x0xIM+B07jRM"
      crossorigin="anonymous"
    ></script>
  </body>
</html>
```

### Das Gridsystem:

Das Gridsystem basiert auf reihen und Spalten um die Seite über HTML hinaus zu strukturieren. Es hilft sich die Webseite vorher in konkrete Bereiche einzuteilen.

Um das Gridsytem nutzen zu können sollte der Bereich in folgenden "Klammern" gesetzt werden:

```html
<div class="container">
  <div class="row">
    <!-- CONTENT AND FURTHER STRUCTURE -->
  </div>
</div>
```

Eine `row` ist in 12 Abschnitte unterteilt. Um diese auf die Inhalte zu verteilen wird das Attribut `col` genutzt. Bei `col-x` gibt "x" an, wie viele der 12 Bereiche für den Inhalt genutzt werden. `col-4` und `col-8` würde 2 Bereiche mit dem Verhältnis 1:2 erstellen. Content der in einer Reihe angegeben sein soll sollte in einem `<div> </div>`hinterlegt werden. Wird `col` nicht weiter spezifiziert, werden die 12 Bereiche gleich auf die Inhalte verteilt.

```html
<div class="container">
  <div class="row">
    <div class="col">
      1 of 2
    </div>
    <div class="col">
      2 of 2
    </div>
  </div>
  <div class="row">
    <div class="col">
      1 of 3
    </div>
    <div class="col">
      2 of 3
    </div>
    <div class="col">
      3 of 3
    </div>
  </div>
</div>
```

Dieser Code erstellt eine Tabelle mit zwei Zeilen. Die erste Zeile hat zwei Spalten die gleich groß sind. Die zweite Zeile hat drei Spalten die gleich groß sind.

[Bootstrap - Dokumentation zu Grid](https://getbootstrap.com/docs/4.3/layout/grid/)
