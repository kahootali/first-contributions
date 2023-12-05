1) The main differences between Docker containers and VM’s are:
Docker containers share OS kernel, and have OS level virtualization, while VMs have their own kernels and have hardware level virtualization.
Docker containers have burstable memory and compute power while VMs have static memory and compute power
Vms come with libraries pre installed while you have to install libraries in containers.

2)  
docker network create assignment-2
docker run -d --name assignment-2-I20-0518 -p 9090:80 --network assignment-2 nginx:1.24.0
first command creates custom network
-d: runs in detached mode 
 --name assignment-2-I20-0518: specifies container name 
-p 9090:80: maps port 9090 on host to port 80 on container
–network: assigns to custom network 
Nginx:1.24.0: defines nginx version

3)
![image](first-contributions\assignment-2\making-docker-container.png)