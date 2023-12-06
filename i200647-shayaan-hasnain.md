Q1: DOCKER CONTAINERS VS VMS:

Docker Containers:
Containers are lightweight and share the host OS kernel. They package an application and its dependencies into a single unit.
They are more resource-efficient compared to VMs because they don't require a full OS for each container.
Containers are faster to start and stop, making them suitable for microservices architectures and rapid scaling.
Docker containers are highly portable and can run consistently across different environments, thanks to containerization.

Virtual Machines (VMs):
VMs are heavier because they include a full OS and virtualized hardware.
Each VM runs its own independent OS and kernel, which can lead to more resource consumption.
VMs are slower to start and require more resources than containers.
They are less portable compared to containers because VM images are tied to specific virtualization platforms.
In summary, Docker containers are ideal for lightweight, isolated application deployment, whereas VMs provide greater isolation but with higher resource overhead.

Q2:

docker run -d --shayaanhasnain assignment-2-I20-0647 -p 9090:80 --network assignment-2 nginx:1.24.0
