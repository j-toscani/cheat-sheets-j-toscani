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

- `ls` um liste aufzurufen (was befindet sich im Verzeichnis?)
- `cd` (change directory) verzeichnis wechseln
- `cd ..` ein Verzeichnis zurück
- `mkdir` neues Verzeichnis erstellen
