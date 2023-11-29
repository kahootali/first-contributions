Docker Containers:

1) Docker containers are lightweight, standalone, and executable packages that include everything needed to run a software, including the code and libraries etc.
2) Containers use the host operating system's kernel. They isolate the application processes from the rest of the system.
3) They start quickly and use fewer resources.
4) Highly portable across environments.
5) Well-suited for microservices architecture and lightweight applications.

Virtual Machines(VM):
1) VMs run on a hypervisor. Each VM has its own operating system and behaves like a separate physical machine.
2) VMs are heavier in terms of resource usage because they include a full operating system for each instance. This can lead to longer startup times and higher resource consumption.
3) VMs provide strong isolation since each VM runs its own operating system.
4) Portability may be more complex due to dependencies on hypervisors.
5) Commonly used for running multiple applications with different OS requirements.


sudo docker run -d --name assignment-2-I20-0586 -p 9090:80 --network assignment-2 nginx:1.24.0

