Docker Containers:
Docker Containers share the OS kernel of the host system and package a program with all of its necessary libraries and binaries. As a result, containers are very efficient, lightweight, and enable quick startup times. Multiple containers can run on the same machine and use less resources than virtual machines because they share the host OS.

Virtual Machines(VMs):
A virtual machine (VM) is a model of a computer system that runs a separate operating system from the host. Although it offers stronger isolation because it runs its own complete OS, it is typically larger and uses more resources than containers. Because they are independent entities, VMs frequently result in duplicated OS overhead and slower boot times, especially when several VMs are used at once.


Docker Command: 
docker run -d --name assignment-2-I19-2167 -p 9090:80 --network assignment-2 nginx:1.24.0

![Screenshot of Docker Command](https://ibb.co/fNnMNcj)
