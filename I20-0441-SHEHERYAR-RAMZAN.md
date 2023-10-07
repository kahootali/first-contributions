Q1) Explain Docker Containers vs VMs

A1: Containers provide OS-level virtualization, abstracting at the application level and packaging both code and dependencies. They offer process-level isolation while sharing the host OS kernel, resulting in efficient resource utilization and quick scalability. Containers are known for burstable compute and memory. In contrast, virtual machines (VMs) use hardware-level virtualization, abstracting at the physical layer, running complete guest OS instances. VMs consume more resources, often requiring tens of gigabytes of storage, and have slower boot times. However, they are favored for their strong isolation and security, as any compromise in one VM does not affect others. 

Q2) Write command to create a docker container in detached mode with name assignment-2-<ROLL_NUMBER> running on host port 9090 and container port 80 using image nginx with version 1.24.0 on a custom network named assignment-2

A2: docker container run -d -p 9090:80 --name assignment-2-I20-0441 --network assignment-2 nginx:1.24.0

Q3) ![SS of above command](image.png)
![SS of logs](image-1.png)