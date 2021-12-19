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

## Documentation de référence de l’API

#### Enregistre un nouveau utilisateur

```http
  POST /user
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `user` | `User` | **Obligatoire**. Object User à envoyer |

#### Retourne la liste de tous les utilisateurs

```http
  GET /user
```

#### Retourne un utilisateur en fonction de l'id

```http
  GET /user/{id}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `id` | **Obligatoire**. Id de l'utilisateur à retourner |

#### Mets à jour un utilisateur en fonction de l'id

```http
  PUT /user/{id}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `id` | **Obligatoire**. Id de l'utilisateur à modifier |
| `user` | `User` | **Obligatoire**. Object User à envoyer | 

#### Suprime un utilisateur en fonction de l'id

```http
  DELETE /user/{id}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `id` | **Obligatoire**. Id de l'utilisateur à supprimer |

#### Enregistre une nouvelle entreprise

```http
  POST /user-company
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `userCompany` | `UserCompany` | **Obligatoire**. Object UserCompany à envoyer |

#### Retourne la liste des entreprises

```http
  GET /user-company
```

#### Retourne une entreprise en fonction de l'id

```http
  GET /user-company/{id}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `id` | **Obligatoire**. Id de l'entreprise à retourner |

#### Mets à jour une entreprise en fonction de l'id

```http
  PUT /user-company/{id}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `id` | **Obligatoire**. Id de l'entreprise à modifier |
| `userCompany` | `UserCompany` | **Obligatoire**. Object UserCompany à envoyer | 

#### Supprime une entreprise en fonction de l'id

```http
  DELETE /user-company/{id}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `id` | **Obligatoire**. Id de l'entreprise à supprimer |

#### Enregistre un nouveau club

```http
  POST /user-club
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `userClub` | `UserClub` | **Obligatoire**. Object UserClub à envoyer |

#### Retourne la liste des clubs

```http
  GET /user-club
```

#### Retourne un club en fonction de l'id

```http
  GET /user-club/{id}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `id` | **Obligatoire**. Id du club à retourner |

#### Mets à jour un club en fonction de l'id

```http
  PUT /user-club/{id}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `id` | **Obligatoire**. Id du club à modifier |
| `userClub` | `UserClub` | **Obligatoire**. Object UserClub à envoyer | 

#### Supprime un club en fonction de l'id

```http
  DELETE /user-club/{id}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `id` | **Obligatoire**. Id du club à supprimer |

#### Enregistre une nouvelle association

```http
  POST /user-association
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `userAssociation` | `UserAssociation` | **Obligatoire**. Object UserAssociation à envoyer |

#### Retourne la liste des associations

```http
  GET /user-association
```

#### Retourne une association en fonction de l'id

```http
  GET /user-association/{id}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `id` | **Obligatoire**. Id de l'association à retourner |

#### Mets à jour une association en fonction de l'id

```http
  PUT /user-association/{id}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `id` | **Obligatoire**. Id de l'association à modifier |
| `userAssociation` | `UserAssociation` | **Obligatoire**. Object UserAssociation à envoyer | 

#### Supprime une association en fonction de l'id

```http
  DELETE /user-association/{id}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `id` | **Obligatoire**. Id de l'association à supprimer |

#### Enregistre un nouveau spot

```http
  POST /spot
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `spot` | `Spot` | **Obligatoire**. Object Spot à envoyer |

#### Retourne la liste des spots

```http
  GET /spot
```

#### Retourne un spot en fonction de l'id

```http
  GET /spot/{id}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `id` | **Obligatoire**. Id du spot à retourner |

#### Mets à jour un spot en fonction de l'id

```http
  PUT /spot/{id}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `id` | **Obligatoire**. Id du spot à modifier |
| `spot` | `Spot` | **Obligatoire**. Object Spot à envoyer | 

#### Supprime une association en fonction de l'id

```http
  DELETE /spot/{id}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `id` | **Obligatoire**. Id du spot à supprimer |

#### Enregistre un nouveau sport mécanique

```http
  POST /admin/mechanical-sport
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `mechanicalSport` | `MechanicalSport` | **Obligatoire**. Object MechanicalSport à envoyer |

#### Retourne la liste des sports mécaniques

```http
  GET /mechanical-sport
```

#### Retourne un sport mécanique en fonction de l'id

```http
  GET /mechanical-sport/{id}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `id` | **Obligatoire**. Id du sport mécanique à retourner |

#### Mets à jour un sport mécanique en fonction de l'id

```http
  PUT /admin/mechanical-sport/{id}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `id` | **Obligatoire**. Id du sport mécanique à modifier |
| `mechanicalSport` | `MechanicalSport` | **Obligatoire**. Object MechanicalSport à envoyer | 

#### Supprime un sport mécanique en fonction de l'id

```http
  DELETE /admin/mechanical-sport/{id}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `id` | **Obligatoire**. Id du sport mécanique à supprimer |

#### Enregistre une nouvelle difficulté

```http
  POST /admin/difficulty
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `difficulty` | `Difficulty` | **Obligatoire**. Object Difficulty à envoyer |

#### Retourne la liste des difficultés

```http
  GET /difficulty
```

#### Retourne une difficulté en fonction de l'id

```http
  GET /difficulty/{id}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `id` | **Obligatoire**. Id de la difficulté à retourner |

#### Mets à jour une difficulté en fonction de l'id

```http
  PUT /admin/difficulty/{id}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `id` | **Obligatoire**. Id de la difficulté à modifier |
| `difficulty` | `Difficulty` | **Obligatoire**. Object Difficulty à envoyer | 

#### Supprime une difficulté en fonction de l'id

```http
  DELETE /admin/difficulty/{id}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `id` | **Obligatoire**. Id de la difficulté à supprimer |

#### Enregistre une nouvelle catégorie

```http
  POST /admin/category
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `category` | `Category` | **Obligatoire**. Object Category à envoyer |

#### Retourne la liste des catégories

```http
  GET /category
```

#### Retourne une catégorie en fonction de l'id

```http
  GET /category/{id}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `id` | **Obligatoire**. Id de la catégorie à retourner |

#### Mets à jour une catégorie en fonction de l'id

```http
  PUT /admin/category/{id}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `id` | **Obligatoire**. Id de la catégorie à modifier |
| `category` | `Category` | **Obligatoire**. Object Category à envoyer | 

#### Supprime une catégorie en fonction de l'id

```http
  DELETE /admin/category/{id}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `id` | **Obligatoire**. Id de la catégorie à supprimer |

#### Enregistre une nouvelle inscription

```http
  POST /user-registration
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `userRegistration` | `UserRegistration` | **Obligatoire**. Object UserRegistration à envoyer |

#### Retourne la liste des inscriptions

```http
  GET /user-registration
```

#### Retourne une inscription en fonction de l'id

```http
  GET /user-registration/{id}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `id` | **Obligatoire**. Id de l'inscription à retourner |

#### Mets à jour une inscription en fonction de l'id

```http
  PUT /user-registration/{id}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `id` | **Obligatoire**. Id de l'inscription à modifier |
| `userRegistration` | `UserRegistration` | **Obligatoire**. Object UserRegistration à envoyer | 

#### Supprime une inscription en fonction de l'id

```http
  DELETE /user-registration/{id}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `id` | **Obligatoire**. Id de l'inscription à supprimer |

#### Enregistre un nouvel événement

```http
  POST /event
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `event` | `Event` | **Obligatoire**. Object Event à envoyer |

#### Retourne la liste des événements

```http
  GET /event
```

#### Retourne un événement en fonction de l'id

```http
  GET /event/{id}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `id` | **Obligatoire**. Id de l'événment à retourner |

#### Mets à jour un événement en fonction de l'id

```http
  PUT /event/{id}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `id` | **Obligatoire**. Id de l'événement à modifier |
| `event` | `Event` | **Obligatoire**. Object Event à envoyer | 

#### Supprime un événement en fonction de l'id

```http
  DELETE /event/{id}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `id` | **Obligatoire**. Id de l'événement à supprimer |

## Concepts étudiés

Dans ce projet, j'ai appris à développer une API REST en respectant le model, repository, service et controller.

Ici, je n'ai donc pas mis en place la partie vue que nous avons pu aborder en cours.

## Support

Pour toute question, merci de me contacter à corentin.bringer@limayrac.fr.
