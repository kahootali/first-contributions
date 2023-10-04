## Question 1
# Docker Containers:

1. Containers are an abstraction at the application layer packaging code and dependencies together.
2. Containers take less space than VMs.
3. Containers are faster and start almost instantly. 
4. Has no 'works on my machine' issue. 
5. Shares hardware, host OS kernel but can have own OS. 

# Virtual Machines: 

1. VMs are an abstraction of phsycial hardware turning one server into many servers. 
2. VMs keep full copies of OS, libraries, etc taking up a lot of space.
3. VMs can be slow to boot. 
4. VMs have the 'works on my machine' issue
5. It Shares hardware but has own OS.

## Question 2
# Command: 
Creating network: docker network create assignment-2
Creating container: docker container run -d --publish 9090:80 --name assignment-2-I20-0437 --network assignment-2 nginx:1.24.0

## Question 3
# Screenshots: 

![1](<Screenshot 2023-10-04 at 12.08.51 PM.png>) ![2](<Screenshot 2023-10-04 at 12.09.22 PM.png>)
![3](<Screenshot 2023-10-04 at 12.14.13 PM.png>)

# Logs
2023-10-04 12:06:52 /docker-entrypoint.sh: /docker-entrypoint.d/ is not empty, will attempt to perform configuration
2023-10-04 12:06:52 /docker-entrypoint.sh: Looking for shell scripts in /docker-entrypoint.d/
2023-10-04 12:06:52 /docker-entrypoint.sh: Launching /docker-entrypoint.d/10-listen-on-ipv6-by-default.sh
2023-10-04 12:06:52 10-listen-on-ipv6-by-default.sh: info: Getting the checksum of /etc/nginx/conf.d/default.conf
2023-10-04 12:06:52 10-listen-on-ipv6-by-default.sh: info: Enabled listen on IPv6 in /etc/nginx/conf.d/default.conf
2023-10-04 12:06:52 /docker-entrypoint.sh: Launching /docker-entrypoint.d/20-envsubst-on-templates.sh
2023-10-04 12:06:52 /docker-entrypoint.sh: Launching /docker-entrypoint.d/30-tune-worker-processes.sh
2023-10-04 12:06:52 /docker-entrypoint.sh: Configuration complete; ready for start up
2023-10-04 12:06:52 2023/10/04 07:06:52 [notice] 1#1: using the "epoll" event method
2023-10-04 12:06:52 2023/10/04 07:06:52 [notice] 1#1: nginx/1.24.0
2023-10-04 12:06:52 2023/10/04 07:06:52 [notice] 1#1: built by gcc 10.2.1 20210110 (Debian 10.2.1-6) 
2023-10-04 12:06:52 2023/10/04 07:06:52 [notice] 1#1: OS: Linux 5.15.49-linuxkit-pr
2023-10-04 12:06:52 2023/10/04 07:06:52 [notice] 1#1: getrlimit(RLIMIT_NOFILE): 1048576:1048576
2023-10-04 12:06:52 2023/10/04 07:06:52 [notice] 1#1: start worker processes
2023-10-04 12:06:52 2023/10/04 07:06:52 [notice] 1#1: start worker process 29
2023-10-04 12:06:52 2023/10/04 07:06:52 [notice] 1#1: start worker process 30
2023-10-04 12:06:52 2023/10/04 07:06:52 [notice] 1#1: start worker process 31
2023-10-04 12:06:52 2023/10/04 07:06:52 [notice] 1#1: start worker process 32 