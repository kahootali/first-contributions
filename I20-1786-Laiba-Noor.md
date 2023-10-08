Q1) Explain Docker Containers vs VMs

VMS:
Vms provide hardware level virtualization,each having its own os and takes alot of space. It offers Static Compute, Static
Memory and High Resource Usage. There is "Work on my machine" issue in Vm.
Containers:
Containers provide Os level virtualization, sharing the host OS's kernel.It offers container level isolation, Shared Kernel,
Burstable Compute,Burstable Memory and Low Resource Usage.It solves "Work on my machine issue" as same image is deployed in staging and production.

Q2) Write command to create a docker container in detached mode with name assignment-2-<ROLL_NUMBER> running on host port 9090 and container port 80 using image nginx with version 1.24.0 on a custom network named assignment-2
docker run -d --name assignment-2-I20-1786 -p 9090:80 nginx:1.24.0 --network assignment-2

Q3) Run the above command and add screenshot of it and share the logs
https://imgur.com/a/oNze6tf
