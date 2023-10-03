# Q1)  
##### Isolation
Each Virtual Machines runs it's own Operating System with it's own kernet & resources.
Docker Containers share the host kernel. The application & it's dependencies are packaged together using the underlying kernel as the host.
##### Resource Efficieny 
VMs are resource intensive and their resources are fixed.
Containers have burstable memory which can expand and shrink as needed.
Furthermore, as containers share host kernel & resources, they are comparatively very lightweight.
##### Startup Time
VMs take longer because they have to boot an entire Operating System.
Therefore, containers start up almost instantly.

# Q2)
docker network create assignment-2
docker container run -d --publish 9090:80 --name assignment-2-I20-2448 --network assignment-2 nginx:1.24.0