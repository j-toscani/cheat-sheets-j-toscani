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

### In Verzeichnissen bewegen

| Command                        | Use                                                            |
| ------------------------------ | -------------------------------------------------------------- |
| `ls`                           | um liste des Verzeichnisses aufzurufen                         |
| `exa -T`                       | öffnet den Verzeichnisbaum ausgehend vom aktuellen Verzeichnis |
| `cd [Pfad]` oder `cd [Ordner]` | Verzeichnis wechseln zu Ordner oder einem bestimmten Pfad      |
| `cd ..`                        | ein Verzeichnis zurück Navigieren                              |
| `../`                          | in einem Pfad ein Verzeichnis zurück gehen                     |
| `mkdir`                        | neues Verzeichnis erstellen                                    |
| `pwd`                          | aktuelles Verzeichnis anzeigen                                 |

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
