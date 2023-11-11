Q1 : Explain Docker Containers vs VMs


Containers
● Operating System-level virtualization, commonly referred to as containerization, functions at the application layer. It bundles both the application code and its prerequisites into a self-contained entity.
● Containers utilize the underlying hardware resources and the host operating system kernel, with the option for an isolated operating system environment if necessary.
● Container images are notably compact, typically ranging in size from tens to hundreds of megabytes, contributing to their efficiency in terms of storage.
● Containers deliver a robust level of isolation, guaranteeing that the applications housed within them do not disrupt one another.
● Key attributes of containers encompass isolation, shared kernel, the capacity to allocate burstable computing and memory resources, and efficient utilization of system resources.


VMs
● Hardware-Level Virtualization involves the abstraction or creation of a virtual representation of physical computer hardware.
● In this setup, multiple virtual machines (VMs) share the same physical hardware but operate independently with their own operating systems.
● Each VM consists of a comprehensive set of components, encompassing a full operating system, application software, binaries, and libraries.
● VMs can consume a substantial amount of storage space, often necessitating several gigabytes (GBs) or even tens of GBs each.
● VMs are isolated from one another, ensuring that actions or problems within one VM typically have no impact on other VMs running on the same hardware.
● VMs mimic complete operating systems and provide a fixed allocation of computing resources and memory. This can lead to high resource consumption since each VM has its dedicated resource allocation.




Q2 : Write command to create a docker container in detached mode with name assignment-2-<ROLL_NUMBER> running on host port 9090 and container port 80 using image nginx with version 1.24.0 on a custom network named assignment-2


Ans: 

docker run -d --name assignment-2-I18-0689 -p 9090:80 nginx:1.24.0 --network assignment-2