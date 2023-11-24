Q1) Explain Docker Containers vs VMs.
Ans) Virtual machines (VMs) operate at the hardware level, providing an abstraction layer over physical hardware to create separate environments. Each VM has its own complete operating system, applications, and libraries. However, VMs tend to be resource-intensive, often requiring significant storage space, making them suitable for static workloads. While VMs offer strong isolation between VMs, they may face challenges in achieving isolation between applications within the same VM. This can lead to compatibility issues between development and operations teams.

In contrast, containers are based on OS-level virtualization, abstracting at the application layer, which includes both the application code and its dependencies. Containers share the host OS kernel, making them highly efficient and lightweight, typically consuming only a fraction of the resources compared to VMs. Containers excel in providing robust isolation at the application level, ensuring that different applications remain completely isolated from one another. They are particularly well-suited for dynamic workloads and address the common problem of "it works on my machine" by enabling developers to create, test, and deploy applications consistently across different environments.

Q2) Write command to create a docker container in detached mode with name assignment-2-<ROLL_NUMBER> running on host port 9090 and container port 80 using image nginx with version 1.24.0 on a custom network named assignment-2
Ans) docker network create assignment-2

docker run -d -p 9090:80 --name assignment-2-I20-0507 --network assignment-2 nginx:1.24.0

Q3) Run the above command and add screenshot of it and share the logs
Ans) ![](Screenshot.PNG)
