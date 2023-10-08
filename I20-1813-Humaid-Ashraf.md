Q1) Explain Docker Containers vs VMs

Ans:
Docker containers offer a lightweight form of virtualization. They abstract the application layer, bundling code and dependencies, and share the host's operating system kernel. This makes them highly efficient in terms of resource usage, typically requiring only tens to hundreds of megabytes in size. Containers provide isolation at the process level, ensuring that applications run independently within them. Docker containers are known for their portability and quick deployment, making them an ideal choice for microservices architectures.

On the other hand, virtual machines (VMs) provide a more traditional form of virtualization. Each VM includes its own complete operating system, application stack and libraries. VMs abstract the physical hardware, offering stronger isolation as they run separate operating systems. However, this comes at the cost of higher resource consumption, with VMs typically needing tens of gigabytes in storage and memory. VMs are often preferred for running legacy applications or when strict isolation is required, but they are less efficient in terms of resource utilization compared to containers.

Q2) Write command to create a docker container in detached mode with name assignment-2-<ROLL_NUMBER> running on host port 9090 and container port 80 using image nginx with version 1.24.0 on a custom network named assignment-2

-sudo docker network create assignment-2
-sudo docker run -d -p 9090:80 --name assignment-2-I20-1813 --network assignment-2 nginx:1.24.0
-sudo docker logs assignment-2-I20-1813

Q3) Run the above command and add screenshot of it and share the logs

Sccrenshots attached in the folder.
