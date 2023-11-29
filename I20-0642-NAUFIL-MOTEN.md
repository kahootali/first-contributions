Q1 Ans:

Docker Containers:

Lightweight, share the host OS kernel.
Efficient resource usage.
Ideal for microservices and CI/CD.
Use containerization engine and images.

Virtual Machines (VMs):

Full OS virtualization.
Require hypervisor for management.
Stronger isolation but higher resource usage.
Suitable for running diverse OS or legacy apps.

Q2 Ans:

docker run -d -p 9090:80 --name assignment-2-i200642 --network assignment-2 nginx:1.24.0

Q3 Ans:

I wrote following commands and the screenshots of the results are attached with classroom submission:

docker network create assignment-2 (this is to create network)
docker run -d -p 9090:80 --name assignment-2-i200642 --network assignment-2 nginx:1.24.0
docker ps
docker logs assignment-2-i200642

Logs output:

/docker-entrypoint.sh: /docker-entrypoint.d/ is not empty, will attempt to perform configuration
/docker-entrypoint.sh: Looking for shell scripts in /docker-entrypoint.d/
/docker-entrypoint.sh: Launching /docker-entrypoint.d/10-listen-on-ipv6-by-default.sh
10-listen-on-ipv6-by-default.sh: info: Getting the checksum of /etc/nginx/conf.d/default.conf
10-listen-on-ipv6-by-default.sh: info: Enabled listen on IPv6 in /etc/nginx/conf.d/default.conf
/docker-entrypoint.sh: Launching /docker-entrypoint.d/20-envsubst-on-templates.sh
/docker-entrypoint.sh: Launching /docker-entrypoint.d/30-tune-worker-processes.sh
/docker-entrypoint.sh: Configuration complete; ready for start up
2023/10/08 17:29:36 [notice] 1#1: using the "epoll" event method
2023/10/08 17:29:36 [notice] 1#1: nginx/1.24.0
2023/10/08 17:29:36 [notice] 1#1: built by gcc 10.2.1 20210110 (Debian 10.2.1-6)
2023/10/08 17:29:36 [notice] 1#1: OS: Linux 5.10.16.3-microsoft-standard-WSL2
2023/10/08 17:29:36 [notice] 1#1: getrlimit(RLIMIT_NOFILE): 1048576:1048576
2023/10/08 17:29:36 [notice] 1#1: start worker processes
2023/10/08 17:29:36 [notice] 1#1: start worker process 29
2023/10/08 17:29:36 [notice] 1#1: start worker process 30
2023/10/08 17:29:36 [notice] 1#1: start worker process 31
2023/10/08 17:29:36 [notice] 1#1: start worker process 32