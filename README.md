# API REST Projet scolaire Java

Le projet est une API REST développée avec Spring Boot pour la réalisation d'un projet 
scolaire.

Ici, le sujet est de faire une API qui possède les CRUD pour chacun des objets.

Le contexte est une entreprise que différents utilisateurs peuvent se connecter et 
s'inscrire à l'application, particulier, club de sport, association ou entreprise. 
Ici, la connexion et l'inscription ne sont pas abordées.

Chaque utilisateur, peut à la fois retrouver des lieux pour pratiquer son sport mécanique,
mais aussi en rechercher à l'aide de filtres comme le choix du sport mécanique ou la difficulté.

Aussi, il est possible de retrouver des événements avec les mêmes possibilités de filtres. 
Chaque événement possède des catégories pour pouvoir s'y inscrire en fonction de sa date 
de naissance. (Exemple: benjamin, cadet, senior, etc.)

## Installation

Pour installer le projet avec Git.

```bash
  git clone https://github.com/c-bringer/API-REST-Projet-scolaire-Java.git
  cd API-REST-Projet-scolaire-Java
```

## Variables d'environnement

Pour lancer le projet, il faut penser en premier à modifier les données de connexion à la base de données.

```bash
  spring.datasource.url=jdbc:mysql://localhost:3306/sportingo
  spring.datasource.username=root
  spring.datasource.password=root
```

## Lancer le projet

Après avoir cloné et se positionner dans le répertoire du projet.

Installer les dépendances Maven.

Lancer le serveur.

## Concepts étudiés

Dans ce projet, j'ai appris à développer une API REST en respectant le model, repository, service et controller.

Ici, je n'ai donc pas mis en place la partie vue que nous avons pu aborder en cours.

## Support

Pour toute question, merci de me contacter à corentin.bringer@limayrac.fr.
