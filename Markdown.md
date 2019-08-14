# Markdown

[**Was Markdown genauer ist**](https://www.markdownguide.org/getting-started#whats-markdown)

## Ressources

1. [Tutrorial](https://www.markdowntutorial.com/)
1. [cheat sheet](https://guides.github.com/pdfs/markdown-cheatsheet-online.pdf)

## Befehle

### Textformat

```Markdown
_lorem_ oder        "Schrift kursiv"
*lorem*

__lorem__ oder      "Schrift fett"
**lorem**

\* \*               "Format entfernen"
```

### Aufzählungen

```Markdown
-   "ungeordnete Liste"
1.  "geordnete Liste"
  - oder "doppelt einrücken für nächste Ebene"
  2.
```

### Links

```Markdown
[git](#gitpush)  "in einem Dokument auf die Überschrift "git push" verlinken"
```

```Markdown
() "Link auf Seite einfügen und Linkbar machen"
[] "Text im Dokument als Link darstellen"
[] im text + []: "www.xyz.de"; "Referenz link im Document einfügen. Ist nicht sichtbar!"
```

```Markdown
![Benjamin Bannekat](https://octodex.github.com/images/bannekat.png) "Ein Bild einfügen"
Logik: "!" + "Alternative Bezeichnung (Text)" + "Link zum Bild"
```

```Markdown
- ">" Block Quote einstellen
```

> This is what a Block Quote looks like :)

### Source Code

\```Sprache  
Befehl  
\```

##### z.B. für HTML:

\```html  
\<h1>Headline\</h1>\
\```

```html
<h1>Dies ist eine Änderung</h1>
```
