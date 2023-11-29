# Q1 Docker Containers Vs Vms
Docker containers and virtual machines (VMs) are both technologies used for virtualization, but they operate at different levels of abstraction. VMs virtualize the entire hardware stack, allowing multiple operating systems to run on a single physical machine. Each VM includes its own guest OS, consuming more resources and requiring a hypervisor for management. In contrast, Docker containers share the host OS kernel, making them lightweight and efficient. They encapsulate applications and their dependencies, ensuring consistency across different environments. This makes containers faster to start, use fewer resources, and allows for easier scaling. Overall, Docker containers are well-suited for application deployment and microservices architectures, while VMs are better suited for running multiple, diverse applications on the same host.

# Q2 Write command to create a docker container in detached mode with name assignment-2-<ROLL_NUMBER> running on host port 9090 and container port 80 using image nginx with version 1.24.0 on a custom network named assignment-2

```bash
sudo docker network create assignment-2
sudo docker pull nginx:1.24.0
sudo docker run -d -p 9090:80 --network assignment-2 --name assignment-2-I18-0530 nginx:1.24.0
```

# Q3 Share the logs of the command 
```bash
vacaramin@vacaramin-Latitude-E7270:~/Desktop/temp/first-contributions$ sudo docker network create assignment-2
9d393989cd62a77bef164b9be0a59eee079e1cf0ee0a63a07c1181eede144270
vacaramin@vacaramin-Latitude-E7270:~/Desktop/temp/first-contributions$ sudo docker pull nginx:1.24.0
1.24.0: Pulling from library/nginx
Digest: sha256:73341830a31bf12a44c846b6b323dd8a4fab7668e72c16e9124913ff097c9536
Status: Image is up to date for nginx:1.24.0
docker.io/library/nginx:1.24.0
vacaramin@vacaramin-Latitude-E7270:~/Desktop/temp/first-contributions$ sudo docker run -d -p 9090:80 --network assignment-2 --name assignment-2-I18-0530 nginx:1.24.0
3f2872468b2393d15a6dcf78e4805d617ca68e5b86cbf0053fe7a41c1646f9f8
```

