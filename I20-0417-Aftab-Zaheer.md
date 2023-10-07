#Assignment 2 Questions and Answers

Q1. Explain Docker Containers vs VMs

Ans. 
The major difference between both are that the docker container shares the existing infrastructure of the machine it is installed on as it shares the OS kernel of the host machine. However, in the case of VMs, it brings its own infrastructure as each VM has a full fledged OS with all its libraries, applications, binaries as well as libraries. This makes the VM heavyweight as it may take many GBs per instance, but in the case of Docker Container, it basically shares the OS kernel as mentioned above, and bring along the application code along with their dependancies. This makes them lightweight and faster to boot as compared to VMs. Another major difference between them is that the Containers enable burstable computing which allows them to increase the number of CPUs used to ensure load balancing in peak usage which allows them to be more responsive. However, this is not the case with VMs, as they only offer static computing, meaning once the CPUS assigned, they cannot be exceeded unless manually adjusted by the users themselves, and it also requires restarting the VM therefore maintaining a rigid structure. Another major difference between the two is that the Ops using VMs are required to keep the OS on the VM up to date and the softwares installed up to date to ensure no compatibility issues arise. They also are responsible for ensuring that their softwares work with newly installed libraries. However, this responsibility of Ops is reduced by the containers as they are only required to install the docker containers and the issues of compatibility will not arise.

Q2. Write command to create a docker container in detached mode with name assignment-2-<ROLL_NUMBER> running on host port 9090 and container port 80 using image nginx with version 1.24.0 on a custom network named assignment-2

Ans.
docker run -d --name assignment-2-I20-0417 -p 9090:80 --network assignment-2 nginx:1.24.0


Q3. Run the above command and add screenshot of it and share the logs

Ans.
Screenshots of the command running have been added to the GCR. commands of checking logs are below
sudo docker logs assignment-2-I20-0417


