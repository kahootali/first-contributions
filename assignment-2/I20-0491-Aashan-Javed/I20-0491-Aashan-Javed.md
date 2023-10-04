# Assignment 2 - I20-0491 - Aashan Javed

## Q1 Explain Docker Containers vs VMs

Docker containers are lightweight, share the core of the host operating system and package applications with their dependencies for efficient and consistent deployment. VMs, on the other hand, virtualize entire operating systems, resulting in higher resource utilization but greater isolation between applications.

## Q2 Write command to create a docker container in detached mode with name assignment-2-I12-0198 running on host port 9090 and container port 80 using image nginx with version 1.24.0 on a custom network named assignment-2

Creating a Docker container with the above requirements can be done with the following command:

```shell
docker run -d --name assignment-2-I20-0491 -p 9090:80 --network assignment-2 nginx:1.24.0

## Q3) Run the above command and add screenshot of it and share the logs

**Screenshot**
![Screenshot](https://drive.google.com/file/d/1iMaehGsMTsBLmrkDIPpLG684_SpNDmY1/view?usp=sharing)

**Docker Container Logs:**

/docker-entrypoint.sh: /docker-entrypoint.d/ is not empty, will attempt to perform configuration
/docker-entrypoint.sh: Looking for shell scripts in /docker-entrypoint.d/
/docker-entrypoint.sh: Launching /docker-entrypoint.d/10-listen-on-ipv6-by-default.sh
10-listen-on-ipv6-by-default.sh: info: Getting the checksum of /etc/nginx/conf.d/default.conf  
10-listen-on-ipv6-by-default.sh: info: Enabled listen on IPv6 in /etc/nginx/conf.d/default.conf
/docker-entrypoint.sh: Launching /docker-entrypoint.d/20-envsubst-on-templates.sh
/docker-entrypoint.sh: Launching /docker-entrypoint.d/30-tune-worker-processes.sh
/docker-entrypoint.sh: Configuration complete; ready for start up
2023/10/04 09:33:24 [notice] 1#1: using the "epoll" event method
2023/10/04 09:33:24 [notice] 1#1: nginx/1.24.0
2023/10/04 09:33:24 [notice] 1#1: built by gcc 10.2.1 20210110 (Debian 10.2.1-6)
2023/10/04 09:33:24 [notice] 1#1: OS: Linux 5.15.90.1-microsoft-standard-WSL2
2023/10/04 09:33:24 [notice] 1#1: getrlimit(RLIMIT_NOFILE): 1048576:1048576
2023/10/04 09:33:24 [notice] 1#1: start worker processes
2023/10/04 09:33:24 [notice] 1#1: start worker process 29
2023/10/04 09:33:24 [notice] 1#1: start worker process 30
2023/10/04 09:33:24 [notice] 1#1: start worker process 31
2023/10/04 09:33:24 [notice] 1#1: start worker process 32
2023/10/04 09:33:24 [notice] 1#1: start worker process 33
2023/10/04 09:33:24 [notice] 1#1: start worker process 34
2023/10/04 09:33:24 [notice] 1#1: start worker process 35
2023/10/04 09:33:24 [notice] 1#1: start worker process 36
2023/10/04 09:33:24 [notice] 1#1: start worker process 37
2023/10/04 09:33:24 [notice] 1#1: start worker process 38
2023/10/04 09:33:24 [notice] 1#1: start worker process 39
2023/10/04 09:33:24 [notice] 1#1: start worker process 40
