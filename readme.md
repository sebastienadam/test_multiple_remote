# Publication sur différents dépôts

## Introduction

Voici un petit test que j'ai fait pour publier un même projet sur FramaGit et GitHub.

## Procédure

Voici comment je m'y suis pris:

* Création du projet sur [FramaGit](https://framagit.org/): https://framagit.org/sebastienadam/test_multiple_remote
* Création du projet sur [GitHub](https://github.com/): https://github.com/sebastienadam/test_multiple_remote
* Création du projet en local:

````
$ git clone https://framagit.org/sebastienadam/test_multiple_remote.git
$ cd test_multiple_remote/
````

* Ajout du dépôt GitHub:

````
$ git remote add github https://github.com/sebastienadam/test_multiple_remote.git
````

* Vérification de la configuration des dépôts distants:

````
$ git remote
github
origin
````

* Création d'un fichier de test.
* Publication du fichier:

````
$ git add --all
$ git commit -m "<message>"
$ git push origin master
$ git push github master
````
 Maintenant, la publication sur FramaGit se fait avec `git push` (c'est le dépôt par défaut) et la publication du GitLab se fait avec `git push github`.