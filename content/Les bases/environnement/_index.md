+++
date = '2024-12-10T15:04:39+01:00'
draft = false
title = 'Environnement'
weight = 2
+++

## Choisir son environnement

N'importe quel éditeur de texte peut être utilisé pour coder en Python. Mais attention, on parle d'éditeur de texte, pas de "traitement de texte" (comme Word par exemple).

Voici quelques exemples :

- Sublime Text : très utilisé il y a quelques années mais nécessite une licence
- Visual Studio Code : de Microsoft, gratuit et assez léger, il permet de changer de version de Python rapidement.

Il existe également des environnements de développement complets (IDE) :

- Thonny (pour débutant) : facile à installer et multi-plateforme.
- PyCharm : payant mais il existe une version open source gratuite, c'est l'outil des professionnels mais il est assez lourd. A privilégier pour les grands projets.

Et aussi des outils inclassables très utilisés en data science :

- Jupyter notebook : ressemble à un bloc note et donne un aperçu de ce que l'on fait. Gratuit.
- Anaconda : rassemble des librairies pour Python et R, mais très lourd. Dédié à la data science.

## Conseil

Pour la suite de cette formation, je vais utiliser Visual Studio Code et Jupyter notebook. Je vous conseille de faire de même dans un premier temps.

## installation

### Windows

- Utiliser le site Python www.python.org, ne pas utiliser le Windows Store.
- Voir le bouton Download : toutes les versions avec leurs dates de support
- Choisir "executable installer" en x86 64 bits.
- Lancer l'installation :
  - cocher "inclure dans le PATH"
  - choisir Customize installation (évite les pbs de permission)
  - py(laucher) : permet de choisir la version de Python à utiliser
  - cocher "install for all users"
  - Dernière étape : Disable Path limit (cliquer dessus)

Pour vérifier :
- Lancer IDLE
- Ouvrir un invite de commande et taper Python (saisir exit() pour sortir)

Si pb, pour modifier les variables d'environnement : saisir "envir" dans la barre de recherche

Pour lancer une version particulière :
````py
py -3.12
````

### Mac

- ouvrir le terminal : saisir python puis TAB : affiche les versions installées
- installer la dernière version depuis le site www.python.org (faire l'installation par défaut)

## Le terminal

Le terminal = interface qui permet d'accéder au Shell (plusieurs disponibles : bash, Z-Shell(zsh))

Tout ce que l'on fait avec une interface graphique est faisable depuis un terminal. Dans certains cas, il n'y a pas d'alternative.

Le terminal est indispensable pour tout développeur qui se respecte pour plusieurs raisons :

- Exécuter des commandes sur des serveurs sans interface graphique
- Installer des utilitaires uniquement disponibles en ligne de commande
- Administrer plus facilement un environnement UNIX (très utilisé dans le monde du développement)

### Le cas de Windows

Windows utilise l'invite de commande comme Terminal pour passer des commandes DOS. Ces commandes sont différentes de celles utilisées sur les autres shells de Mac ou Linux.
Par ailleurs, les chemins d'accès sont différents.
Il est souvent plus simple de coder sous Mac oinsta Linux que Windows... (impossible de créer des dossers cachés, d'accéder à des serveurs distants en SSH (sauf à utiliser PuTTY, de gérer le versionning avec GIT, etc.)

Comment améliorer l'expérience sous Windows ? en installer un émulateur de Terminal comme par exemple WSL (windows subsystem Linux) présent par défaut depuis Windows 10 mais un peu lourd, CMDR (https://cmder.app), etc. Ou en utilisant PowerSHell

Mise à jour de PowerShell :
https://learn.microsoft.com/fr-fr/powershell/scripting/whats-new/migrating-from-windows-powershell-51-to-powershell-7?view=powershell-7.4

### Quelques commandes

- pwd : Print Working Directory
- cd : Change Directory
- ls : liste le contenu
- le dossier ~ (ALT + N)
- clear
- mkdir : make directory
- rm : remove
- touch (ni sur Windows)