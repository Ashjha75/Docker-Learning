# List all Docker images
docker images

# Pull an image from Docker Hub
docker pull <image_name>

# Build an image from a Dockerfile
docker build -t <image_name> .

# List all running containers
docker ps

# List all containers (including stopped ones)
docker ps -a

# Run a container from an image
docker run -d -p <host_port>:<container_port> <image_name>

# Stop a running container
docker stop <container_id>

# Remove a stopped container
docker rm <container_id>

# Remove an image
docker rmi <image_name>

# View logs of a container
docker logs <container_id>

# Execute a command inside a running container
docker exec -it <container_id> <command>

# Start a stopped container
docker start <container_id>

# Restart a running container
docker restart <container_id>

# Remove all stopped containers
docker container prune

# Remove all unused images
docker image prune

# Remove all unused volumes
docker volume prune

# Remove all unused networks
docker network prune

# Remove all unused data (containers, images, volumes, networks)
docker system prune

# Build and start containers using Docker Compose
docker-compose up

# Stop and remove containers using Docker Compose
docker-compose down

# Build images without starting containers using Docker Compose
docker-compose build

# List all services defined in a Docker Compose file
docker-compose config --services

# View logs of all services in a Docker Compose application
docker-compose logs

# Scale services in a Docker Compose application
docker-compose scale <service_name>=<number_of_instances>