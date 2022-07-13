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

#### Neues Repository erstellen

1. `mkdir` in der Konsole einen neuen Ordner erstellen
1. `cd [NewFolder]` in den neuen Ordner wechseln
1. `git init` um das Repo zu initialisieren
1. Auf [github.com](http:\www.github.com) neues Repository anklicken und den Anweisungen folgen
1. Dateien erstellen, einzeln via `git add [NewFile]` adden
1. Ersten commit mit "first commit" kommentieren.

#### Neuen Branch erstellen

1. `git checkout -b [BranchName]` Neuen Branch erstellen und dahin wechseln
1. `git commit -a -m "[ChangeDescription]"` Änderungen comitten
1. `git push -u origin [BranchName]`Branch ins Git pushen

##### Consolen Output:

`git checkout -b j-toscani`
Switched to a new branch 'j-toscani'  
`git status`  
 On branch j-toscani  
 Changes not staged for commit:  
 (use "git add <file>..." to update what will be committed)  
 (use "git checkout -- <file>..." to discard changes in working directory)  
 modified: j-toscani.md  
no changes added to commit (use "git add" and/or "git commit -a")

`git add j-tocsani.md`

`git commit -m "added content to my md-Document"`

`git push -u origin j-toscani`

Enumerating objects: 7, done.  
Counting objects: 100% (7/7), done.  
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.  
Writing objects: 100% (4/4), 408 bytes | 408.00 KiB/s, done.  
Total 4 (delta 2), reused 0 (delta 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.  
remote:

remote: Create a pull request for 'j-toscani' on GitHub by visiting:
remote: https://github.com/neuefische/sushi-app/pull/new/j-toscani

remote:
To github.com:neuefische/sushi-app.git

- [new branch] j-toscani -> j-toscani
  Branch 'j-toscani' set up to track remote branch 'j-toscani' from 'origin'.

## Befehle

| Command                     | Use                                           |
| --------------------------- | --------------------------------------------- |
| `add .`                     | Komplettes Repo der Stage hinzufügen          |
| `add [Dateienname]`         | Nur Änderungen einer datei adden              |
| `commit -m`                 | Repo der Stage commiten                       |
| `commit -a -m`              | Repo der Stage hinzufügen und direkt comitten |
| `push origin master`        | Commit in den Master des gitHub pushen        |
| `branch [BranchName]`       | Branch erstellen                              |
| `push -u origin BranchName` | Commit in einen Branch des gitHub pushen      |
| `git diff <hash-from>..<hash-to> -- ./foo-folder` | Einen Ordner mit einem älteren Stand vergleichen |
| `git checkout <hash> -- ./foo-folder` | Einen Ordner auf einen älteren Stand zurücksetzen |
