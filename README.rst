.. Hearkinator documentation master file, created by
   sphinx-quickstart on Fri Jun  3 22:00:14 2016.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Documentation pour le bot Hearkinator
=======================================
Objectifs du projet
=======================================
Hearkinator est un robot slack développé avec le langage de programmation Python.
Le robot est inspiré du célèbre Génie Akinator http://fr.akinator.com/ mais le mécanisme diffère.

En effet, Hearkinator se joue à deux. Un joueur (user) cherche un challenger pour une partie. Le but est de trouver le 
personnage auquel pense l'un des joueur. Le joueur qui lance la partie et qui demande le challenge doit répondre par oui
ou par non aux question du challenger qui essaie de trouver le personnage. Une fois que le challenger trouve le personnage,
le nombre de tentative est indiqué par le robot et invite le challenger a lancer une partie à son tour. A la fin de la partie
le bot indique le meilleur des deux joueur.



.. toctree::
   :maxdepth: 2



Installation de HearKinator
=============================
Pour installer Hearkinator, suivre les instructions ci-dessous:

* Créer un dossier (mkdir nom_dossier)
* Entrer la commande: python -m venv . (Attention un espace entre venv et le point). Cette commande va installer l'environnement virtuel.
* Entrer la commande: Scripts\\activate.bat
* Entrer la commande suivante dans l'environnement crée: pip install hearkinator
* Entrer la commande: pip install aiohttp
* Entrer la commande: pip install websockets (Attention n'oubliez par le s car il existe aussi un websocket sans le s)
* Entrer la commande: pip install slackclient

A ce niveau le robot est prèt au lancement.

Où trouver hearkinator après installation
==========================================

Après l'installation du robot, suivre le chemin:
   Lib/site-packages/hearkinator/akinator_bot.py
   

Lancer le robot
==========================================

Toujours dans le repertoire crée, faire:

* set SLACK_TOKEN = <valeur du tocken ici>
* puis lancer la commande python Lib/site-packages/hearkinator/akinator_bot.py
* Se connecter à slack et là on trouve le bot hearkinator.
