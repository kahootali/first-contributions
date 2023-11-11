##Q1) Difference between Docker Containers vs VMs
-VMs provide hardlevel virtualization whereas containers have OS level abstraction.
-Vms share hardware but they have their own OS whereas container can/cannot have their own OS.
-Vms have complete OS and static memory whereas containers have burstable compute and burstable memory.
-Vms are very large in size i.e Gigabytes whereas containers take upto few hundred megabytes.

##Q2) Command to create a docker container in detached mode
docker run -d -p 9090:80 --name assignment-2-I19-1741 --network assignment-2 nginx:1.24.0
