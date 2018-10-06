# Trinket M0 installation guide

### Pre-requis :
- Pc
- Nintendo Switch
- fer a souder
- Trinket M0
- Tournevis
- Kynar

## Software
- Installer le logiciel arduino : `sudo pacman -S arduino`
- Lancer le logiciel : `sudo arduino`
- Dans `File->Preferences`, ajouter cette URL : `https://adafruit.github.io/arduino-board-index/package_adafruit_index.json`
- Dans `Tools->Board->Board Manager` installer : `Arduino SAMD Boards by Arduino`, `Arduino SAMD Boards by Adafruit`
- Dans `Tools->Board` selectionner `Adafruit Trinket M0`
 - Dans `Sketch->Include Library->Manage Libraries` installer : `USBHost`, `Adafruit DotStar`

Fin de la configuration.

On peut maintenant brancher en usb le Trinket M0.
Dans `Tools->Port` selectionner le Trinket M0

Telecharger le contenue du repo. (Merci a Quantum-cross pour le code) 

Ouvrir le code du projet : `File->Open->main/main.ino`

Appuyer sur le bouton reset de l'arduino

Puis compiler et uploader le code dans le Trinket : `Sketch->Verify/Compile`, `Sketch->Upload`

### Compiler avec un autre payload :

- Utiliser le tool dans le dossier `Payload2Header` pour convertir le payload en .h
- Deplacer le .h dans le dossier main et editer le fichier main.ino en remplacant `#include "ReiNX.h"` par le nom de votre payload.h

## Hardware

#### Preparation du Trinket M0 :

Desouder le port micro usb.
Dessouder la resistance comme sur la photo.

[PHOTO]

#### Preparation de la Switch :
Demonter la plaque arriere de la console.
Pour ca, il faut retirer les 2 railles pour les joycons, les 6 vis derriere la console et la vis au niveau de la micro SD

Puis enlever la plaque metalique.

Debrancher la batterie.




### Thank's too :

@noemu
