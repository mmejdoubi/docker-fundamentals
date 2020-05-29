# docker-fundamentals-path

## vauables resources:
- Introduction to Containers, VMs and Docker: a good article from medium, https://medium.com/free-code-camp/a-beginner-friendly-introduction-to-containers-vms-and-docker-79a9e3e119b

## What is docker ?
- Docker is a platform to build, run and share applications within containers. The use of containers to deploy applications is called containerisation. A container isolate the application and its dependencies from the host and from other applications.

## Image and Containers
## Why docker ?

## Docker commands
- To print the docker version: ```docker --version```
- To get information about the docker engine: ```docker info```, the printed info like running/stopped containers, images, volumes...
- To get information about specific docker command: ```docker commandName --help```, ```docker images --help``` will display info about the ```docker images``` command and how to use it.
- To list docker images: ```docker images``` or ```docker image ls```
- To list docker containers: ```docker ps```, this command will list only the running containers. to list all containers, ```docker ps -a```, so stopped containers will also be displayed.
- To pull an image from the default repisotory: ```docker pull imageName```
- To run a container from an image: ```docker run imageName```, if the image exists localy, the docker engine will create/start the container, otherwise, the image will be downloaded from the default repository and a new container will be created and started.
- To run a container from an image in an interactive mode: ```docker run -it imageId```
- To log in to the docker hub using a username and a password: ```docker login```, after a succesful login, we can push images to the docker hub repositories.
- To remove an image from local repositories: ```docker rmi imageName``` or ```docker rmi imageId```. If the image is running in a container, ```docker rmi -f imageName```
- To push an image to the remote docker hub repository: a tag shoud be given to the specified image, ```docker tag imageId username/imagename:versionTag```, now the image could be pushed to the remote repository by  ```docker push username/imagename:versionTag```
- To start and stop a container: ```docker start containerId```, ```docker stop containerId```
- To get stats about running containers: ```docker stats``` show memory usage, cpu%, IO of the running containers.
- To check disq usage talken by containers, images, volumes: ```docker system df```
- To remove unused data, all stoped containers, dangling images: ```docker system prune```, dangling images means image not associated with a container.


