Question 1: Explain Docker Containers vs VM

Docker Container:
    Containers are OS level virtualized environments to run applications. They come with application, requried binaries and their own OS. They share the kernel of the host OS. Containers run as processes on host OS. The have burstable memory which can increase or decrease according to the need. Docker is a provider which provides containers technology and the container of Docker are called Docker containers.

VMs:
    Virtual Machines are hardware level virtualized environments. They have a fixed memory and storage. VMs comes with their own OS and kernel. To run an application on VMs, application and dependencies are installed manually. When required, their memory and storage is expanded manually.


Question 2:
    Command = docker run -d --name assignment-2-I19-2195 -p 9090:80 --network assignment-2 nginx:1.24.0

    This command runs an nginx container named assignment2-I19-2195 on host port 80 in a network named assignment-2


Question 3:

    The screenshots has been attached with submission and logs are the following

    docker ps
CONTAINER ID   IMAGE          COMMAND                  CREATED         STATUS         PORTS                                   NAMES
6e40076f8b6b   nginx:1.24.0   "/docker-entrypoint.…"   3 minutes ago   Up 3 minutes   0.0.0.0:9090->80/tcp, :::9090->80/tcp   assignment-2-I19-2195
root@zakariya-VirtualBox:/home/zakariya# docker logs assignment-2-I19-2195
/docker-entrypoint.sh: /docker-entrypoint.d/ is not empty, will attempt to perform configuration
/docker-entrypoint.sh: Looking for shell scripts in /docker-entrypoint.d/
/docker-entrypoint.sh: Launching /docker-entrypoint.d/10-listen-on-ipv6-by-default.sh
10-listen-on-ipv6-by-default.sh: info: Getting the checksum of /etc/nginx/conf.d/default.conf
10-listen-on-ipv6-by-default.sh: info: Enabled listen on IPv6 in /etc/nginx/conf.d/default.conf
/docker-entrypoint.sh: Launching /docker-entrypoint.d/20-envsubst-on-templates.sh
/docker-entrypoint.sh: Launching /docker-entrypoint.d/30-tune-worker-processes.sh
/docker-entrypoint.sh: Configuration complete; ready for start up
2023/10/08 09:48:41 [notice] 1#1: using the "epoll" event method
2023/10/08 09:48:41 [notice] 1#1: nginx/1.24.0
2023/10/08 09:48:41 [notice] 1#1: built by gcc 10.2.1 20210110 (Debian 10.2.1-6) 
2023/10/08 09:48:41 [notice] 1#1: OS: Linux 5.15.0-41-generic
2023/10/08 09:48:41 [notice] 1#1: getrlimit(RLIMIT_NOFILE): 1048576:1048576
2023/10/08 09:48:41 [notice] 1#1: start worker processes
2023/10/08 09:48:41 [notice] 1#1: start worker process 29
2023/10/08 09:48:41 [notice] 1#1: start worker process 30
2023/10/08 09:48:41 [notice] 1#1: start worker process 31
2023/10/08 09:48:41 [notice] 1#1: start worker process 32
2023/10/08 09:48:41 [notice] 1#1: start worker process 33
2023/10/08 09:48:41 [notice] 1#1: start worker process 34

This line is being added to handle the comment on PR

