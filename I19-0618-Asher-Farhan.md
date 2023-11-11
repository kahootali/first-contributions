Q1) Explain Docker Containers vs VMs?
ANS: 

    DOCKER CONTAINERS:
-> Docker contaienrs are light weight containers that share host OS kernel.
-> Conatiners usually have eficeint resource usage. They can run on a single host.
-> Containers dont require entire OS to boot up so they can start quickly.
-> Docker containers can easily be managed.
-> Containers are ideal for microservices architecture.
-> Containers are lightweight, efficeint and portable solution for modern applications.

    VM:
-> VMs are usually heavyweight because they tend to run full OS.
-> VMs consume more resource and CPU usage which lags the perfomance of host machines.
-> There is a strong isolation on VM since each VM run on separate OS.
-> VMs take longer time to start as comapred to containers.
-> VMs are less portable than OS.
-> VMs are typically used for running larger, monolithic applications.

Q2) Write command to create a docker container in detached mode with name assignment-2-<ROLL_NUMBER> running on host port 9090 and container port 80 using image nginx with version 1.24.0 on a custom network named assignment-2?

ANS: 

    docker run -d --name assignment-2-I19-0618 -p 9090:80 --network assignment-2 nginx:1.24.0

    