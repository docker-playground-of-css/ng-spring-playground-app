
# Projet pour construire le système front et back

## Objectifs

L'objectif de ce dépôt est de faire communiquer le front avec le back ! Les deux projets étant sur des dépôts GitHub différents.

## Dépots relatifs

- [Backend : java-playground-of-css/Todo-REST-API-Spring-Boot](https://github.com/java-playground-of-css/Todo-REST-API-Spring-Boot)
- [Frontend : js-playground-of-css/ng-playground-app](https://github.com/js-playground-of-css/ng-playground-app)

## Déployer

Nécessite Docker.

### Initialement

```
docker-compose up --build
```

### En cas de changement du back ou du front

#### Arrêter les conteneurs

```
docker-compose down
```

#### Reconstruire l'image

```
docker-compose build --no-cache
```

Remarque : détruit la base de données (en l'état actuel) !

#### Mettre en route les conteneurs

```
docker-compose up --force-recreate -d
```

## Détail technique

### Frontend

- Réalisé en **Angular 19**

### Backend

- Réalisé en **Java 11** avec **Spring Boot**

### Base de données

- **MySQL**
