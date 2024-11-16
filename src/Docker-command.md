# List all Docker images
```sh 
docker images
```

# Pull an image from Docker Hub
```sh 
docker pull <image_name>
```

# Build an image from a Dockerfile
```sh 
docker build -t <image_name> 
```.
```

# List all running containers
```sh 
docker ps
```

# List all containers (including stopped ones)
```sh 
docker ps -a
```

# Run a container from an image
```sh 
docker run -d -p <host_port>:<container_port> <image_name>
```

# Stop a running container
```sh 
docker stop <container_id>
```

# Remove a stopped container
```sh 
docker rm <container_id>
```

# Remove an image
```sh 
docker rmi <image_name>
```

# View logs of a container
```sh 
docker logs <container_id>
```

# Execute a command inside a running container
```sh 
docker exec -it <container_id> <command>
```

# Start a stopped container
```sh 
docker start <container_id>
```

# Restart a running container
```sh 
docker restart <container_id>
```

# Remove all stopped containers
```sh 
docker container prune
```

# Remove all unused images
```sh 
docker image prune
```

# Remove all unused volumes
```sh 
docker volume prune
```

# Remove all unused networks
```sh 
docker network prune
```

# Remove all unused data (containers, images, volumes, networks)
```sh 
docker system prune
```

# Build and start containers using Docker Compose
```sh 
docker-compose up
```

# Stop and remove containers using Docker Compose
```sh 
docker-compose down
```

# Build images without starting containers using Docker Compose
```sh 
docker-compose build
```

# List all services defined in a Docker Compose file
```sh 
docker-compose config --services
```

# View logs of all services in a Docker Compose application
```sh 
docker-compose logs
```

# Scale services in a Docker Compose application
```sh 
docker-compose scale <service_name>=<number_of_instances>
```