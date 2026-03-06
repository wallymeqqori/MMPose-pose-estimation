# PROJET MIDL 2 - MMPOSE

MEQQORI Wally - DE PAIVA Stefan - CUTAYA Julian
## Description
• Découvrir et manipuler une librairie de vision par ordinateur de l’écosystème OpenMMLab.

• Réaliser une analyse de trajectoire à partir de vidéos (ex. mouvement humain, sportif, animal…).

• Concevoir un modèle de prédiction de trajectoire, en apprentissage supervisé ou par apprentissage par renforcement (RL).

## Objectifs
- Exploitation de mouvements semi-complexes, comme des mouvements sportifs


# MMPose-pose-estimation
L’objectif principal est de concevoir un système de vision par ordinateur capable d’analyser des mouvements humains et de prédire leurs trajectoires futures. Nous avons utilisé la librairie MMPose pour l’extraction de points clés squelettiques et un réseau de neurones récurrents de type LSTM pour la modélisation temporelle et la prédiction.

Voici un exemple :


<img src="main_large.gif" width="600">

Il suffit de déposer une vidéo de type .mp4, .avi, .mov ou .mkv dans le dossier du notebook pour produire deux gifs, un calculant le barycentre, "barycentre.gif" et l'autre faisant une détection de keypoints "pose2d.gif" ( ici les articulations principales du corps humain et les caractéristiques principales du visage ).

Le temps d'exécution est proportionnel à la longueur de la vidéo, variant entre 5 et 15 minutes.

Il y a en plus de cela des fichiers .csv qui sont générés sur les positions x et y du barycentre ainsi que de chaque keypoints, ce qui sera nécessaire pour la partie prévisionnelle ML/RL.

