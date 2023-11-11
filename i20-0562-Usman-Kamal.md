Assignment 2 Answers:


Question 1: Explain Docker Containers vs VMs

Answer 1: Docker Containers and VMs may serve a similar prupose but they have some fundamental differences that are given below:
1. Containers are lightweight becase they share the OS kernel. A container uses host OS for system calls. On the other hand, VMs are heavyweight because each VM contains a full OS.
2. Containers provide us with process and file system isolation whereas VMs provide full isolation. Each VM runs its own OS.
3. Containers use few resources because they don't require a full OS. On the other hand, VMs consumes more resources because each VM runs a complete OS.
4. Containers are very fast in speed and start almost instantly. Vms take longer because they need to start a complete OS.




Question 2: 

For this, we will use the following command:
docker run -d --name assignment-2-I20-0562 -p 9090:80 --network assignment-2 nginx:1.24.0


Question 3:
Screenshots are attached in the same folder as this.
