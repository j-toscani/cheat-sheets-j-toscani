# HTML

## Ressources

1. [Mozilla](https://developer.mozilla.org/en-US/)
1. [Wiki](https://en.wikipedia.org/wiki/List_of_XML_and_HTML_character_entity_references)
1. [The Living Standard](https://html.spec.whatwg.org/dev/)

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
  - Wenn ein Abschnitt markiert werden muss, der nicht wirklich ein anderer Abschnitt ist, sondern nur anders via CSS gestyled wird
- Wann verwendet man b und wann strong? Wann i und wann emphasis?
  - i und b sind nur da um das Design zu ändern. strong und emphasis wenn die Wörter hervorgehoben werden, weil sie eine semantische beduetung für den Inhalt der Seite haben
- Wie baut man eine figure mit einem Bild und Text auf?

```html
<figure>
  <img src="/media/examples/elephant-660-480.jpg" alt="Elephant at sunset" />
  <figcaption>An elephant at sunset</figcaption>
</figure>
```

- Wofür steht dl, dd und dt
  - `dl`= description list-> wird genutzt um eine Liste zu erstellen, in der Wörter und ihre Beschreibungen aufgelistet werden können
  - `dt` = Description Term-> Definiert das Wort, dass beschrieben werden soll
  - `dd` = description detail-> fügt dem Wort weitere Detailinformationen hinzu (Beschreibung, Übersetzung, Erklärung etc.)
- Was sind 3 void Elemente, die du kennst?
  - img, link, input
- Wofür wird small verwendet?
  - Verringert die Schriftgröße eines Textes um 1
    - _Hat das auch eine semantische Wirkung?_
- Was ist der Unterschied zwischen dem img- und dem picture-Element?
  - `<img>` wird im `<picture>` element verwendet
  - `<picture>` bietet dem browser und dem Gerät über source unterschiedliche quellen für ein bild an und kann sie so beschreiben, dass das Gerät für sich die richtige Quelle wählt
    - _Nach welcher Logik entscheidet das Gerät?_
- Welche 5 input-types kennst du neben `<input type="text">`?
  - button, checkbox, email, radio, submit
  - Siehe dazu [hier](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input)
- Was macht man mit select und option?
  - `<select>` gibt mir die Möglichkeit ein Dropdown Menü einzubauen und über `<option>` kann ich die darin enthaltenen optionen definieren

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

| Command     | Use | Explanation |
| ----------- | --- | ----------- |
| `<source>`  | In  |             |
| `<picture>` | In  |             |
| `<img>`     | In  |             |
| `<audio>`   | In  |             |
| `<video>`   | In  |             |

[MDN: Source](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/source)

### Einbinden von Input und Formularen

#### `<Input>`

| Input Type  | Use | Explanation |
| ----------- | --- | ----------- |
| `<source>`  | In  |             |
| `<picture>` | In  |             |
| `<img>`     | In  |             |
| `<audio>`   | In  |             |
| `<video>`   | In  |             |

[MDN: Input](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input)

#### `<Form>`
