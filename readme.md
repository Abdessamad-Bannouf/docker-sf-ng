
# Symfony 6 + PHP 8.0.13 avec Docker
# Angular dernière version

**SEULEMENT pour l'environnement de DEV, pas pour la production**

Docker avec Symfony 6 & PHP 8.0.13
Docker avec Angular dernière version

## Lancer localement

Lancer la commande docker-compose

```bash
  docker-compose up -d
```


Pour se connecter au containeur Symfony
```bash
  docker exec -it sf bash
```


Pour se connecter au containeur Angular
```bash
  docker exec -it ng bash
```


*l'application est disponible à l'adresse: http://127.0.0.1:4300*

*Pour le back, aller à l'adresse: http://127.0.0.1:9000*

*Pour le PHPMyadmin, il faut se rendre sur l'adresse: http://127.0.0.1:8080* 

Si il y a besoin de la base de données, il faut modifier le fichier .env comme cet exemple:

```yaml
  DATABASE_URL="postgresql://symfony:ChangeMe@database:5432/app?serverVersion=13&charset=utf8"
```

## Prêt à être utilisé avec

This docker-compose fournit :

- PHP-8.0.13-cli (Debian)
    - Composer
    - Symfony CLI
    - NodeJS, NPM, YARN
- postgres:13-alpine
- Node / Angular dernière version
