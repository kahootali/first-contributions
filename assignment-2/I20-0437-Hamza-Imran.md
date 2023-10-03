##### Q1) Explain Docker Containers vs VMs
**Ans)** VM's provide an abstraction layer over the hardware while containers provide an absdtraction layer at the app level. In containers we are provided with all the required dependencies whereas in VM's we have to install them by ourselves. Containers tend to be in smaller sizes a matter of MB's, while VM's tend to be in the range of 2GB+. In VM's each machine has their own kernal, while in Containers each container share the OS kernel with each other. Since containers is packaged with all the required dependencies we don't get the issues such as it works on my machine, while in VM's we tend to get such issues.

##### Q2) Write command to create a docker container in detached mode with name assignment-2-<ROLL_NUMBER> running on host port 9090 and container port 80 using image nginx with version 1.24.0 on a custom network named assignment-2
**Ans)** 
###### For creating network assignment-2
``` docker network create assignment-2```
###### For creating container
```docker container run -d --publish 9090:80 --name assignment-2-I20-0437 --network assignment-2 nginx:1.24.0```