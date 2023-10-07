## Q1) Explain Docker Containers vs VMs

### Docker Containers:
1. Containers have OS level virtualization
2. Containers use the host's kernel but can also have its own OS
3. Containers have Burstable Compute and Memory
4. Containers are generally considered less secure due to lower isolation
5. Containers are genrally less resource intensive 

### Virtual Machines:
1. VMs have Hardware level virtualization
2. VMs have their own OS
3. VMs have Static Compute and Memory
4. VMs are generally considered more secure due to higher isolation
5. VMs are generally more resource intensive

<br>

## Q2) Write command to create a docker container in `detached` mode with name `assignment-2-<ROLL_NUMBER>` running on host port `9090` and container port `80` using image `nginx` with version `1.24.0` on a custom network named `assignment-2`

### Commands:

To create custom network:
```cmd
$ docker network create assignment-2
```

To create container:
```cmd
$ docker container run -d --publish 9090:80 --name assignment-2-I19-1715 --network assignment-2 nginx:1.24.0
```

**Note:** I had to use `sudo` with both commands as I needed superuser permissions for both the commands to work for me

<br>

## Q3) Run the above command and add screenshot of it and share the logs

### Screenshots:
![1](<docker_run.PNG>)
![2](<nginx.PNG>)

### Logs:
![3](<logs.PNG>)

/docker-entrypoint.sh: /docker-entrypoint.d/ is not empty, will attempt to perform configuration
/docker-entrypoint.sh: Looking for shell scripts in /docker-entrypoint.d/
/docker-entrypoint.sh: Launching /docker-entrypoint.d/10-listen-on-ipv6-by-default.sh
10-listen-on-ipv6-by-default.sh: info: Getting the checksum of /etc/nginx/conf.d/default.conf
10-listen-on-ipv6-by-default.sh: info: Enabled listen on IPv6 in /etc/nginx/conf.d/default.conf
/docker-entrypoint.sh: Launching /docker-entrypoint.d/20-envsubst-on-templates.sh
/docker-entrypoint.sh: Launching /docker-entrypoint.d/30-tune-worker-processes.sh
/docker-entrypoint.sh: Configuration complete; ready for start up
2023/10/07 21:33:56 [notice] 1#1: using the "epoll" event method
2023/10/07 21:33:56 [notice] 1#1: nginx/1.24.0
2023/10/07 21:33:56 [notice] 1#1: built by gcc 10.2.1 20210110 (Debian 10.2.1-6) 
2023/10/07 21:33:56 [notice] 1#1: OS: Linux 5.4.0-164-generic
2023/10/07 21:33:56 [notice] 1#1: getrlimit(RLIMIT_NOFILE): 1048576:1048576
2023/10/07 21:33:56 [notice] 1#1: start worker processes
2023/10/07 21:33:56 [notice] 1#1: start worker process 28
2023/10/07 21:33:56 [notice] 1#1: start worker process 29
2023/10/07 21:33:56 [notice] 1#1: start worker process 30
