### Q1) Explain Docker Containers vs VMs
**Ans)** Docker Containers are lightweight isolated processes that share the host OS, allowing them to start quickly and use resources dynamically. Meanwhile, Virtual Machines perform hardware level virtualization and contain a full OS instance, making them bulkier and slower to boot.

### Q2) Write command to create a docker container in detached mode with name assignment-2-<ROLL_NUMBER> running on host port 9090 and container port 80 using image nginx with version 1.24.0 on a custom network named assignment-2
**Ans)** 
```bash
docker network create assignment-2 && docker run -d -p 9090:80 --name assignment-2-I20-0409 --network assignment-2 nginx:1.24.0
```

### Q3) Run the above command and add screenshot of it and share the logs
**Ans)**
cakes@Jellycake:~$ docker network create assignment-2 && docker run -d -p 9090:80 --name assignment-2-I20-0409 --network assignment-2 nginx:1.24.0
666585c3cf999c3a8d5b1bdd97817ef799ddd88982fd606ebd86da451bd38ecc
04a2f78e8f3618a231d62019b631548011b26895cc53eb7de036bebdbe4101ef
cakes@Jellycake:~$ docker logs assignment-2-I20-0409
/docker-entrypoint.sh: /docker-entrypoint.d/ is not empty, will attempt to perform configuration
/docker-entrypoint.sh: Looking for shell scripts in /docker-entrypoint.d/
/docker-entrypoint.sh: Launching /docker-entrypoint.d/10-listen-on-ipv6-by-default.sh
10-listen-on-ipv6-by-default.sh: info: Getting the checksum of /etc/nginx/conf.d/default.conf
10-listen-on-ipv6-by-default.sh: info: Enabled listen on IPv6 in /etc/nginx/conf.d/default.conf
/docker-entrypoint.sh: Launching /docker-entrypoint.d/20-envsubst-on-templates.sh
/docker-entrypoint.sh: Launching /docker-entrypoint.d/30-tune-worker-processes.sh
/docker-entrypoint.sh: Configuration complete; ready for start up
2023/10/05 13:38:05 [notice] 1#1: using the "epoll" event method
2023/10/05 13:38:05 [notice] 1#1: nginx/1.24.0
2023/10/05 13:38:05 [notice] 1#1: built by gcc 10.2.1 20210110 (Debian 10.2.1-6)
2023/10/05 13:38:05 [notice] 1#1: OS: Linux 5.10.102.1-microsoft-standard-WSL2
2023/10/05 13:38:05 [notice] 1#1: getrlimit(RLIMIT_NOFILE): 1048576:1048576
2023/10/05 13:38:05 [notice] 1#1: start worker processes
2023/10/05 13:38:05 [notice] 1#1: start worker process 29
2023/10/05 13:38:05 [notice] 1#1: start worker process 30
2023/10/05 13:38:05 [notice] 1#1: start worker process 31
2023/10/05 13:38:05 [notice] 1#1: start worker process 32
2023/10/05 13:38:05 [notice] 1#1: start worker process 33
2023/10/05 13:38:05 [notice] 1#1: start worker process 34
2023/10/05 13:38:05 [notice] 1#1: start worker process 35
2023/10/05 13:38:05 [notice] 1#1: start worker process 36
2023/10/05 13:38:05 [notice] 1#1: start worker process 37
2023/10/05 13:38:05 [notice] 1#1: start worker process 38
2023/10/05 13:38:05 [notice] 1#1: start worker process 39
2023/10/05 13:38:05 [notice] 1#1: start worker process 40
2023/10/05 13:38:05 [notice] 1#1: start worker process 41
2023/10/05 13:38:05 [notice] 1#1: start worker process 42
2023/10/05 13:38:05 [notice] 1#1: start worker process 43
2023/10/05 13:38:05 [notice] 1#1: start worker process 44
