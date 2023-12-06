Q1) Explain Docker Containers vs VMs:

Docker Containers and Virtual Machines (VMs) are both technologies used 
for running applications in isolated environments, but they operate differently:

Docker Containers:

Containers are lightweight and share the host OS kernel.
They package an application and its dependencies together.
Containers start quickly and use fewer resources.
Ideal for microservices architecture and scaling applications.

VMs (Virtual Machines):

VMs are more like running a full operating system.
They run multiple applications on top of a hypervisor.
VMs are slower to start and use more resources.
Suitable for running different OS types and legacy applications. 

Q2) Write command to create a docker container in detached mode with name assignment-2-<ROLL_NUMBER> 
running on host port 9090 and container port 80 using image nginx with version 
1.24.0 on a custom network named assignment-2:

docker run -d --name assignment-2-i20-0538 -p 9090:80 --network assignment-2 nginx:1.24.0

![Screenshot](https://imgur.com/a/gsopNEa)





