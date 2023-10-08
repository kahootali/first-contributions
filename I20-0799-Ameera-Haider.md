**Q1) Docker Containers vs VMs**

**Docker Containers:**
- Docker containers are lightweight, portable, and self-contained packages that can run applications and their dependencies.
- They utilize the host operating system's kernel and isolate the application from the rest of the system.
- A Docker container includes everything an application needs to run, such as code, libraries, runtime, and system tools.
- Containers are fast to start, use fewer resources, and are highly portable because they can run on any system that supports Docker.

**Virtual Machines (VMs):**
- VMs are virtual computers that run an operating system and applications just like a physical computer.
- Each VM includes a complete operating system and a hypervisor, which is software that manages VMs.
- VMs are isolated from each other and from the host system.
- They are more resource-intensive compared to containers because they need to run a full OS.

**Comparison:**

- **Resource Efficiency:**
  - Containers share the host OS kernel, making them lightweight and efficient in terms of resource usage.
  - VMs require a separate OS for each instance, consuming more resources and memory.

- **Isolation:**
  - Containers provide process-level isolation, meaning each containerized application is isolated from others running on the same host system.
  - VMs offer stronger isolation since they run separate OS instances, providing a higher level of security and independence between VMs.

- **Startup Speed:**
  - Containers can start almost instantly since they don't need to boot an entire operating system.
  - VMs take longer to start because they need to boot a complete OS.

**Q2) Docker Container Creation Command**

To create a Docker container in detached mode with a specific name, host port, container port, using a specific image, and on a custom network, you can use the following command:

```sh
docker run -d --name assignment-2-I20-0799 -p 9090:80 --network assignment-2 nginx:1.24.0
```

**Q3) Docker Container Creation and Screenshot**

Screenshots of the Docker container creation command and the logs have been added to the repository.