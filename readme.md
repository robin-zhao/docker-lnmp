Docker for LNMP
===============

# Build once
$ docker-composer build

# Start containers
$ docker-compose up -d

# Stop all containers
$ docker kill $(docker ps -q)

# View all containers
$ docker ps

# view nginx log (access & error)
$ docker logs -f [container-id]


