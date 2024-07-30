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

