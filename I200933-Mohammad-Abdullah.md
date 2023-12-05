Q1) Explain Docker Containers vs VMs
Docker containers represent the active instances of Docker images. They utilize OS-level virtualization, with the sharing of the OS kernel. On the other hand, virtual machines (VMs) employ hardware-level virtualization. Containers include their own libraries, while VMs require manual installation of all components. Containers offer flexible compute resources, while VMs are characterized as static computing machines.
Q2) Write command to create a docker container in detached mode with name assignment-2-<ROLL_NUMBER> running on host port 9090 and container port 80 using image nginx with version 1.24.0 on a custom network named assignment-2
docker container run -d --name assignment-2-I20-0933 -p 9090:80 --network assignment-2 nginx:1.24.0
Q3) logs
/docker-entrypoint.sh: /docker-entrypoint.d/ is not empty, will attempt to perform configuration
/docker-entrypoint.sh: Looking for shell scripts in /docker-entrypoint.d/
/docker-entrypoint.sh: Launching /docker-entrypoint.d/10-listen-on-ipv6-by-default.sh
10-listen-on-ipv6-by-default.sh: info: Getting the checksum of /etc/nginx/conf.d/default.conf
10-listen-on-ipv6-by-default.sh: info: Enabled listen on IPv6 in /etc/nginx/conf.d/default.conf
/docker-entrypoint.sh: Launching /docker-entrypoint.d/20-envsubst-on-templates.sh
/docker-entrypoint.sh: Launching /docker-entrypoint.d/30-tune-worker-processes.sh
/docker-entrypoint.sh: Configuration complete; ready for start up
2023/10/08 15:02:41 [notice] 1#1: using the "epoll" event method
2023/10/08 15:02:41 [notice] 1#1: nginx/1.24.0
2023/10/08 15:02:41 [notice] 1#1: built by gcc 10.2.1 20210110 (Debian 10.2.1-6) 
2023/10/08 15:02:41 [notice] 1#1: OS: Linux 6.2.0-32-generic
2023/10/08 15:02:41 [notice] 1#1: getrlimit(RLIMIT_NOFILE): 1048576:1048576
2023/10/08 15:02:41 [notice] 1#1: start worker processes
2023/10/08 15:02:41 [notice] 1#1: start worker process 29
2023/10/08 15:02:41 [notice] 1#1: start worker process 30
2023/10/08 15:02:41 [notice] 1#1: start worker process 31
2023/10/08 15:02:41 [notice] 1#1: start worker process 32
172.18.0.1 - - [08/Oct/2023:15:04:30 +0000] "GET / HTTP/1.1" 200 615 "-" "Mozilla/5.0 (X11; Linux x86_64; rv:103.0) Gecko/20100101 Firefox/103.0" "-"
172.18.0.1 - - [08/Oct/2023:15:04:31 +0000] "GET /favicon.ico HTTP/1.1" 404 153 "http://127.0.0.1:9090/" "Mozilla/5.0 (X11; Linux x86_64; rv:103.0) Gecko/20100101 Firefox/103.0" "-"
2023/10/08 15:04:31 [error] 29#29: *1 open() "/usr/share/nginx/html/favicon.ico" failed (2: No such file or directory), client: 172.18.0.1, server: localhost, request: "GET /favicon.ico HTTP/1.1", host: "127.0.0.1:9090", referrer: "http://127.0.0.1:9090/"

