# Terminal Shell Commands

## Ressources

1. [Sich bewegen und Dateien Manipulieren](https://www.codecademy.com/learn/learn-the-command-line)
1.

### SSH-Key erstellen

ssh-keygen -t rsa -b 4096 -C "julian_toscani@gmx.de"  
eval "\$(ssh-agent -s)"  
nano ~/.ssh/config

dort eingeben:  
Host \*
AddKeysToAgent yes
UseKeychain yes
IdentityFile ~/.ssh/id_rsa
sh-add -K ~/.ssh/id_rsa

Public Key ausgeben:  
cat id_rsa.pub
(dieser muss dann für jedes Gerät auf dem Server oder dem GitHub Profil hinterlegt werden.)

## Befehle

### Allgmeines

| Command       | Use                                                       |
| ------------- | --------------------------------------------------------- |
| `man`         | mögliche Erweiterungen für einen Befehl anzeigen (Manual) |
| `:q!`oder `q` | einen Editor beenden                                      |
| `code .`      | öffnet die Dateien im Verzeichnis mit VSCode              |

### Shortcuts zur Inputmanipulation

| Command    | Use                                                      |
| ---------- | -------------------------------------------------------- |
| `Esc + T`  | Die letzten beiden Worte vor dem Cursor vertauscchen     |
| `Ctrl + H` | Verhalten entspricht dem drücken von `Entf`              |
| `Ctrl + W` | Verhalten entspricht dem drücken von `Ctrl + Entf`       |
| `Ctrl + R` | Aktiviert eine Suche in der Kommandohistorie             |
| `Ctrl + U` | Kommandozeile löschen                                    |
| `Ctrl + C` | Kommando stoppen                                         |
| `Ctrl + L` | Kommando-Output entfernen                                |
| `Ctrl + T` | Die letzten beiden Buchstaben vor dem Cursor vertauschen |

### In Verzeichnissen bewegen

| Command                        | Use                                                            |
| ------------------------------ | -------------------------------------------------------------- |
| `ls`                           | um liste des Verzeichnisses aufzurufen                         |
| `exa -T`                       | öffnet den Verzeichnisbaum ausgehend vom aktuellen Verzeichnis |
| `cd [Pfad]` oder `cd [Ordner]` | Verzeichnis wechseln zu Ordner oder einem bestimmten Pfad      |
| `cd ..`                        | ein Verzeichnis zurück Navigieren                              |
| `../`                          | in einem Pfad ein Verzeichnis zurück gehen                     |
| `mkdir`                        | neues Verzeichnis erstellen                                    |
| `pwd` oder `~+`                | Arbeitsverzeichnis anzeigen                                    |
| `exit`                         | Die Bash schließen                                             |

### Daten und Verzeichnisse manipulieren

| Command                     | Use                                                                    |
| --------------------------- | ---------------------------------------------------------------------- |
| `touch`                     | erstellt eine leere Datei                                              |
| `cp [Name] [NewName]`       | Kopiert die Datei mit dem Namen "Name" unter dem neuen Namen "NewName" |
| `cp [Name1] [Name2] [/dir]` | Kopiert die Dateien "Name" & "NewName" in das Verzeichnis /dir         |
| `cp m*.txt`                 | Kopiert alle ".txt" Dateien die mit "m" anfangen                       |
| `mv`                        | eine Datei bewegen                                                     |
| `rm`                        | eine Datei löschen                                                     |
| `rm -R`                     | eine Verzeichnis löschen                                               |

### Besondere Zeichen

| Command        | Use                                                                                                                                                     |
| -------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `\``           | Dient als "escape Character". Mehr infos dazu [hier](https://stackoverflow.com/questions/15783701/which-characters-need-to-be-escaped-when-using-bash). |
| `#`            | Leitet einen Kommentar ein                                                                                                                              |
| `.`            | Aktuelles Verzeichnis. Auch nutzbar um "versteckte Dateien" zu benennen, wenn `.` am Anfang des Dateinamens steht.                                      |
| `..`           | Verweis zum Elternverzeichnis                                                                                                                           |
| `~`            | Verweis zum Heimverzeichnis                                                                                                                             |
| `*`, `?`, `[]` | Wildcards. `*` sind alle möglichen Zeichen und Zeichen Ketten, `?` ist ein Zeichen das alle möglichen Zeichen sein können                               |
| `[]`           | Ist eine Wildcard für ein Zeichen, in dem eine Range von bestimmten Zeichen festgelegt werden kann, z.B. `[3-5]` erlaubt die Zeichen `3`, `4` & `5`     |
| `|`            | Benutzt den Output des letzten Befehls und nutzt ihn als Input für den nächsten Befehl                                                                  |
| `>`            | Nimmt den output vom vorherigen Kommando und nutzt diesen für die Manipulation einer Datei. Bsp: `ls > file.txt`. Überschreibt vorhandene Dateien.      |
| `>>`           | Wie `>`. Allerdings wird der output angehangen, die Datei daher nicht überschrieben.                                                                    |
| `&&`           | Führt mehrere Scripte hintereinander aus. Die nachfolgenden Scripte werden nur ausgeführt, wenn die vorherigen erfolgreich waren.                       |
