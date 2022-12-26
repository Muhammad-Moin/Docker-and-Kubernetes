Docker has two components:
1- Docker client
2- Docker daemon
Docker image is as an object that contains an OS file system and an application.

*	Container is a stop version of images.
*	If you are a developer you can think of an image as a class.

								find version
1- docker version

								find how many images 
2- docker images or docker image ls

								find how many contaniers are run or  #show list of docker container
3- docker container ls or docker ps // or docker ps -a (-a used for additional information )
   			or
   docker container ls

								stop the containers
6- docker stop (id) i.e docker stop 93434a03cd2

								start the containers
7- docker start(id) i.e docker start 93434a03cd2


								Go back to running container shell
8- docker exec -it 93434a03cd2 (may be name or id)

	Removing the container so it must be in stop mode if container is not stop so first stop the container and then remove.
9- docker rm (id) i.e docker rm 93434a03cd2
			or
   docker rm alpine:latest
			and
   docker container rm 93434a03cd2

								pull the image from the docker hub
10- docker pull ameenalam/static-web
			or
   docker image pull alpine:latest	

								run the web container in browser
11- docker run --name=web1 -p 3000:80 -d ameenalam/static-web
			or
    docker run -it aamirpinger/helloworld sh (iterative mode pull the image if not find on local machine and create a container and run it)

Examples:
docker run --name=web2 -p 4000:80 -d nginx:latest (-d stand for detech mean run the container and it will automatically run on backgroung)
docker run --name=web3 -p 4000:80 -d mystaticapp:v1

#build the images from the Dockerfile
12- docker build -t mystaticapp:v1 .


*	if you want to run a container in background so press (ctrl PQ)
