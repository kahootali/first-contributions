Q1) Explain Docker Containers vs VMs

* VMs have hardware level virtualization while containers have OS level virtualization.
* VMs have static compute, static memory while containers have burstable compute and burstable memory.
* VMs provide strong isolation because they run separate operating systems. This makes them suitable for running different OS versions or multiple applications with conflicting dependencies.
* Containers offer a lower level of isolation since they share the host OS kernel. While this makes them more lightweight, it also means that containers may not provide the same level of security and isolation as VMs in certain scenarios.

Q2) Write command to create a docker container in `detached` mode with name `assignment-2-<ROLL_NUMBER>` running on host port `9090` and container port `80` using image `nginx` with version `1.24.0` on a custom network named `assignment-2`

* sudo docker network assignment-2
* sudo docker run -d --name assignment-2-I20-0542 -p 9090:80 --network assignment-2 nginx:1.24.0

Q3) Run the above command and add screenshot of it and share the logs

![1696696205791](image/I20-0542-BILAL-KHAN/1696696205791.png)
