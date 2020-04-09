# Docker Commands

## To check docker version

	docker version

## To check number of running docker containers

	docker ps
	docker container ls -a

## To check number of images

	docker images

## To run a container

	docker run image

## To stop a running container

	ctrl + c

## To remove cotainer

	docker rm container_id | container_name

## |To remove images

	docker rmi image_name:tag

## To pull an image

	docker pull image

## To run a container from image with custom name "webapp"

	docker run --name webapp nginx

## To run a container in particular port & creating a local volume

	docker run -p "80:80" -v ${PWD}/app:/app mattrayner/lamp:latest-1804

## To run ssh in docker container

	docker exec -it <container name> /bin/bash

## To start an exited container with previous data

	docker start container_id
	docker attach container_id

	OR

	docker container start -a container_id