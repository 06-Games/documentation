---
title: Configuration
description: La configuration du serveur
published: true
date: 2019-07-21T15:17:01.896Z
tags: 
---

> Les fichiers de configuration sont créer après le premier lancement du serveur, merci de ne pas le créer avant ce premier démarrage afin d'éviter tout problème de compatibilité entre les versions du serveur
{.is-info}


# Le fichier config.ini
Ce fichier contient tout les paramètres principaux du serveur :
| Propriété                	| Valeurs acceptées         	| Valeur par defaut 	| Description |
|--------------------------	|---------------------------	|-------------------	|-------------------	|
|                          	|         <span style="display: flex; justify-content: center; align-items: center;">**Server**</span>        	|                   	|                   	|
| server.create_log        	| False/True                	| True              	| Le serveur doit créer des fichiers [logs](#le-dossier-log) ? |
| server.icon              	| Chaine de charctère 	| icon.png          	| Le chemin d'accès vers l'icone du serveur |
| <span>server.name</span> 	| Chaine de charctère            	| Angry Dash Server 	| Le nom du serveur |
| server.port              	| 1-65535                   	| 20000             	| Le port d'écoute du serveur |
|                          	|        <span style="display: flex; justify-content: center; align-items: center;">**Players**</span>        	|                   	|                   	|
| players.limit            	| 1-Infini (ou presque)     	| 50                	| Le nombre maximum de connections simultanées |
|                          	|          <span style="display: flex; justify-content: center; align-items: center;">**Map**</span>          	|                   	|                   	|
| map.reload_for_players   	| False/True                	| True              	| Lors de l'exucution de la commande `reload`, la carte doit être rechargée par les joueurs déjà connecté ? |

# Le fichier map.level
Ce fichier contient la map du serveur, il peut être remplacé par n'importe quel map créée dans Angry Dash

# Le dossier log
Ce dossier contient tout les fichiers logs du serveur (sauf si ceux-ci sont désactivé dans le fichier de configuration). Ces fichiers permettent de garder la trace de vos actions, de se qu'il se passe sur le serveur et des erreurs rencontrées. Ils sont nécessaires pour effectuer un rapport de bug.