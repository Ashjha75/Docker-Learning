# Docker Learning

![Docker Logo](https://www.docker.com/sites/default/files/d8/2019-07/Moby-logo.png)

Welcome to my Docker learning journey! This repository documents my progress as I explore and master Docker, a powerful platform for developing, shipping, and running applications.

## Table of Contents

- [Introduction](#introduction)
- [Getting Started](#getting-started)
- [Basic Docker Commands](#basic-docker-commands)
- [Creating a Dockerfile](#creating-a-dockerfile)
- [Building and Running Containers](#building-and-running-containers)
- [Docker Compose](#docker-compose)
- [Resources](#resources)

## Introduction

Docker is an open platform for developing, shipping, and running applications. It enables you to separate your applications from your infrastructure so you can deliver software quickly. With Docker, you can manage your infrastructure in the same ways you manage your applications.

## Getting Started

To get started with Docker, you need to install Docker on your machine. Follow the official installation guide for your operating system:

- [Docker for Windows](https://docs.docker.com/docker-for-windows/install/)
- [Docker for Mac](https://docs.docker.com/docker-for-mac/install/)
- [Docker for Linux](https://docs.docker.com/engine/install/)

## Basic Docker Commands

Here are some basic Docker commands to get you started:

```sh
# Pull an image from Docker Hub
docker pull <image_name>

# List all Docker images
docker images

# Run a Docker container
docker run -d -p 80:80 <image_name>

# List all running containers
docker ps

# Stop a running container
docker stop <container_id>

```
# Creating A Docker
A Dockerfile is a text document that contains all the commands to assemble an image. Here's an example of a simple Dockerfile:
``` bash
# Use an official OpenJDK runtime as a parent image
FROM openjdk:11-jre-slim

# Set the working directory in the container
WORKDIR /app

# Copy the current directory contents into the container at /app
COPY . /app

# Add the application's JAR file to the container
COPY target/your-spring-boot-app.jar /app/your-spring-boot-app.jar

# Make port 8080 available to the world outside this container
EXPOSE 8080

# Run the Spring Boot application
ENTRYPOINT ["java", "-jar", "/app/your-spring-boot-app.jar"]
```
# Building and Running the Docker Container
``` Bash
# Build the Docker image
docker build -t your-spring-boot-app .

# Run the Docker container
docker run -p 8080:8080 your-spring-boot-app
```