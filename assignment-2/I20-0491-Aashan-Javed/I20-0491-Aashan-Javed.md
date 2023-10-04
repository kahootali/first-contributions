# Assignment 2 - I20-0491 - Aashan Javed

## Q1 Explain Docker Containers vs VMs

Docker containers are lightweight, share the core of the host operating system and package applications with their dependencies for efficient and consistent deployment. VMs, on the other hand, virtualize entire operating systems, resulting in higher resource utilization but greater isolation between applications.

## Q2 Write command to create a docker container in detached mode with name assignment-2-I12-0198 running on host port 9090 and container port 80 using image nginx with version 1.24.0 on a custom network named assignment-2

Creating a Docker container with the above requirements can be done with the following command:

```shell
docker run -d --name assignment-2-I20-0491 -p 9090:80 --network assignment-2 nginx:1.24.0
