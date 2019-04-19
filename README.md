# docker-begin

Docker
-----------------------------
--- Docker images
docker images -a -q -f
docker run <name>
docker history ubuntu = > view history of image
docker pull <name>  => pull image

--- docker container
docker ps -a
docker run --name <custome name> -it <image name> -> docker run --name MyUbuntu -it ubuntu

docker stats -> see memory/CPU...
docker attach <name>
docker kill  <name/id> => stop container
docker stop<name/id> => stop container
docker start<name/id> => stop container
docker rm <name/id> => remove container

--- Docker file
Create "Dockerfile" 
docker build -t <name>:1.0 <localtion> => build image

-- Docker compose
1. docker-compose --version
2. create docker-compose.yml
3. docker-compose config => Check validity:  add docker version 3, syntax must be correct (space, breakline...)
4. docker-compose up -d
5. docker-compose down
6. docker-compose up -d --scale <service>=<4> => docker-compose up -d --scale database=4
