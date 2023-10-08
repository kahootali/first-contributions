#225

Q1) Explain Docker Containers vs VMs

Docker containers are a lightweight and efficient way to package and run applications, making them suitable for modern, agile, and scalable software development. VMs provide stronger isolation and are a good choice when you need to run different OS versions or have specific hardware requirements.

Isolation :
Virtual Machines (VMs): Each VM runs its own operating system with its own kernel and resources, providing strong isolation between VM instances.
Docker Containers: Containers share the host kernel, isolating applications and dependencies within the container while sharing the underlying kernel, making them lightweight.

Resource Efficiency :
Virtual Machines (VMs): VMs are resource-intensive, with fixed resource allocations for each instance.
Docker Containers: Containers are resource-efficient, with burstable memory that can expand and shrink as needed. They are lightweight due to sharing host resources.

Startup Time :
Virtual Machines (VMs): VMs take longer to start because they need to boot an entire operating system.
Docker Containers: Containers start up almost instantly since they don't require booting a full OS.

Q2)
For this question I have used these commands.

docker --version
docker run -d --name assignment-2-I190431 -p 9090:80 --network assignment-2 nginx:1.24.0
