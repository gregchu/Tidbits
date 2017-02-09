Pull image, then run and mount drive. The following pulls the latest tensorflow CPU only image and mounts ~/ on the local machine to /root on the docker image

`sudo docker run -it -v ~/:/root -p 8888:8888 gcr.io/tensorflow/tensorflow /bin/bash`

Detach
`ctrl-p+ctrl-q`

Reattach
`docker attach CONTAINER_NAME`

List containers
`docker ps`

Commit container changes to docker image


Remove docker containers

``docker rm `docker ps --no-trunc -aq` ``

to list last used container
``docker ps -l -q``
