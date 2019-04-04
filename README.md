# Some essentials Docker commands

## Run

```shell
# Run an image
docker run IMAGE_NAME

# Run an image and use its terminal
docker run -it IMAGE_NAME

# Run in background
docker run -d IMAGE_NAME

# Run in background and on a random external port
docker run -d -P IMAGE_NAME

# Run in background, on a random external port and changing the container's name
docker run -d -P --name NEW_CONTAINER_NAME

# Run in background and choosing the external port
docker run -d -p ####:80 IMAGE_NAME
OBS: #### = your port of choice
```
