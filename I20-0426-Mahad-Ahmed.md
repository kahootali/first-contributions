Q1. Differences between Docker Containers and VMs

Ans.

1- VMs are hardware level virtualization and provide abstraction of physical hardware. Docker containers provide OS level virtualization at the application layer.

2- VMs are isolated but their applications are not. Whereas in Docker containers both the containers and their applications are isolated.

3- VMs have static compute and static memory whereas Docker containers have burstable compute and burstable memory.

------------------------------------------------------------------

Q2. Docker Command

// Create a network
sudo docker network create assignment-2

// Create a docker container
sudo docker run -d --name assignment-2-I200426 -p 9090:80 --network assignment-2 nginx:1.24.0

//Screenshot Attached as image.png

Q3. 


