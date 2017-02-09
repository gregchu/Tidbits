Pull ubuntu image, then run and mount ~/ to /root

`sudo docker run -it -v ~/repo:/root/repo ubuntu /bin/bash`

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
