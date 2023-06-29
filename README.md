# My API Docker Deployment

This repository contains a Dockerfile for building a Docker image of My API, a RESTful API built with Golang.

## Prerequisites

- Docker installed on your machine.

## Building the Docker Image

To build the Docker image, navigate to the directory containing the Dockerfile and execute the following command:

 ` ` `bash
docker build -t my-api .
 ` ` `

This command builds the Docker image and tags it as "my-api".

## Running the Docker Container

To run the Docker container, execute the following command:

 ` ` `bash
docker run -d -p 8080:8080 my-api
 ` ` `

This command runs the Docker container in detached mode and maps port 8080 of the container to port 8080 of the host machine.

## Accessing the API

With the Docker container running, you can access the API at `http://localhost:8080`.

## Stopping the Docker Container

To stop the Docker container, first get the container ID with the following command:

 ` ` `bash
docker ps
 ` ` `

Then, stop the container with the following command:

 ` ` `bash
docker stop <container-id>
 ` ` `

Replace `<container-id>` with the ID of your running Docker container.

