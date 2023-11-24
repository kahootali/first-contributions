##### Q1) Explain Docker Containers vs VMs
**Ans)** VM's provide an abstraction layer over the hardware while containers provide an absdtraction layer at the app level. In containers we are provided with all the required dependencies whereas in VM's we have to install them by ourselves. Containers tend to be in smaller sizes a matter of MB's, while VM's tend to be in the range of 2GB+. In VM's each machine has their own kernal, while in Containers each container share the OS kernel with each other. Since containers is packaged with all the required dependencies we don't get the issues such as it works on my machine, while in VM's we tend to get such issues.

##### Q2) Write command to create a docker container in detached mode with name assignment-2-<ROLL_NUMBER> running on host port 9090 and container port 80 using image nginx with version 1.24.0 on a custom network named assignment-2
**Ans)** 
###### For creating network assignment-2
``` docker network create assignment-2```
###### For creating container
```docker container run -d --publish 9090:80 --name assignment-2-I20-0437 --network assignment-2 nginx:1.24.0```


##### Q3) Run the above command and add screenshot of it and share the logs
Logs:
2023-10-03 12:51:30 /docker-entrypoint.sh: /docker-entrypoint.d/ is not empty, will attempt to perform configuration
2023-10-03 12:51:30 /docker-entrypoint.sh: Looking for shell scripts in /docker-entrypoint.d/
2023-10-03 12:51:30 /docker-entrypoint.sh: Launching /docker-entrypoint.d/10-listen-on-ipv6-by-default.sh
2023-10-03 12:51:30 10-listen-on-ipv6-by-default.sh: info: Getting the checksum of /etc/nginx/conf.d/default.conf
2023-10-03 12:51:30 10-listen-on-ipv6-by-default.sh: info: Enabled listen on IPv6 in /etc/nginx/conf.d/default.conf
2023-10-03 12:51:30 /docker-entrypoint.sh: Launching /docker-entrypoint.d/20-envsubst-on-templates.sh
2023-10-03 12:51:30 /docker-entrypoint.sh: Launching/docker-entrypoint.d/30-tune-worker-processes.sh
2023-10-03 12:51:30 /docker-entrypoint.sh: Configuration complete; ready for start up
2023-10-03 12:51:30 2023/10/03 07:51:30 [notice] 1#1: using the "epoll" event method
2023-10-03 12:51:30 2023/10/03 07:51:30 [notice] 1#1: nginx/1.24.0
2023-10-03 12:51:30 2023/10/03 07:51:30 [notice] 1#1: built by gcc 10.2.1 20210110 (Debian 10.2.1-6) 
2023-10-03 12:51:30 2023/10/03 07:51:30 [notice] 1#1: OS: Linux 5.15.49-linuxkit-pr
2023-10-03 12:51:30 2023/10/03 07:51:30 [notice] 1#1: getrlimit(RLIMIT_NOFILE): 1048576:1048576
2023-10-03 12:51:30 2023/10/03 07:51:30 [notice] 1#1: start worker processes
2023-10-03 12:51:30 2023/10/03 07:51:30 [notice] 1#1: start worker process 29
2023-10-03 12:51:30 2023/10/03 07:51:30 [notice] 1#1: start worker process 30
2023-10-03 12:51:30 2023/10/03 07:51:30 [notice] 1#1: start worker process 31
2023-10-03 12:51:30 2023/10/03 07:51:30 [notice] 1#1: start worker process 32
2023-10-03 12:51:30 2023/10/03 07:51:30 [notice] 1#1: start worker process 33