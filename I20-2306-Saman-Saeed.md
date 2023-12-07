Q1.

Docker Containers :

1. OS level virtualization
2. Burstable memory, burstable compute
3. Shares kernel of the host VM
4. Have own binaries and libraries
5. Lighweight and portable
6. No "Works on my machine" issue

VMs:

1. Hardware level virtualization
2. Static memory, static compute
3. Has its own copy of OS
4. Need to install binaries and libraries
5. Heavyweight and non-portable
6. "Works on my machine" issue

Q2:

Creating a docker network
docker network create assignment-2

docker run -d --name assignment-2-I20-2306 --network assignment-2 -p 9090:80 nginx:1.24.0

Q3:
![Alt text](image.png)
