Docker for LNMP
===============

# What's in it
1. Mysql 5.7
2. PHP 7.2 with PHP-FPM
3. NGINX latest
4. PHPMYADMIN

# Steps
1. create a folder www/project.docker (.docker suffix is a MUST)
2. in Host add "127.0.0.1 project.docker" to /etc/hosts

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


