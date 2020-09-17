### Resources and reference material for Docker

## YouTube videos / series

- [FreeCodeCamp Docker Tutorial](https://www.youtube.com/watch?v=fqMOX6JJhGo)

## Articles / written tutorials

- [Docker Tutorial for Beginners](https://docker-curriculum.com/) - docker-curriculum
- [The Docker Handbook](https://www.youtube.com/watch?v=fqMOX6JJhGo) -FreeCodeCamp
- [How to reduce Node Docker image size](https://itsopensource.com/how-to-reduce-node-docker-image-size-by-ten-times/) - itsopensource.com

## Commands

#### `docker ps` - Show all currently running containers

#### `docker create [image name]` - Prep a container with the specified image without starting it

#### `docker start [image / container]` - Start a created, or previously stopped container

#### `docker run [image name]` - Combines create & start to prep a new container and run an image
  - If the image is not present, it will be pulled / downloaded on the first run
  
#### `docker run -d [image]` - Run a container in the background (detached)

#### `docker stop [container name]` - Stop a container
  - Can use the container ID or the container name as the parameter to stop
  - Stop command allows the container to shut down on its' own time after cleanup

#### `docker kill [container name]` - Immediately stop a container
  - docker stop falls back to docker kill if the container doesn't shut down within 10 seconds

#### `docker rm [container name]` - Remove a stopped / exited container
  - Can use the ID or name in the command
  
#### `docker images` - List downloaded images

#### `docker rmi [image name]` - remove a specific image or list of images
  - Containers using the image must be exited first
  
#### `docker pull [image]` - Download an image without running the container

#### `docker attach [container]` - Attach a container to run in the foreground

#### `docker exec` - Run a command on a docker container

#### `docker system prune` - Remove all stopped containers
  - This will also remove all build cache, and all networks not used by at least one container

#### `docker logs [container id]` - Get logs of any events emitted from a container

