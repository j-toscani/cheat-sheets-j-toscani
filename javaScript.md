# JS-Start

## Ressource

1. [Introduction to JS](http://javascript.info/)

## The Basics

Java-Script wird genutzt um HTML zu manipulieren und zu generieren. Dabei gibt es drei grundlegende Elemente auf die man zurückgreift:

- Variablen
- Funktionen
- Events

Oft läuft es so ab, dass man eine Funktion bei eintreten eines Events aufruft. Das Ergebnis der Funktion ist dann von der jeweiligen Variable abhängig.

### Variables

| Command   | Explanation                                                              |
| --------- | ------------------------------------------------------------------------ |
| String    | Eine Zeichenfolge, meist umgeben von ""                                  |
| mumeric   | Eine Zahl mit der Mathematische Berechnungen durchgeführt werden können. |
| boolean   | dichotome Variable: true/false                                           |
| null      | lehrer Container                                                         |
| undefined | undefinierter Wert                                                       |

#### Was man nicht vergessen sollte:

- Der Operator "+" kann dazu verwendet werden Strings aneinander zu reihen.

- Formatiert man einen boolean in eine Zahl, so steht true für 1 und false für null.
- Eine Variable, die besteht, aber keinen Wert hat, ist leer und hat daher den Wert "null". Eine Variable die "gerufen" wird, aber nie definiert wurde, ist "undefined".
- JS hat functionen und Operatoren, die variablen selbstständig verändern, daher **VORSICHT**.

### Functions

### Events

### How to manipulate HTML

Um HTML zu manipulieren müssen drei Elemente beachtet werden:

- Selector
- Funktion
- Event

Dies kann (auch wenn etwas komplex) in etwa wie folgt aussehen:

1. Erst werden die zu verändernden Elemente definiert.

2. Dann wird der Event definiert. Er ist wie folgt zu lesen:

   - submitButton = Hier geschieht der Event
   - addEventListener = Betrachte dieses Element/Hier wird ein Event beschrieben
   - (Wann soll der Event eintreten? , [more](https://developer.mozilla.org/en-US/docs/Web/Events)
   - Welche Funktion beschreibt die Änderung?)

3. Dann wird die funktion definiert, die beschreibt, welche Änderung wo durchgeführt wird.

```javaScript
"use strict";

// Submit an input after clicking a Button

// Define the elements that have to be included
const submitButton = document.querySelector(".change-theme");
const inputName = document.querySelector(".input-name");
const outputName = document.querySelector("#text");

// Define when the change should be submitted
submitButton.addEventListener("click", logInput);

// Define where the text should be applied
function logInput() {
  outputName.innerHTML = inputName.value;
}
```

#### DOM

Das DOM ist ein browserseitiges Document, was es ermöglicht auf die HTML-Struktur zuzugreifen. Dabei kann man entweder über Klassen (z.B `.container`) id s (z.B. `#navElement`) oder direkt auf Strukturelemente zurückgegriffen werden.

Letzteres ist recht kompliziert. Dazu müssen die unterpunkte einzelnd aufgeführt und mit punkten verbuden werden. Aus diesem Grund werden oft Variablen generiert, um diese Elemente anzusteuern ([more](http://javascript.info/dom-navigation)).
