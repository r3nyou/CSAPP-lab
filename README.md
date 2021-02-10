# Computer Systems: A Programmer's Perspective, 3/E (CS:APP3e)
download from [Lab Assignmests](http://csapp.cs.cmu.edu/3e/labs.html)

## lab env
### prerequisite
- docker

pull image
```
docker pull ubuntu
```
run a new container
```
docker container run -it -v /path_to/csapp/:/csapp --name=csapp_env ubuntu /bin/bash
```
install 
```
apt-get update
apt-get install sudo
sudo apt-get install build-essential
sudo apt-get install gcc-multilib
sudo apt-get install gdb
```
restart the container
```
docker container start csapp_env
```
Run bash in a running container
```
docker container exec -it csapp_env /bin/bash
```
Exiting a Docker Container
```
exit
```
Kill running containers
```
docker container kill csapp_env
```