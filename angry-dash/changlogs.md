---
title: Notes de version
description: La liste des changements effectués à chaque version
published: true
date: 2019-09-14T19:20:38.484Z
tags: 
---

# 0.4.x
## 0.4: Plus de libertés
> Cette mise à jour est encore au stade de pré-publication, les nouvelles fonctionnalités répertoriées ci-dessous sont sujettes à des changements drastiques.
{.is-info}
* <span style="font-size: 18px;">**Éditeur**</span>
  * Masquage automatique de la Toolbox
  * Les évènements sont rangés dans le menu build de l'éditeur
* <span style="font-size: 18px;">**Gameplay**</span>
  * Évènements programmables
      * Programmation visuelle et textuelle des évènements
      * Programmation en Lua, plus accessible que le C#
  * Début d'une API pour Angry Dash, plein d'actions disponibles, tels que:
      * Le changement de couleur
      * Faire perdre/gagner le niveau
      * La téléportation   
  * Groupes de blocs
  * De nouveaux blocs
* <span style="font-size: 18px;">**Autres changements**</span>
  * Avertissement de connexion à internet: un pop-up s'affiche lors d'un changement d'état de la connexion à internet
  * Dé-sélection des niveaux dans la liste des niveaux éditables
  * Support natif des processeurs 64 bits sur Android
  * **Bug fix:**  Les collisions fonctionnent correctement lorsque les textures ne font pas 100x100 pixels


# 0.3: La mise à jour solitaire
## 0.3: La personalisation
[![Download)](https://img.shields.io/badge/Download-0.3-blue.svg?style=flat-square)](https://github.com/06Games/Angry_Dash/releases/tag/2019.05.26)

* <span style="font-size: 18px;">**Interface**</span>
	* Refonte presque totale de l'interface
	* Ajout des Ressources Packs
		* Ils contiennent les textures et les musiques du jeu ainsi que les fichiers de langue
		* Les textures peuvent être animé grâce au support de la norme [APNG](https://developer.mozilla.org/fr/docs/Images_PNG_anim%C3%A9es)
		* Personalisation accrue des textures au travers de [configurations](https://next.json-generator.com/4J-tADUCH) dans des fichiers JSON du même ID
* <span style="font-size: 18px;">**Gameplay**</span>
  * Possibilité de mettre en pause un niveau joué en solo
  * Recompense à la fin d'un niveau officiel
  * Le joueur laisse un tracé derrière lui
  * Notation et commentaires des niveaux de la communauté
  * Paramétrage des niveaux
  	* Conditions de victoire: Nombre de lancés maximum, ...
    * Distance maximale par lancé
  * **Bug fix:** Les rebonds fonctionnent normalement
  * **Bug fix:** Les accélérations fonctionnent correctement
* <span style="font-size: 18px;">**Éditeur**</span>
	* Sauvegarde automatique
  * Affichage des coordonnées
  * Le retour dans l'éditeur après avoir testé un niveau est bien plus rapide
  * Les layers sont maintenant pleinement fonctionnels
  * **Bug fix:** la grille a été totalement repensé afin d'augmenter grandement les performances du jeu, fini les lags lors des mouvements !
* <span style="font-size: 18px;">**Autres changements**</span>
	* Notre mignifique logo s'affiche au démarrage du jeu
  * Ajout d'un menu debogage
  	* Affichage de Graphy avec des statistiques avancées sur les performaces du jeu
  	* Affichage des erreurs directement dans jeu
    * Affichage des coordonées dans le player de niveau
		*	Affichage de la config de l'appareil
  * Forte réduction de la taille de l'application
  * Optimisation des chargements
  * Support ARM64
  * Amélioration de la sécurité des comptes 06Games
	* Les niveaux sont maintenant en XML
  	* Plus faible impact sur les performances
    * Meilleur flexibilité (préparatifs pour le modding 😉)
    * Espace disque réduit

# 0.2.x: Un passage important
## 0.2.2: Les derniers ajutements
[![Download)](https://img.shields.io/badge/Download-0.2.2-blue.svg?style=flat-square)](https://github.com/06-Games/Angry-Dash/releases/tag/0.2.2)

* <span style="font-size: 18px;">**Editeur**</span>
	* **La trigger Move**
  	* Global Rotation : Possibilité d'effectuer une rotation en un seul bloc au lieu de chaque blocs indépendamment
  	* Le calcule du reset est plus fiable
		* Les translations en fonction du joueur fonctionnent correctement
		* Ajout de traductions manquantes
		* Optimisation
		* Le Move repose sur le temps écoulé au lieu d'un nombre d'image défini pouvant causer des problème en cas de chute de FPS
	* **Mais aussi...**
  	* Le déplacement Android n'est plus inversé
		* Les niveaux vides ne bloquent plus le jeu
		* Suppression des publicID

## 0.2.1: Une version pas si petite
[![Download)](https://img.shields.io/badge/Download-0.2.1-blue.svg?style=flat-square)](https://github.com/06-Games/Angry-Dash/releases/tag/0.2.1)
* <span style="font-size: 18px;">**Editeur**</span>
	* **Les triggers**, un nouvel évènement : le Move
		* Possiblité de déplacer des blocs ou la caméra
		* Possibilité d'effectuer des rotation des blocs ou de la caméra
		* Menu éditer différent pour chaque type de triggers/blocs
	* **Des niveau plus affirmés**
		* Vos niveau n'ont jamais été aussi complet : avec notre nouveau format de niveau, les possibilités sont infini
		* Des niveaux jamais obsolètes : avec notre système de mise à jour intelligente, vos niveaux seront toujours utilisable, même après plusieurs mise à jour
		* Les coordonées négatives ne nous font plus peur, vous pouvait dorénavant placer des blocs en coordonées négatives
	* **Un éditeur stable**
		* Avec cette version, adieu les décalage de blocs
		* La grille est maintenant parfaitement fonctionnel, elle va maintenant être votre meilleur ami
		* Vous pouvez dorénavant avoir un aperçu du bloc que vous éditez lorsque vous changez sa couleur
* <span style="font-size: 18px;">**Quelques optimisation**</span>
	* L'accès à l'éditeur est maintenant plus rapide
	* Un écran de chargement a été ajouté lors de l'édition d'un niveau
	* Les fichiers temporaires sont supprimés à la sortie du jeu
* <span style="font-size: 18px;">**Mais aussi ...**</span>
	* Les langues s'affichent directement lors de l'ouverture des paramètres
	* Le téléchargement des fichiers de langues est ignoré dans le cas où le fichier index n'existe pas
	* On peut de nouveau télécharger ses niveaux publiés
	* Correction d'une erreur survenant lors de la dé-sélection de tout les blocs
	* Les menus ne se changent plus dans l'éditeur quand on entre un nombre
	* La barre de progression refonctionne durant le téléchargement des niveaux officiels
	* On peut de nouveau ouvrir un niveau si le dossier Musics n'existe pas
	* Les niveaux supprimés ne sont plus affichés dans le menu récent

## 0.2: La grande version
[![Download)](https://img.shields.io/badge/Download-0.2-blue.svg?style=flat-square)](https://github.com/06-Games/Angry-Dash/releases/tag/0.2)
* <span style="font-size: 18px;">**Editeur**</span>
  * **Déplacement dans l'éditeur**
	  * <span style="font-family: Courier New; font-weight: bold;">PC :</span> Ajout d'un déplacement sur PC avec les touches : Flèche `droite`/`gauche`/`haut`/`bas`
    * <span style="font-family: Courier New; font-weight: bold;">Android :</span> Ajout d'un déplacement intuitif sur android, créer des niveaux n'a jamais été aussi facile désormé !
  * **Les Triggers**
    * Ajout des évènements (appelé Triggers) dans l'éditeur afin de pouvoir controler votre niveaux a volonté, comme par exemple le point de départ et d'arrivé.
  * **Grille**
    * Ajout d'une grille dans l'éditeur pour mieux savoir où sont nos blocs. Elle désactivable et réactivable en un clique en haut à droite grâce au bouton déstiné.
  * **Mode de réaparition**
    * Ajout de plusieurs mode de réaparition, cela permet de controler les différents points de réaparitions dans votre niveau. Vous pouvez choisir entre : Réaparaître à la dernière position, Réaparaître au dernier check point, ou Réaparaître au début du niveau.
  * **Musique**
    * Ajout des musiques dans les niveaux, pour en séléctionner une, aller dans options > musiques. Choisissez votre musiques parmit une liste, ou  rechercher l'artiste en question, ou le nom de la musique grâce à notre filtre.
  * **Publication de niveaux**
    * Ajout de la possibilité de publier vos propre niveaux au monde entier !
    * Et si vous voulez améliorer un de vos niveaux déjà publié, c'est aussi possible de le mettre à jour.
  * **Multi-Séléction**
	  * Ajout de la multiséléction dans l'éditeur, vous pouvez séléctionner plusieurs blocs pour changer leurs attributs ! Pratique.
  *  **Récent**
     * Ajout d'un menu récents, vous permettant de reprendre votre dernière activité là où vous l'avez laissé. 
* <span style="font-size: 18px;">**Menu Principal**</span>
  * **Options**
    * Ajout de nouvelles options, comme par exemple l'antialiasing, ou la suppression des fichiers logs.
  * **Profile**
    * Ajout du menu profile, il permet de gérer votre compte et vos niveaux (et vos amis, pas encore disponible :/)
  * **Inventaire**
    * Ajout de votre inventaire, c'est ici que vous pouvez personnaliser votre personnage etc...
  * **Boutique**
    * Cette boutique permet d'acheter des skins pour personnaliser votre personnage. Ammassez des pièces dans les niveaux du jeu ainsi que ceux en ligne (A venir). Attrapez-les toutes ! :)
* <span style="font-size: 18px;">**Jouer**</span>
  * **Niveaux Officiels**
    * Ajout des 10 premiers niveaux du jeu !
  * **Serveur** 
    * Ajout des serveurs, cela permet d'être plusieurs dans un même niveaux (voir la [section dédié](./#angry-dash-server))
    * Préparation à l'arrivé des serveurs officiels (ils ne sont malheureusement pas encore disponible :/)

# 0.1.x: Les préparatifs
## 0.1.3: Stabilisation
[![Download)](https://img.shields.io/badge/Download-0.1.3-blue.svg?style=flat-square)](https://github.com/06-Games/Angry-Dash/releases/tag/0.1.3)
* Corretion d'un bug avec les murs
* Recréation du menu accueil
* Support multi-résolution

## 0.1.2: Les murs
[![Download)](https://img.shields.io/badge/Download-0.1.2-blue.svg?style=flat-square)](https://github.com/06-Games/Angry-Dash/releases/tag/0.1.2)
* Ajout des murs
* Ajout d'une musique dans l'accueil

## 0.1.1: Le déplacement
[![Download)](https://img.shields.io/badge/Download-0.1.1-blue.svg?style=flat-square)](https://github.com/06-Games/Angry-Dash/releases/tag/0.1.1)
* Joystick invisible sur le player
* Remplacement des bandes blanches par des bandes noires

## 0.1: Première version
[![Download)](https://img.shields.io/badge/Download-0.1-blue.svg?style=flat-square)](https://github.com/06-Games/Angry-Dash/releases/tag/0.1)
* Version initiale