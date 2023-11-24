Question 1: Difference bw Container & VMs.

Ans. VMs are hardware level virtualization , Containers are OS level Virtualiztaion. VMs share hardware, have their own OS. Containers share hardware as well as kernal of host OS. Containers bring application and all the required dependencies for it. Manual Installation of Application and Dependencies are required for VMs. VMs take more space, static compute, static memory and high resource usage. Containers take lesser space , Burstable compute, Burstable memory and low resouce usage.

Question 2:

docker run -d --name assignment-2-I20-0548 -p 9090:80 --network assignment-2 nginx:1.24.0
