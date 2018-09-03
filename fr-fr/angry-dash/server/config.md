<!-- TITLE: Configuration -->
<!-- SUBTITLE: La configuration du serveur -->

**Note :** les fichiers de configuration sont créer après le premier lancement du serveur, merci de ne pas le créer avant ce premier démarrage afin d'éviter tout problème de compatibilité entre les versions du serveur

# Le fichier config.ini
Ce fichier contient tout les paramètres principaux du serveur :
| Propriété                	| Valeurs acceptées         	| Valeur par defaut 	|
|--------------------------	|---------------------------	|-------------------	|
|                          	|         <span style="display: flex; justify-content: center; align-items: center;">**Server**</span>        	|                   	|
| server.create_log        	| False/True                	| True              	|
| server.icon              	| Nom du fichier de l'icone 	| icon.png          	|
| <span>server.name</span> 	| Nom du serveur            	| Angry Dash Server 	|
| server.port              	| 1-65535                   	| 20000             	|
|                          	|        <span style="display: flex; justify-content: center; align-items: center;">**Players**</span>        	|                   	|
| players.limit            	| 1-Infini (ou presque)     	| 50                	|
|                          	|          <span style="display: flex; justify-content: center; align-items: center;">**Map**</span>          	|                   	|
| map.reload_for_players   	| False/True                	| True              	|

# Le fichier map.level
Ce fichier contient la map du serveur, il peut être remplacé par n'importe quel map créer dans Angry Dash

# Le dossier log
Ce dossier contient tout les fichiers logs du serveur (sauf si ceux-ci sont désactivé dans le fichier de configuration). Ces fichiers permettent de garder la trace de vos actions, de se qu'il se passe sur le serveur et des erreurs rencontrées. Ils sont nécessaires pour effectuer un rapport de bug.