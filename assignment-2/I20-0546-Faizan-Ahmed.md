Answer 1:-

*Containers*

Containers take an OS-level virtualization approach. They abstract at the application layer by bundling code and its dependencies together into compact packages. Containers share the host hardware and OS kernel but can have their own OS components if necessary. They're far more space-efficient, usually clocking in at tens to hundreds of megabytes.

Containers offer application-level isolation, a shared kernel, burstable compute and memory, and keeps resource usage low. It simplifies Ops' job as they only need to create VMs and install Docker. Developers write code, test it locally in a container based on the same image, and then deploy that exact image in different environments. This approach  reduces compatibility issues and entirely eliminates the "Works on my machine" issue.

However, isolation in containers is process-level and somewhat less secure compared to VMs.


*Virtual Machines*

VMs, on the other hand, operate on the principle of hardware-level virtualization. They abstract the physical hardware and each VM runs its own full operating system alongside the application, binaries, and libraries. As a result, VMs tend to be quite bulky, sometimes taking up tens of gigabytes. VMs are isolated from one another , unlike applications, providing complete OS isolation. However, they're pretty static when it comes to resource allocation, and they demand a significant amount of resources.

From an operational perspective, VMs are the responsibility of Ops. Ops not only create VMs but also deal with installing software dependencies and software itself. This can be a bit of a problem due to potential compatibility issues. On the other hand, developers write their code and test it on their local machines, which can lead to "Works on my machine" issue.

Answer 2:-

sudo docker network create assignment-2
sudo docker run -d --name assignment-2-I20-0546 -p 9090:80 --network assignment-2 nginx:1.24.0

Answer 3:-

faizan@faizan-VirtualBox:~$ sudo docker logs assignment-2-I20-0546 > container_logs.txt
2023/10/07 22:31:05 [notice] 1#1: using the "epoll" event method
2023/10/07 22:31:05 [notice] 1#1: nginx/1.24.0
2023/10/07 22:31:05 [notice] 1#1: built by gcc 10.2.1 20210110 (Debian 10.2.1-6) 
2023/10/07 22:31:05 [notice] 1#1: OS: Linux 6.2.0-34-generic
2023/10/07 22:31:05 [notice] 1#1: getrlimit(RLIMIT_NOFILE): 1048576:1048576
2023/10/07 22:31:05 [notice] 1#1: start worker processes
2023/10/07 22:31:05 [notice] 1#1: start worker process 29
2023/10/07 22:31:05 [notice] 1#1: start worker process 30
2023/10/07 22:31:05 [notice] 1#1: start worker process 31
2023/10/07 22:31:05 [notice] 1#1: start worker process 32
