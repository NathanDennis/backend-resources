### Resources and reference material for Docker

## YouTube videos / series

- [FreeCodeCamp Docker Tutorial](https://www.youtube.com/watch?v=fqMOX6JJhGo)

## Articles / written tutorials

- [Docker Tutorial for Beginners](https://docker-curriculum.com/) - docker-curriculum
- [The Docker Handbook](https://www.youtube.com/watch?v=fqMOX6JJhGo) -FreeCodeCamp
- [How to reduce Node Docker image size](https://itsopensource.com/how-to-reduce-node-docker-image-size-by-ten-times/) - itsopensource.com

## Commands

#### `docker ps` - Show all currently running containers

#### `docker run [image name]` - Run an image
  - If the image is not present, it will be pulled / downloaded on the first run
  
#### `docker run -d [image]` - Run a container in the background (detached)

#### `docker stop [container name]` - Stop a container
  - Can use the container ID or the container name as the parameter to stop

#### `docker rm [container name]` - Remove a stopped / exited container
  - Can use the ID or name in the command
  
#### `docker images` - List downloaded images

#### `docker rmi [image name]` - remove a specific image or list of images
  - Containers using the image must be exited first
  
#### `docker pull [image]` - Download an image without running the container

#### `docker attach [container]` - Attach a container to run in the foreground

#### `docker exec` - Run a command on a docker container
