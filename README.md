# Pablo Huys

## Question 3

### a) Télécharger l'image Nginx version 1.27.5

```bash
docker pull nginx:1.27.5
```

### b) Lister les images Docker

```bash
docker images
```

### d) Servir Nginx avec un fichier local

```bash
docker run --name "web-serv" -p 8080:80 -v C:\Users\pablo\Desktop\docker-training\html:/usr/share/nginx/html -d fb39280b7b9e
```

> `-d fb39280b7b9e` correspond à l'identifiant de l'image `nginx:1.27.5`.

### e) Supprimer le conteneur

```bash
docker rm -f web-serv
```

### f) Utilisation de cp pour remplacer un fichier
```bash
docker run --name "web-serv" -p 8080:80 -d fb39280b7b9e
```
```bash
docker cp C:\Users\pablo\Desktop\docker-training\html web-serv:/usr/share/nginx/
```

> Cette commande remplace le dossier `html` par votre version locale.

## Question 4

### a)
