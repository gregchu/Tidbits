Pull image, then run and mount drive. The following pulls the latest tensorflow CPU only image
`sudo docker run -it -v ~/:/root -p 8888:8888 gcr.io/tensorflow/tensorflow /bin/bash`

Detach
`ctrl-p+ctrl-q`

Reattach
`sudo docker run -it -v ~/:/root CONTAINER_ID /bin/bash

List containers
`docker ps -l`

Save state of container
`sudo docker commit `docker ps -lq` CONTAINER_NAME`
where CONTAINER_NAME is made up


