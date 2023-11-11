Answer 1:
Docker Container are lightweight virtualizations that share the host kernel. They are much smaller in size and are faster to start than VMS. They are more
resource efficient since they share host's kernel and libraries but less secure than VMs because containers are less isolated than VMs.

VMS on the other hand are heavyweight virtualizations that have their own OS. They are bigger in size and are slower to load since they need to boot their OS.
They are are not resource efficient since they have their own OS but are more isolated and hence, more secure than docker containers.




Answer 2:

docker network create assignment-2 && docker run -d -p 9090:80 --name assignment-2-I20-0440 --network assignment-2 nginx:1.24.0




Answer 3:
![Screenshot of Task2](image.png)
