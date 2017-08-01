### Image->Container: pull ubuntu image, then run and mount ~/repo to /root/repo

`sudo docker run -it -v ~/repo:/root/repo ubuntu /bin/bash`

### Detach

`ctrl-p+ctrl-q`

### Reattach

`docker attach CONTAINER_NAME`

### Start

`docker start CONTAINER_NAME`

### List containers

`docker ps`

### Commit container changes

`docker commit CONTAINER_NAME`

### Stop or kill container

``docker stop/kill CONTAINER NAME``

### Remove all docker containers

``docker rm `docker ps --no-trunc -aq` ``

### Remove a docker container

``docker rm CONTAINER_NAME``

### List last used container

``docker ps -l -q``

### Rename docker container
``docker rename CONTAINER NEW_NAME``

### Remove all dangling volumes
`docker volume rm $(docker volume ls -qf dangling=true)`

### List images
`docker images`

### Remove images
`docker rmi IMAGE_ID`

### Nvidia-docker
edit Dockerfile s.t. contains:
```
FROM nvidia/cuda:8.0-devel-ubuntu16.04
```
then run:
```
sudo docker build -t $IMAGE_NAME - < Dockerfile
sudo nvidia-docker run -it -v /home/gchu/mnt:/root/ $IMAGE_NAME /bin/bash
```


