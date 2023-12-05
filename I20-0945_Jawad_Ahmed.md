-------------------------------------------------------
Jawad Ahmed
I20-0945
CS-B
Dev Ops
Assignment 2 
--------------------------------------------------------

Task : 1

Q. VMs vs. Containers
-----------------------
Ans.

Virtual Machines: 

1. Virtual Machines are hardware level virtualization.They provide abstraction of the physical hardware.
2. Virtual Machines share physical hardware but contains their own Operating System.
3. Each VM has a full copy of an operating system , application ,binaries and  libraries.
4. VMs have complete Operating System , Static Compute, Static Memory, High Resource Usage.

Containers: 

1. Containers have Operating Systems level virtualizations. They have abstraction at the application level.
2. Containers share physical hardware and Host OS Kernel.
3. Containers have Container Isolation, Shared Kernel, Burstable Compute, Burstable Memory and Low Resource Usage.
4. Containers are Isolated and so are the apps.


---------------------------------------------------------------------------------------------------


Task2:

Q.
---------------------

Ans.

docker container run -d --publish 9090:80 --name assignment2-I20-0945 --network assignment-2 nginx:1.24.0




---------------------------------------------------------------------------------------------------


Task3:

Q.

Ans.

The docker container (assignment2-I20-0945) and the logs of containers is attached with the following directory.

---------------------------------------------------------------------------------------------------
