# wordpress-docker-simple

A simple docker environment for a wordpress application.

This configuration is using the following images from [DockerHub](https://hub.docker.com/):
* __Wordpress__: wordpress:latest (official)
* __MariaDb__: mariadb:latest (official)

You can customize all the versions and packages in the *docker-compose.yaml* file, or in the */images/*.

## Quickstart
1. __Install__ [docker](https://docs.docker.com/install/)

2. __Wordpress__ Download latest [wordpress](https://de-at.wordpress.org/download/) to *your_wordpress_directory*

5. __Start:__ Build the docker containers
   ```
   # Move to directory which includes docker-compose.yml file
   docker-compose up -d
   ```

6. __DONE!__ open http://localhost:8000 and follow wordpress setup guide.


<br>


## Useful commands
```
# create and start containers without logging
docker-compose up -d
 
# create and start containers with log
docker-compose up
 
# stop and remove containers, networks, images, and volumes
docker-compose down
 
# step into the php container
docker-compose exec app bash
 
# step into the mysql container
docker-compose exec mysql bash
 
# list containers
docker-compose ps
 
# remove unused data
docker system prune
```
