Q1) Explain Docker Containers vs VMs

Ans 1) Containers: Containers provide OS level virtualization i.e. abstraction at
the app layer (code + dependencies). Containers share the host OS kernel and so many containers can be run on the same host eg. Alpine, CentOS containers can be run on ubuntu host OS. They take up less space (typically tens to hundreds of MBs in size) compared to VMs and are quick to start up.

VMs: VMs provide Hardware level virtualization i.e. abstraction of physical hardware. They share Hardware but have own OS. Each VM has a full copy of an operating system + application + binaries + libraries. They can take upto tens of GBs and hence are slower to boot up than containers.

Q2) Write command to create a docker container in detached mode with name assignment-2-<ROLL_NUMBER> running on host port 9090 and container port 80 using image nginx with version 1.24.0 on a custom network named assignment-2

Ans 2) docker run -d --name assignment-2-I20-1822 -p 9090:80 --network assignment-2 nginx:1.24.0

Q3) Run the above command and add screenshot of it and share the logs
