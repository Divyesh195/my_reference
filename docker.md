# Docker

## 1. Basic commands

### Show all containers (running --> remove -a)
```
docker ps -a
```
### Stop/Start container
```
docker stop/start [container ID]
```
### List images
```
docker images
```
### Remove Images
```
docker rmi [Image_name]
```

## 2. Run commands

### Run images
```
docker run -it --name [provide container name] [image_name]
```
###### -it means interactive mode and -t means just visible terminal<br>Providing name using --name is optional


### Run images with port binding
```
docker run -d -p 5000:5000 --name [container_name] [docker_image]:tag
```
##### -d --> run in background <br> -p host_port --> container_port <br> if image has other tag then 'latest' then it is necessary to provide that in run command.


### Run images with environment varibales and network
```
docker run -d -p27017:27017 \
--name mongo_image --network mongo_network \
-e MONGO_INITDB_ROOT_USERNAME=divyesh84 \
-e MONGO_INITDB_ROOT_PASSWORD=0548 \
mongo
```

### Run containers again in interactive mode
```
docker start -ai [container name]
```
###### doesn't work everytime

### Run containers again in interactive mode (reliable method)
```
docker start container_name
docker exec -it container_name bash
```

## 3. Build commands

### Simple and Most comman
```
docker build -t my_website:1.0 .
```

##### -t is used to give name to the image. 1.0 is the tag given to the image, which is optional.  <br> . means build for current directory 


## 4. Docker Networks

### List all networks 
```
docker network ls
```
### Create a network
```
docker network create [network_name]
```