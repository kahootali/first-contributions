Q1) Explain Docker Containers vs VMs
Ans) Virtual machines (VMs) and Docker containers are two different methods for managing and deploying applications.  Containers, like Docker, operate at the operating system level, sharing the host OS kernel while isolating user spaces. As a result, they are ideal for scaling applications, very effective at utilizing resources, and rapid to start and stop. However, because of the same kernel, they offer process-level isolation and can have similar security issues. With the ability to package apps and dependencies into a single container image for consistent behavior across different environments, containers are very portable.

In contrast, virtual machines that run on a hypervisor replicate whole operating systems and offer higher isolation and security. VMs are appropriate in situations needing stronger isolation and interoperability with several operating systems, but they are larger and more expensive. When numerous VMs run on the same physical host, they take longer to start up and potentially waste resources. Your unique application requirements will determine whether you choose VMs or Docker containers; containers are preferred for their portability, agility, and efficiency, while VMs are preferred for their improved isolation and OS compatibility.


Q2) Write command to create a docker container in detached mode with name assignment-2-<ROLL_NUMBER> running on host port 9090 and container port 80 using image nginx with version 1.24.0 on a custom network named assignment-2

Ans) docker run -d --name assignment-2-I20-0856 -p 9090:80 --network assignment-2 nginx:1.24.0

Q3) Run the above command and add screenshot of it and share the logs

