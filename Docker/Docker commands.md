## **Docker commands**





**#Manage containers **:



| commands                                 | description                              |
| ---------------------------------------- | ---------------------------------------- |
| `docker ps`                              | show all running containers              |
| `docker ps -a`                           | show a list of all containers            |
| `docker rm container_name`               | delete a container                       |
| `docker rm -f container_name`            | delete a running container               |
| `docker container prune`                 | delete a stopped container               |
| `docker stop container_name`             | stop a running container                 |
| `docker start container_name`            | start a stopped container                |
| `docker cp container_name:source target` | copy a file from a container to the host |
| `docker cp target container_name:source` | copy a file from host to container       |
| `docker exec -it container executable`   | start a shell inside running container   |
| `docker rename old_name new_name`        | rename a container                       |
| `docker commit container_name`           | create an image out of a container       |

**#Run a new  container	**



| commands                                                     | description                                     |
| ------------------------------------------------------------ | ----------------------------------------------- |
| `docker run Image`                                           | start a new container from an image             |
| `docker run --name container_image`                          | .... and assign it a name                       |
| `docker run -p HOTSPORT:CONTAINERPORT IMAGE` EXAMPLE `docker run -p 8080:80 nginx` | ....and map a port                              |
| `docker run -P IMAGE`                                        | ... and map all ports                           |
| `docker run -d IMAGE`                                        | ...and start a container in background          |
| `docker run --hostname HOSTNAME IMAGE`                       | ... and assign it a host-name                   |
| `docker run --add-host HOSTNAME:IP IMAGE`                    | ...and add a dns entry                          |
| `docker run -v HOSTDIR:TARGETDIR IMAGE ` EXAMPLE  `docker run -v ~/:/usr/share/nginx/html nginx` | ...and map a local directory into the container |
| `docker run -it --entrypoint EXECUTABLE IMAGE`               | ...but change the entrypoint                    |

**#Docker compose**

| commands               | description          |
| ---------------------- | -------------------- |
| `docker-compose up`    | run a docker-compose |
| `docker-compose up -d` | run in background    |
| `docker-compose down`  | down                 |



**#Docker volumes	**



| commands                                  | description              |
| ----------------------------------------- | ------------------------ |
| `docker volume ls`                        | list all volumes         |
| `docker volume rm [volume_name]`          | remove specific volume   |
| `docker volume rm $(docker volume ls -q)` | remove all unused volume |



**#Docker build**

| command                                                  | description                                                  |
| -------------------------------------------------------- | ------------------------------------------------------------ |
| `sudo docker build -t [name_image] [path_of_dockerfile]` | The `docker build` command builds Docker images from a Dockerfile and a “context” |

**#Docker run**

| command                                                | description                      |
| ------------------------------------------------------ | -------------------------------- |
| `docker run -p [port_number:port_number] [image_name]` | Run a command in a new container |

