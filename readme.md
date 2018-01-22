Docker for LNMP
===============

# What's in it
1. Mysql 5.7
2. PHP 7.2 with PHP-FPM
3. NGINX latest
4. PHPMYADMIN

# Steps
1. create a folder www/project.docker (.docker suffix is a MUST)
2. in Host append "127.0.0.1 project.docker" to /etc/hosts

# Some commands

## Build once
$ docker-composer build
## Start containers
$ docker-compose up -d
## Stop all containers
$ docker kill $(docker ps -q)
## View all containers
$ docker ps
## view nginx log (access & error)
$ docker logs -f [container-id]


# Others

1. Mysql Host name is "db"
2. PHPMYADMIN http://localhost:8082/
3. Your project http://project.docker/
4. Tweak PHP configuration in phpconf.ini
5. Add new PHP extension in Dockerfile-php and build

