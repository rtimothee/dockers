# Dockers

List of Docker-compose files for setup somes web applications

### Usefull docker commands : 
#### Containers
- `docker ps` : list active containers
- `docker ps -a` : list all containers
- `docker start/stop [container name]` :  Start/Stop a docker container
- `docker rm [container name]` : remove container but not the associated image(s)
- `docker stop $(docker ps -q)` : Stop all dockers
- `docker rm $(docker ps -a -q)` : Remove all containers
#### Images
- `docker images` : list all docker images
- `docker rmi $(docker images -q)` : remove all docker images
#### Networks
- `docker network ls` : networks list
#### Docker compose
- `docker-compose [-f docker-compose.file.yml] up -d` : start/builds the containers configured in the docker-compose file(s)
- `docker-compose down` : Stops containers and removes containers, networks, volumes, and images created by 'up'
