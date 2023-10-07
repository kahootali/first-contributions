# Answers to Questions for Assignment 2
# Question-1

-Container vs VMs:
1. VMs have Hardware level virtualization ( physical layer ) while containers have OS level virtualization( application layer ).
2. VMs share Hardware but has own it own operating system while containers share hardware, host OS kernel but can have own operating systems.
3. VMs can take up to tens of GBs while containers are much smaller in size, and they have a lot less overhead than virtual machines (they don't need an OS)
4. VMs are isolated, apps are not while containers share the same OS and kernel with other containers, reducing overhead but limiting isolation capabilities.
5. Containers are lightweight and portable, whereas virtual machines (VMs) require more resources than containers but can be run on any infrastructure that supports them.
6. VMs have static compute, static high Resource and usages whereas containers are dynamic in nature with low resource consumption but can be scaled up or down on demand.

# Question-2
Creating the required network using:
 ->docker network create assignment-2

Launch the designated container using:
 ->docker run -d --name assignment-2-I20-0489 --network assignment-2 -p 9090:80 nginx:1.24.0

Explaination of Launch Command:
-> docker run [OPTIONS] IMAGE[:TAG|@DIGEST] COMMAND [ARG...]
Run a command in a new container.
Options:
    -d : Detached mode: Run container in background and print container ID.
    -name="nginx" : Assign a name to the container.
    -network: Connect a container to a network.
    -p : Publish a container's port(s) to the host (format: ip:hostPort:containerPort)

# Question-3
Commands screenshot: Docker-Commands.png [Root]
Running Container: Running-Container.png [Root]
Nginx Running: Nginx-Running.png [Root]