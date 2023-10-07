# Answers for Questions in Assignment#2

# Q1
- In virtual machines the virtualization is hardware based therefore having its own kernel and OS whereas in       Containers OS level virtualization takes place allowing it to share Host kernel.
- In virtual machines libraries and dependancies have to be installed seperately whereas in Containers they come pre-installed.
- Virtual Machines have static compute and memory whereas Containers have burstable compute and memory.
- Virtual Machines are isolated themself not their applications whilst in Containers both the container itself and their respective applications are isolated.

# Q2
- "docker network create assignment-2" used for creating a network named assignment-2
- "docker run -d --name assignment-2-I20-0792 -p 9090:80 --network assignment-2 nginx:1.24.0" used to run container
where:
-d: Runs the container in detached mode, meaning it runs in the background.
--name assignment-2-I20-0792: Specifies the name of the container.
-p 9090:80: Maps port 9090 on the host to port 80 on the container.
--network assignment-2: Connects the container to the custom network named assignment-2.
nginx:1.24.0: Specifies the image to use nginx version 1.24.0.