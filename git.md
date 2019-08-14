# Git

## Ressources

1. [Einfach Einstieg in Git](https://rogerdudler.github.io/git-guide/index.de.html)
1. [Lernspiel (Terminus)](http://web.mit.edu/mprat/Public/web/Terminus/Web/main.html)

## Prozesse

### Best Practise

1. Kleinteilig committen damit die Messages klar definieren, was commited wurde.

### Arbeitsphasen

1. Lokal
   1. In VSCode speichern
   1. In der Stage speichern
   1. In den Baum commiten
1. Online
   1. Auf GitHub pushen

![Bild des WorkFlows](/resources/gitWorkflow.jpg)

#### Neuen Branch erstellen

1. `git checkout -b [BranchName]` Neuen Branch erstellen und dahin wechseln
1. `git commit -a -m "[ChangeDescription]"` Änderungen comitten
1. `git push --set-upstream origin [BranchName]`Branch ins Git pushen

## Befehle

| Command                                | Use                                           |
| -------------------------------------- | --------------------------------------------- |
| `add .`                                | Komplettes Repo der Stage hinzufügen          |
| `add [Dateienname]`                    | Nur Änderungen einer datei adden              |
| `commit -m`                            | Repo der Stage commiten                       |
| `commit -a -m`                         | Repo der Stage hinzufügen und direkt comitten |
| `push origin master`                   | Commit in den Master des gitHub pushen        |
| `branch [BranchName]`                  | Branch erstellen                              |
| `push --setupstream origin BranchName` | Commit in einen Branch des gitHub pushen      |
