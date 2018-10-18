# docker-angular-node-v10-5

Docker local development environment for Angular - tested with Windows10 and Ubuntu 1804 

1- clone this repository

    git clone git@github.com:sys0dm1n/docker-angular-node-v10-5.git

2- got to the www folder and clone your frontend project

Replace the repository URL by your project's URL. Make sure the folder created in www is called yourproject or you'll have to update the Dockerfile-node accordingly.

    cd www
    git clone git@github.com:<user-name>/yourproject.git yourproject

## verbose mode, pull images and build container if any

Make sure **your path** is where your **docker-compose.yml** file is to run the docker-compose commands

    $ cd /some/path/docker-angular-node-v10-5/
    $ docker-compose up
    $ cd /some/path/docker-angular-node-v10-5/www/yourproject/
    $ npm install

## deamon mode, pull images and build containers if any

    $ docker-compose up -d

##  start conatiners

    $ docker-compose start

## stop containers

    $ docker-compose stop

## stop and delete containers

    $ docker-compose -s rm

## list running container

    $ docker ps 

## list all containers

    $ docker ps -a

## enter inside the container

    $ docker exec -it <container-name-or_container-ID> -f bash

## logs

    $ docker logs  <container-name-or.container-ID> -f
