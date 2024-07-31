What is Docker and its uses?

Docker is a software platform that allows you to build, test, and deploy applications quickly.

Docker packages software into standardized units called containers that have everything the software needs to run including libraries, system tools, code, and runtime.

Docker makes the packaging process easier and lets developers ship their apps as a single package. 

Docker was made by Solomon Hykes In 2013.

Docker Containers are a standardized unit of software that allows developers to isolate their app from its environment, solving the “it works on my machine” headache.

Basic commands used in Docker are. :

* docker built -t imagename . --> To build a docker image in the current direcotry must use the ( . ) after the image name .
* docker run -d --name containername -p 8080:80 image_name --> To run a docker container in background ( -d to detach from the terminal to work at background and -- name to assign a container name and -p to specify a port number) .
* docker ps / ps -a --> To list out working containers ( ps ) , To list out all non and working containers ( ps -a ) .
* docker system prune -a --> To remove all unused images (not just dangling ones), containers, networks, and optionally volumes , You can use -a -f options along with this command to remove everythings without and confirmation .

Docker image commands :
* docker image ls --> To list out images .
* docker image prune --> To remove dangling or untagged images assosiated with the containers .
* docker pull image_name:tag --> To pull image from docker hub .
* docker rmi image_id --> To remove an image .
* docker rmi -f my_image:latest --> To remove images from a container even if it still running .
* docker rmi -f image1 image2 image3 --> To remove multiple images .

Docker container commands :
* docker run options image_name:tag --> To run a container .
* docker start container_id --> To satrt a stopped container .
* docker stop container_id --> To stop a container .
* docker exec -it container_id command --> To execute a command in a running container .
* docker inspect container_id_or_name --> To inspect a container .
* docker rm container_id --> To remove a container .
* docker rm -f container_name --> To remove a running cotainer forcefully .
* docker logs container_id --> To see logs of a container .
* docker container prune --> To remove stopped containers which are not in use .

Docker volume commands :
* docker system prune -a --volumes --> To include unused volumes in the cleanup .
* docker volume create vol-name --> To create volume .
* docker volume ls --> To list out volumes .
* docker volume inspect vol-name --> To inspect a volume .
* docker volume rm vol-name --> To delete volume .

Docker network commands :
* docker network ls --> To list out the networks .
* docker network inspect network_name --> To inspect a network .
* docker network create network-name --> To create network .
* docker network rm network-name --> To remove network .
* docker network connect network-name container-name --> To connect a netwrok into a container .
* docker network disconnect network-name container name --> To disconnect a network into a container .
* docker network prune --> To remove all unused networks .
