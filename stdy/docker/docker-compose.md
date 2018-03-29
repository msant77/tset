# Docker Compose Basics

## Docker Compose, Service

```
  498  sudo npm i pm2 -g
  499  ps2 list
  500  pm2
  501  pm2 list
  508  docker ps
  517  docker service ls
  518  docker -h
  519  docker service
  520  docker service ls\
  521  docker service
  522  docker service ls
  523  docker swarm init
  526  docker service ls
  527  docker stack ls
  529  docker-compose ps
  533  docker ps -a
```
> From the above list, check and separate unproper stuff from this file such as `ps2`, `docker service`, `docker swarm`


## The following are specific `docker-compose` commands usage
```
#docker-compose command list
docker-compose

#docker-compose run the _docker-compose.yml_
docker-compose up

#docker-compose stop running
docker-compose down

#force docker-compose to run and build all its nodes
docker-compose up --build

#docker-compose up and with the -d makes the whole thing runs into the detached mode
docker-compose up -d 

#checks the logs generated by the docker-compose detached mode
docker-compose logs

#make logs behave in a way it won't show everything it's been logged so far, down to the last 100 lines
#the last parameter `api` locks for the logs referred to the `api` service, supposedely described in the `docker-compose.yml` file
docker-compose logs --tail=100  api

#the `-f` parameter makes the above `docker-compose logs` locks after the print out
docker-compose logs --tail=100 -f api
```  
