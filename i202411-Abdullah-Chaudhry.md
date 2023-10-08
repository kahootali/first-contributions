# Assignment 2

### Question One: 
**Containers vs Vm**
	- Docker containers are lightweight, portable, and consistent runtime environments for applications.
	- They share the host OS kernel, which makes them more efficient in terms of resource utilization.
	- Containers are isolated from each other using namespaces and control groups (cgroups).
	- They start up quickly and consume fewer resources.
	- VMs are complete virtualized environments that emulate physical hardware.
	- Each VM includes a full OS, which makes them bulkier compared to containers.
	- VMs provide strong isolation since they run on a hypervisor that manages resources.
	- VMs take longer to start up and consume more resources due

### Question two: 
```
docker run -d -p 9090:80 --name Assignment-2-i202411 --network assignment-2 nginx:1.24.0
```

### Question Three: 
Running on the above command on fedora 38. 
Logs
```
/docker-entrypoint.sh: /docker-entrypoint.d/ is not empty, will attempt to perform configuration
/docker-entrypoint.sh: Looking for shell scripts in /docker-entrypoint.d/
/docker-entrypoint.sh: Launching /docker-entrypoint.d/10-listen-on-ipv6-by-default.sh
10-listen-on-ipv6-by-default.sh: info: Getting the checksum of /etc/nginx/conf.d/default.conf
10-listen-on-ipv6-by-default.sh: info: Enabled listen on IPv6 in /etc/nginx/conf.d/default.conf
/docker-entrypoint.sh: Launching /docker-entrypoint.d/20-envsubst-on-templates.sh
/docker-entrypoint.sh: Launching /docker-entrypoint.d/30-tune-worker-processes.sh
/docker-entrypoint.sh: Configuration complete; ready for start up
2023/10/08 16:58:45 [notice] 1#1: using the "epoll" event method
2023/10/08 16:58:45 [notice] 1#1: nginx/1.24.0
2023/10/08 16:58:45 [notice] 1#1: built by gcc 10.2.1 20210110 (Debian 10.2.1-6) 
2023/10/08 16:58:45 [notice] 1#1: OS: Linux 6.5.5-200.fc38.x86_64
2023/10/08 16:58:45 [notice] 1#1: getrlimit(RLIMIT_NOFILE): 1073741816:1073741816
2023/10/08 16:58:45 [notice] 1#1: start worker processes
2023/10/08 16:58:45 [notice] 1#1: start worker process 29
2023/10/08 16:58:45 [notice] 1#1: start worker process 30
2023/10/08 16:58:45 [notice] 1#1: start worker process 31
2023/10/08 16:58:45 [notice] 1#1: start worker process 32
2023/10/08 16:58:45 [notice] 1#1: start worker process 33
2023/10/08 16:58:45 [notice] 1#1: start worker process 34
2023/10/08 16:58:45 [notice] 1#1: start worker process 35
2023/10/08 16:58:45 [notice] 1#1: start worker process 36
```