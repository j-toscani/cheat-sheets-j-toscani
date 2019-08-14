# HTML

## Ressources

1. [Mozilla](https://developer.mozilla.org/en-US/)
1. [Wiki](https://en.wikipedia.org/wiki/List_of_XML_and_HTML_character_entity_references)

## Begriffe

| Begriff | Beispiel                       | Erklärung                                                                                  |
| ------- | ------------------------------ | ------------------------------------------------------------------------------------------ |
| Tag     | _\<img>_ oder _\<div>_         | Beschreibt ein Element. Ist der Grund dafür, dass Inhalte unterschiedlich angezeigt werden |
| Content | \<div> _Hello World_ \</div>   | Inhalt im Tag, z.B. ein text, der zur Überschirft formatiert werden soll                   |
| Element | **\<div> Hello World \</div>** | Tag + Content                                                                              |
| VoidTag | <img src="" alt="">            | Tag, der keinen Content umschließt/manipuliert                                             |

![Element Struktur](/resources/html_element-structure.png)

#### Hausaufgabe:

- Wann aside innerhalb von article, wann außerhalb?
  - Soll der Inhalt neben dem Artikel stehen, dann außerhalb. Soll es im Artikel stehen, dann innerhalb.
- Was kommt in main rein? Wie oft darf man main pro Seite verwenden?
  - Es darf nur einmal genutzt werden. Beschreibt den Hauptinhalt des Dokuments. Hat starke, semantische Wirkung.
- Wann ist div geeigneter als section?
  - asd
- Wann verwendet man b und wann strong? Wann i und wann em?
  - asd
- Wie baut man eine figure mit einem Bild und Text auf?
  - asd
- Wofür steht dl, dd und dt
  - asd
- Was sind 3 void Elemente, die du kennst?
  - asd
- Wofür wird small verwendet?
  - asd
- Was ist der Unterschied zwischen dem img- und dem picture-Element?
  - asd
- Welche 5 input-types kennst du neben <input type="text">?
  - asd
- Was macht man mit select und option?
  - asd

## Befehle

### Struktur und Semantik

In HTML

| Command     | Use                                                                                                  | Explanation                                                                                                                                                                                                               |
| ----------- | ---------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `<body>`    | Includes all Elements of Webpage. Can only be used once                                              | Umschießt alle Strukturierenden und inhaltlichen Elemente der Seite                                                                                                                                                       |
| `<header>`  | Top Most Section ob Webpage                                                                          | Beschreibt den Bereich der Kopfzeile der Webseite. Hier werden oft Headerbilder hinterlegt oder die Navigationsleiste eingefügt.                                                                                          |
| `<main>`    | Only to be used once. Main Part of Webpage                                                           | Beschreibt den Hauptteil der Webseite.                                                                                                                                                                                    |
| `<article>` | Beschreibt einen unabhängigen Abschnitt                                                              | The HTML <article> element represents a self-contained composition in a document, page, application, or site, which is intended to be independently distributable or reusable                                             |
| `<aside>`   | Erstellt abschnitt mit geringerer Wichtigkeit                                                        | The HTML <aside> element represents a portion of a document whose content is only indirectly related to the document's main content. Asides are frequently presented as sidebars or call-out boxes.                       |
| `<section>` | Generischer Tag um einen Abschnitt anzuzeigen                                                        | The HTML <section> element represents a standalone section — which doesn't have a more specific semantic element to represent it — contained within an HTML document. Typically, but not always, sections have a heading. |
| `<footer>`  | Wird genutzt um Informationselemente zum Betreiber zu hinterlegen (Kontakt, Anfahrt, Impressum etc.) | Bottom most Section                                                                                                                                                                                                       |

### Einbinden von Medien

### Einbinden von Input und Formularen
