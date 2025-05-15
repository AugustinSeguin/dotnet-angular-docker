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

[App back accessible](http://localhost:5000/swagger/index.html)
 
[App front accessible ici](http://localhost:4200/browser/)

