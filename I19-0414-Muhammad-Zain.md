Q1. Explain Docker Conatiners VS VMs

Answer:

VMs:
● Hardware level virtualization i.e. abstraction of physical hardware
● Share Hardware but has own OS
● Each VM has a full copy of an operating system + application + binaries + libraries ● can take up to tens of GBs.
● VMs are isolated, apps are not
● Complete OS, Static Compute, Static Memory, High Resource Usage

Containers:
● OS level virtualization i.e. abstraction at the app layer (code + dependencies)
● Share hardware, host OS kernel but can have own OS
● take up less space (typically tens to hundreds of MBs in size)
● containers are isolated, so are the apps ● Container Isolation, Shared Kernel, Burstable Compute, Burstable Memory, Low Resource Usage

Q2. Write command to create a docker container in detached mode with name assignment-2-<ROLL_NUMBER> running on host port 9090 and container port 80 using image nginx with version 1.24.0 on a custom network named assignment-2

Answer:

docker run -d --name assignment-2-I19-0414 -p 9090:80 --network assignment-2 nginx:1.24.0

Q3. Run the above command and add screenshot of it and share the logs

Answer:

Note: Screenshots are attached with this folder

### Container logs

/docker-entrypoint.sh: /docker-entrypoint.d/ is not empty, will attempt to perform configuration
/docker-entrypoint.sh: Looking for shell scripts in /docker-entrypoint.d/
/docker-entrypoint.sh: Launching /docker-entrypoint.d/10-listen-on-ipv6-by-default.sh
10-listen-on-ipv6-by-default.sh: info: Getting the checksum of /etc/nginx/conf.d/default.conf
10-listen-on-ipv6-by-default.sh: info: Enabled listen on IPv6 in /etc/nginx/conf.d/default.conf
/docker-entrypoint.sh: Launching /docker-entrypoint.d/20-envsubst-on-templates.sh
/docker-entrypoint.sh: Launching /docker-entrypoint.d/30-tune-worker-processes.sh
/docker-entrypoint.sh: Configuration complete; ready for start up
2023/10/08 07:30:37 [notice] 1#1: using the "epoll" event method
2023/10/08 07:30:37 [notice] 1#1: nginx/1.24.0
2023/10/08 07:30:37 [notice] 1#1: built by gcc 10.2.1 20210110 (Debian 10.2.1-6)
2023/10/08 07:30:37 [notice] 1#1: OS: Linux 5.15.90.1-microsoft-standard-WSL2
2023/10/08 07:30:37 [notice] 1#1: getrlimit(RLIMIT_NOFILE): 1048576:1048576
2023/10/08 07:30:37 [notice] 1#1: start worker processes
2023/10/08 07:30:37 [notice] 1#1: start worker process 29
2023/10/08 07:30:37 [notice] 1#1: start worker process 30
2023/10/08 07:30:37 [notice] 1#1: start worker process 31
2023/10/08 07:30:37 [notice] 1#1: start worker process 32
2023/10/08 07:30:37 [notice] 1#1: start worker process 33
2023/10/08 07:30:37 [notice] 1#1: start worker process 34
2023/10/08 07:30:37 [notice] 1#1: start worker process 35
2023/10/08 07:30:37 [notice] 1#1: start worker process 36
172.18.0.1 - - [08/Oct/2023:07:31:52 +0000] "GET / HTTP/1.1" 200 615 "-" "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/117.0.0.0 Safari/537.36" "-"
2023/10/08 07:31:53 [error] 30#30: \*1 open() "/usr/share/nginx/html/favicon.ico" failed (2: No such file or directory), client: 172.18.0.1, server: localhost, request: "GET /favicon.ico HTTP/1.1", host: "localhost:9090", referrer: "http://localhost:9090/"
172.18.0.1 - - [08/Oct/2023:07:31:53 +0000] "GET /favicon.ico HTTP/1.1" 404 555 "http://localhost:9090/" "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/117.0.0.0 Safari/537.36" "-"
