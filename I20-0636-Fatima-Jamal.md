Q1) Explain Docker Containers vs VMs

VMs:
● Hardware level virtualization i.e. abstraction of physical hardware.
● Share Hardware but has own OS.
● Each VM has a full copy of an operating system, application,
binaries and libraries.
● can take up to tens of GBs of space.
● VMs are isolated, apps are not.
● Complete OS, Static Compute, Static Memory and High Resource Usage.
● Works on my machine issue
● More secure than containers.

Containers :
● OS level virtualization i.e. abstraction at the app layer (container has code along with dependencies).
● Share hardware and host OS kernel but can have own OS.
● take up less space (typically tens to hundreds of MBs in size).
● containers are isolated, and so are the apps.
● Have Burstable Compute and Memory and Low Resource Usage.
● Ideally no “Works on my machine” issue.
● Process level isolation but relatively less secure.

Q2) Write command to create a docker container in detached mode with name assignment-2-<ROLL_NUMBER> running on host port 9090 and container port 80 using image nginx with version 1.24.0 on a custom network named assignment-2
docker run -d --name assignment-2-I20-0636 --network assignment-2 -p 9090:80 nginx:1.24.0

Q3) Run the above command and add screenshot of it and share the logs
![Screenshot for Q3](https://i.imgur.com/42ysyRa.png) 