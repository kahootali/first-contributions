Q1 Answer:
Containers provide Operating System level virtualization while virtual machines provide hardware level virtualizaiton. This means that while both containers and VMs share hardware, containers additionally share the kernel of the host OS. Hence, Containers are relatively light weight because they contain only the necessary code and dependencies required while each VM has full copy of the OS, application code, binaries and libraries. Containers have burstable memory, meaning they can use more memory than its reserved amount when additional memory is available on the host system. VMs on the other hand cannot use more memory than what has been reserved for them. 
Q2 Answer:
docker run -d --name assignment-2-I20-0768 -p 9090:80 --network assignment-2 nginx:1.24.0
Q3 Answer:
Screenshots uploaded