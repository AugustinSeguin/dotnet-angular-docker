# Lancer le projet avec Docker

## API en dotnet

Assurez-vous d’avoir Docker et Docker Compose installés.

Les services : 
- une web API en .NET 8.0
- une BDD Postgresql

### Lancer les services

```bash
docker-compose up --build -d
```

### Down les services

```bash
docker-compose down -v
```

### Entrer dans un container 

```bash
docker ps -a
```

Récupérer l'id du container

```bash
docker exec -it CONTAINER_ID /bin/sh
```

[App back accessible](http://localhost:5000/swagger/index.html)
 
[App front accessible ici](http://localhost:4200/browser/)

## DevContainer

Ce projet est compatible avec l’environnement de développement Dev Containers de VS Code, permettant de travailler dans un environnement préconfiguré incluant .NET, Angular et PostgreSQL.

**Prérequis**
- Visual Studio Code
- L’extension "Dev Containers" installée (Remote - Containers)
- Docker installé et en cours d'exécution
- Démarrer avec le Dev Container
- Ouvre ce dossier dans VS Code.

Palette de commande > **Reopen in Container**

Utiliser le fichier compose.yaml pour lancer les services (api, db, front)

Ouvrir un shell dans le container du service api

Installer automatiquement les dépendances et extensions définies dans .devcontainer/devcontainer.json

