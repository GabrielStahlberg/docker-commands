# Some essentials Docker commands

```shell
## Find some ready images: https://hub.docker.com/
```

## Show

```shell
# Show all running containers
docker ps

# Show all created containers
docker ps -a

# Show all images
docker images
```

## Start

```shell
# Start a stopped container that was already created
docker start CONTAINER_ID

# Start a stopped container that was already created and hitch the shell
docker start -a -i CONTAINER_ID
```

## Stop

```shell
# Stop a specific container
docker stop CONTAINER_ID
```

## Remove

```shell
# Remove an specific container
docker rm CONTAINER_ID

# Remove an specific image
docker rmi REPOSITORY

# Remove all stopped containers
docker container prune
```

## Run

```shell
# Run an image
docker run IMAGE_NAME

# Run an image and use its shell
docker run -it IMAGE_NAME

# Run in background
docker run -d IMAGE_NAME

# Run in background and on a random external port
docker run -d -P IMAGE_NAME

# Run in background, on a random external port and changing the container's name
docker run -d -P --name NEW_CONTAINER_NAME

# Run in background and choosing the external port
docker run -d -p ????:80 IMAGE_NAME
OBS: ???? = your port of choice
```
