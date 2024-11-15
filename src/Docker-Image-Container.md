# Docker Flow

1st we make a docker file wich contain metadat about the docker image then from this image we generate the new container

## Create a Dockerfile:

A Dockerfile is a text file that contains a set of instructions to build a Docker image.
It specifies the base image to use, application code, dependencies, and any configuration needed to run the application.


## Build the Docker Image:

Use the docker build command to create an image from the Dockerfile.
The Docker build process reads the instructions in the Dockerfile and assembles the image layer by layer.
The resulting image is a snapshot of the application and its environment.


## Verify the Docker Image:

After building the image, you can verify its existence and details using the docker images command.
This command lists all the Docker images available on your system.


## Run a Docker Container:

Use the docker run command to create and start a container from the Docker image.
A container is an instance of the image, running as an isolated process on the host system.
You can specify options such as port mappings, environment variables, and resource limits when running the container.

## Verify the Docker Container:

After running the container, you can verify its status and details using the docker ps command.
This command lists all the running containers on your system.


## Interact with the Docker Container:

You can interact with the running container using various Docker commands.
For example, you can execute commands inside the container, view logs, or stop and remove the container as needed.