# LAMP Stack
Personnal LAMP stack with Docker for local projects

## Dependencies
- Docker
- Docker compose
- Images
  - php:5-apache
  - mysql
  - mailhog
  - phpmyadmin/phpmyadmin

## Build image `chymz/php-apache`
Run `images/php-apache/build.sh`

## Start webserver containers
```shell
docker-compose up -d
```
Webserver `http://localhost:9000`

PhpMyAdmin : `http://localhost:9001`

Mailhog : `http://localhost:9002`


## Stop containers
```shell
docker-compose stop
```
## Configurations
- `conf/php.ini` : PHP configuration file
- `conf/mysql.cnf` : MySQL configuration file
- `conf/php.ini` : Apache configuration file
- `conf/sites` : Apache virtual hosts
