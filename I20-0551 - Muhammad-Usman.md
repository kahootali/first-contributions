Q1: 
Containers: 
1. Abstraction Level: Containers abstract the application layer, encompassing code and dependencies.
2. Resource Sharing: They utilize shared hardware resources and the host OS kernel.
3. Size: Typically compact, ranging from tens to hundreds of gigabytes.
4. Isolation: Containers maintain isolation, enabling different programs to operate.
5. Key Features: Known for efficiency, shared OS kernel, adaptable computation and memory, and distinct containerization.

VMs (Virtual Machines):
1. Abstraction Level: VMs abstract the hardware level, creating virtual versions of physical resources.
2. Resource Sharing: Each VM possesses its independent OS, applications, and libraries.
3. Size: VMs can be substantial, taking up tens of gigabytes individually.
4. Isolation: VMs are isolated, but their programs may not be.
5. Key Features: Feature full OS, static computation and memory, and consume significant resources.

Q2:
docker network create assignment-2
docker run -d --name assignment-2-I20-0551 -p 9090:80 --network assignment-2 nginx:1.24.0