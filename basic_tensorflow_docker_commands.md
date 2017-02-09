Image->Container: pull ubuntu image, then run and mount ~/repo to /root/repo

`sudo docker run -it -v ~/repo:/root/repo ubuntu /bin/bash`

Detach

`ctrl-p+ctrl-q`

Reattach

`docker attach CONTAINER_NAME`

Start

`docker start CONTAINER_NAME`

List containers

`docker ps`

Commit container changes

`docker commit CONTAINER_NAME`

Stop or kill container

``docker stop/kill CONTAINER NAME``

Remove all docker containers

``docker rm `docker ps --no-trunc -aq` ``

Remove a docker container

``docker rm CONTAINER_NAME``

List last used container

``docker ps -l -q``
