Q1 : Explain Docker Containers vs VMs


Containers
● OS level virtualization, also known as containerization, operates at the application layer. It encapsulates both the application code and its dependencies into a self-contained unit.
● Containers share the underlying hardware resources and the host operating system kernel, but they can have their own isolated operating system environment if needed.
● Container images are relatively compact, typically ranging from tens to hundreds of megabytes in size, making them efficient in terms of storage.
● Containers offer a high degree of isolation, ensuring that the applications running within them do not interfere with each other.
● Key characteristics of containers include isolation, shared kernel, the ability to allocate burstable compute and memory resources, and efficient utilization of system resources.


VMs
● Hardware-Level Virtualization refers to the concept of abstracting or creating a virtual representation of physical computer hardware.
● Shared Hardware with Own OS, i-e multiple virtual machines (VMs) share the same physical hardware but each VM runs its own independent operating system.
● Each VM contains a complete set of components, including a full operating system, application software, binaries, and libraries.
● VMs can consume a significant amount of storage space, often requiring several gigabytes (GBs) or even tens of GBs each.
● VMs are isolated from each other, meaning that actions or issues in one VM typically do not affect other VMs running on the same hardware.
● VMs emulate complete operating systems and offer a static allocation of compute resources and memory. This can result in high resource usage, as each VM has its own dedicated allocation of these resources.




Q2 : Write command to create a docker container in detached mode with name assignment-2-<ROLL_NUMBER> running on host port 9090 and container port 80 using image nginx with version 1.24.0 on a custom network named assignment-2


Ans: 

docker run -d --name assignment-2-I19-0444 -p 9090:80 nginx:1.24.0 --network assignment-2
