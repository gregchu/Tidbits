Pull ubuntu image, then run and mount ~/ to /root

`sudo docker run -it -v ~/repo:/root/repo ubuntu /bin/bash`

Detach

`ctrl-p+ctrl-q`

Reattach

`docker attach CONTAINER_NAME`

List containers

`docker ps`

Commit container changes to docker image


Stop or kill container

``docker stop/kill CONTAINER NAME``

Remove all docker containers

``docker rm `docker ps --no-trunc -aq` ``

Remove a docker container

``docker rm CONTAINER_NAME``

to list last used container

``docker ps -l -q``
