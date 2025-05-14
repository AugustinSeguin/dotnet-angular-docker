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

## App Angular

### Build app

```bash
docker build -t mon-app-angular .
```


### Run app

```bash
docker run -d --name mon-app-angular mon-app-angular
```
