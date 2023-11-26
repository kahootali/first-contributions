Question#1:
Explain Docker Containers vs VMs.

VMs                                                          Containers 
VMs provide Hardware level virtualization.                  While Containers provide OS level virtualization.
VMs are more secure                                         Containeres are less secure
They offer static compute and static Memory                 They offer Burstable compute and burstable memory
Ops have to create VMs and install Software dependencies    While Ops only create VMs and install Docker only
along with softwares
VMs have work on my machine issue                           No work on my machine issue


Question#2:
Command to create a Docker container in detached mode
docker run -d --name assignment-2-<I200861> -p 9090:80 --network assignment-2 nginx:1.24.0



