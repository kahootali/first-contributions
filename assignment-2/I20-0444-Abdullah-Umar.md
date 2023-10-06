# Answers to Questions for Assignment 2
## Abdullah Umar 20i-0444

## Q1

- In Containers, host kernel is shared whereas in VM's, it has it's own kernel and entire OS.
- Containers come with their own binaries and dependancies whereas in VM's, they have to be installed separately.
- VM's are more secure since hardware virtualization is done in it whereas containers are less secure because the virtualization is on a software level.
- VM's require more memory than containers.


## Q2

1. First to create the network we run:-

**docker network create assignment-2**

2. Then we run the container for this case with the following command:-

**docker run -d --name assignment-2-I20-0444 --network assignment-2 -p 9090:80 nginx:1.24.0**

Here, -d is for running in detached state, --name flag is used to specify the name of running container, --network flag is for specifying which network this container belongs to, -p is used to specify that container runs on host port 9090 and container port 80, and nginx:1.24.0 is the image we want to run


## Q3

<img src="../docker command.PNG" title="Command run in terminal">
<img src="../nginx working.PNG" title="Screen of working container on 9090 port">
<img src="../docker logs.PNG" title="Logs of container working">
