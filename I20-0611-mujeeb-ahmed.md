Q1 
Imagine we want to live in a house and want to build it . Each House or we call it VM has its own foundation such as walls,plumbing electricity etc. It has full operating system and resources.Each house will be independent of each other.Each house building will take time and resources and have their own infrastructure.If we talk about Docker,imgagine a apartment building,instead of many houses,we have one building (host system) and on top of that we have many apartments.All of the apartment share the same foundation ,system and resources but have seperate bedrooms kitchen etc.Now lets talk about it in tehcnical terms.Vms are more resource intensive and require alot of resources where as docker containers are light weight and faster.Container take OS-level virtualization where as VM offer hardware-level virtualization.VM run seperate full oeprating system where as docker container shares hsot kernel.

Q2
sudo docker network create assignmentdevops-2
sudo docker run -d --name assignment2-I20-0611 -p 9090:80 --network assignmentdevops-2 nginx:1.24.0

Q3
sudo docker logs assignment2-I20-0611 > container_logs.txt
2023/10/08 16:41:24 [notice] 1#1: using the "epoll" event method
2023/10/08 16:41:24 [notice] 1#1: nginx/1.24.0
2023/10/08 16:41:24 [notice] 1#1: built by gcc 10.2.1 20210110 (Debian 10.2.1-6) 
2023/10/08 16:41:24 [notice] 1#1: OS: Linux 6.2.0-34-generic
2023/10/08 16:41:24 [notice] 1#1: getrlimit(RLIMIT_NOFILE): 1048576:1048576
2023/10/08 16:41:24 [notice] 1#1: start worker processes
2023/10/08 16:41:24 [notice] 1#1: start worker process 29

