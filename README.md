# PHP8_fpm_nginx

Docker set up for PHP 8.2 (fpm) + nginx server

## 1. What you will get

- PHP 8.2
  - pdo_mysql
- nginx server
- docker compose set up

## 2. How and where to start

### Add sources
Copy your sources to directory ./src \

### SQL db initialisation
Add startup script(s) for SQL to dir ./docker/mysql/dump/

### Start/stop container
To start:
```
$ docker compose -f ./docker/docker-compose.yaml up -d
```
To stop:
```
$ docker compose -f ./docker/docker-compose.yaml down
```

## 3. Project Structure
```
./docker // docker setup

./src/ // sources directory. Add your app sources here

```

## 4. Hostnames

See docker-compose.yaml

### PHP container
phpfpm

### nginx container
nginx

### mysql
database

## 5. Urls

#### App url
http://localhost:8080

## 6. Network
This docker compose setup creates a network with name 'app_network' for included containers.