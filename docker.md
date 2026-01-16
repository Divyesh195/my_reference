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