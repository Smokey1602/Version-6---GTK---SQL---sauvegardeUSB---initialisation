Bonjour,

Ce répertoire regroupe la version 6 du compteur. Cette version n'influence en rien le traitement video. Elle ajoute simplement la sauvegarde
sur clef USB grace a l'appui d'un bouton

Il garde les options de base:

  - Sauvegarde automatique toutes les minutes
  - Sauvegarde sous dans une BDD
  - Création et sauvegarde d'un graphique
  - Interface graphique grace a opencv
  - Traitement video
  - Comptage
  
  
Et ajoute :

  - sauvegarde sur clef USB sur appui d'un bouton

Il suffit de compiler le fichier "camera.c" sous linux avec la librairie openCV pour essayer le programme 
g++ -Wall -pthread -o camerapio camera.c -lpigpio -lrt ` pkg-config --cflags --libs opencv gtk+-2.0` `mysql_config --cflags --libs` 

Faites attention que la clef USB soit bien branchée et qu'elle porte le nom ONEBEE avant d'effectuer la sauvegarde sur cette derniere. 
