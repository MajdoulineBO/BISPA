# BISPA
l’objectif principale était de concevoir et de mettre en œuvre, en situation réelle, une architecture d'un système complet de surveillance des personnes âgées intelligent, connecté et portatif sous forme d’un bracelet permettant le suivi continu de 
la santé des patients à distance ainsi que l’avertissement des personnes concernées (médecin, famille) via des notifications instantanées et indépendamment de l’endroit du patient. 

En fait, le principe consiste à acquérir d’abord le signal mesuré par l'accélérométre.

Ensuite ce signal va  être stocké en firebase toute en passant par une application mobile pour être deploiée ensuite dans notre modéle qui va prédire le résultat (chute ou non chute).

Il faut d'abord installer arduino IDE 
https://www.arduino.cc/en/Main/Software
Ajouter le code “send_data.ino” to Arduino
Compiler et téléverser le code sur Arduino.Dans notre cas nous avons utilisé (Arduino Nano)

![Alt text](BISPA/BISPA_ARDUINO/arduino_nano.jpg?raw=true "Title")

Installer android Studio 
https://developer.android.com/studio
Ouvrir Android Studio et ouvrir le projet nommé “BISPA”



Compiler et installer l’application sur un smartphone Android.
Ouvrir l’application et choisir le module Bluetooth pour se connecter, dans notre cas nous avons utilisé le module HC-05.


Utiliser Firebase comme une base de données temps réel pour le stockage de données. 
https://firebase.google.com/
Utiliser FCM pour l'envoi des notifications.

Utiliser Pythonanywhere pour héberger le code de prédiction.
https://www.pythonanywhere.com/
créer un nouveau compte
créer un environnement virtuel : connectez-vous à votre compte PythonAnywhere.

Héberger les fichiers de l’application de classification sur un répertoire dans le serveur en ligne PythonAnywhere (dict.mat, predict.py, utils.py, optimize.py, base.py)
Démarrer le fichier "prédict.py".
