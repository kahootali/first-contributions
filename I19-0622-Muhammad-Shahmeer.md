Q1 Explain Docker Containers vs VMs
Answer:
Docker Containers:
1.Docker containers are lightweight because they share the host operating system's kernel.
2.Containers provide process-level isolation.
3.Docker containers are highly portable. You can create a container image on one system and run it on another as long as the target system supports Docker.
4.Containers consume fewer resources than VMs because they don't require a full OS for each instance.

Virtual Machines (VMs):
1.VMs are typically heavier compared to containers because they run a full guest OS in addition to the application and its dependencies. Each VM includes its own kernel and system libraries.
2.VMs provide stronger isolation since they run separate guest OS instances.
3.VMs are less portable than containers. Moving a VM between different hypervisors or cloud platforms can be more challenging due to differences in virtualization technologies.
4.VMs consume more system resources because of the additional overhead of running multiple OS instances.

Q2 Write command to create a docker container in detached mode with name assignment-2-<ROLL_NUMBER> running on host port 9090 and container port 80 using image nginx with version 1.24.0 on a custom network named assignment-2
Answer: 
docker run -d --name assignment-2-I19-0622 -p 9090:80 --network assignment-2 nginx:1.24.0

Q3 Run the above command and add screenshot of it and share the logs
