Q1 - Explain Docker Containers vs VMs

a. Docker does OS level virtualization with kernel sharing whereas VMs perform hardware level virtualization and therefore are heavier.
b. Burstable compute used in Docker whereas Static compute and Memory is used in VMs.
c. Developer writes codes and tests on same image which runs on staging and production enviornments so no "works on my machine" issue. 
With VMs, there is no concept of image, dev and op teams work seprately and "works on my machine" issue occurs frequently.

Q2 -  Write command to create a docker container in detached mode with name assignment-2-<ROLL_NUMBER> running on host port 9090 and container port 80 using image nginx with version 1.24.0 on a custom network named assignment-2
docker run -d --name assignment-2-I20-0904 -p 9090:80 --network assignment-2 nginx:1.24.0

