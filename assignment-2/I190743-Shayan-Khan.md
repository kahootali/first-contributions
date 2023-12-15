								     (Q1)
						
In VM, there is a hardware level virtualization whereas in Containers there is an Operating System level virtualization.
VMs take more space upto Gigabytes while Containers take less space upto Megabytes.
In VMs, there is static compute, static memory and high resource usage while in Containers there is a burstable compute, burstable memory and low resource usage.

 								     (Q2)
 
Command: 
 						
docker run -d --publish 9090:80 --net assignment-2 --name assignment-2-I19-0743 nginx:1.24.0

Output:

Unable to find image 'nginx:1.24.0' locally
1.24.0: Pulling from library/nginx
7dbc1adf280e: Pull complete 
a7184f3665ed: Pull complete 
f144d5d97503: Pull complete 
9097eea98b48: Pull complete 
356d4b647b64: Pull complete 
608e661a622a: Pull complete 
Digest: sha256:73341830a31bf12a44c846b6b323dd8a4fab7668e72c16e9124913ff097c9536
Status: Downloaded newer image for nginx:1.24.0
240e71e4966853fbd777c57ce82bba09cf106638f2bde7291f7f202b7a70c1a8

								     (Q3)

Command:

docker container logs assignment-2-I19-0743	

Output:
					
/docker-entrypoint.sh: /docker-entrypoint.d/ is not empty, will attempt to perform configuration
/docker-entrypoint.sh: Looking for shell scripts in /docker-entrypoint.d/
/docker-entrypoint.sh: Launching /docker-entrypoint.d/10-listen-on-ipv6-by-default.sh
10-listen-on-ipv6-by-default.sh: info: Getting the checksum of /etc/nginx/conf.d/default.conf
10-listen-on-ipv6-by-default.sh: info: Enabled listen on IPv6 in /etc/nginx/conf.d/default.conf
/docker-entrypoint.sh: Launching /docker-entrypoint.d/20-envsubst-on-templates.sh
/docker-entrypoint.sh: Launching /docker-entrypoint.d/30-tune-worker-processes.sh
/docker-entrypoint.sh: Configuration complete; ready for start up
2023/10/07 16:16:01 [notice] 1#1: using the "epoll" event method
2023/10/07 16:16:01 [notice] 1#1: nginx/1.24.0
2023/10/07 16:16:01 [notice] 1#1: built by gcc 10.2.1 20210110 (Debian 10.2.1-6) 
2023/10/07 16:16:01 [notice] 1#1: OS: Linux 6.2.0-34-generic
2023/10/07 16:16:01 [notice] 1#1: getrlimit(RLIMIT_NOFILE): 1048576:1048576
2023/10/07 16:16:01 [notice] 1#1: start worker processes
2023/10/07 16:16:01 [notice] 1#1: start worker process 29
2023/10/07 16:16:01 [notice] 1#1: start worker process 30
2023/10/07 16:16:01 [notice] 1#1: start worker process 31
2023/10/07 16:16:01 [notice] 1#1: start worker process 32
