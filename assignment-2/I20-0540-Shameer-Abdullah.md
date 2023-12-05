1- Docker Containers and Virtual Machines serve as methods to run applications in isolated environments. Docker Containers are lightweight and use the host OS kernel, isolating only the application processes. This makes them efficient and quick to start. On the other hand, VMs operate with their own full OS, making them heavier and consuming more resources. However, VMs offer stronger isolation since they run on separate kernels. While containers are optimal for scalable, lightweight applications, VMs are more suited for tasks that demand the full resources and functionalities of an entire OS.

2- docker run -d -p 9090:80 --name assignment-2-I20-0540 --network assignment-2 nginx:1.24.0-0540

3- LOGS:
![first](SS1.png)
![second](SS2.png)