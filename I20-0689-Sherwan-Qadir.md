Q1) Explain Docker Containers vs VMs?

Ans: 

-> Virtual Machine is hardware level abstraction whereas Docker Containers are OS level virtualization i.e, abstraction at application layer

-> VM's can take upto 10's of GB's whereas containers take less space like 10's of MB's

-> VM's are isolated, applications are not isolated whereas in containers both containers and applications are isolated

->In VM's operations were responsible for vreating VM's, installing dependencies and than software which might not run due to compatibility issues whereas Developers were responsible to run it on local machine. It created works on my machine issue whereas in case of containers OP's responsible for VM creation and installing docker only whereas Developers write and test code in local containers. Same docker image is deployed in production.


Q2) Write command to create a docker container in detached mode with name assignment-2-ROLL_NUMBER running on host port 9090 and container port 80 using image nginx with version 1.24.0 on a custom network named assignment-2?

Ans:

docker network create assignment-2
docker run -d --name assignment-2-I20-0689 -p 9090:80 --network assignment-2 nginx:1.24.0


Q3) Run the above command and add screenshot of it and share the logs?

Ans:

-> Logs:

PS C:\Users\Sherwan Qadir\Desktop\Devops_A2> docker logs assignment-2-I20-0689
/docker-entrypoint.sh: /docker-entrypoint.d/ is not empty, will attempt to perform configuration
/docker-entrypoint.sh: Looking for shell scripts in /docker-entrypoint.d/
/docker-entrypoint.sh: Launching /docker-entrypoint.d/10-listen-on-ipv6-by-default.sh
10-listen-on-ipv6-by-default.sh: info: Getting the checksum of /etc/nginx/conf.d/default.conf
10-listen-on-ipv6-by-default.sh: info: Enabled listen on IPv6 in /etc/nginx/conf.d/default.conf
/docker-entrypoint.sh: Launching /docker-entrypoint.d/20-envsubst-on-templates.sh
/docker-entrypoint.sh: Launching /docker-entrypoint.d/30-tune-worker-processes.sh
/docker-entrypoint.sh: Configuration complete; ready for start up
2023/10/03 23:12:23 [notice] 1#1: using the "epoll" event method
2023/10/03 23:12:23 [notice] 1#1: nginx/1.24.0
2023/10/03 23:12:23 [notice] 1#1: built by gcc 10.2.1 20210110 (Debian 10.2.1-6)
2023/10/03 23:12:23 [notice] 1#1: OS: Linux 5.10.16.3-microsoft-standard-WSL2
2023/10/03 23:12:23 [notice] 1#1: getrlimit(RLIMIT_NOFILE): 1048576:1048576
2023/10/03 23:12:23 [notice] 1#1: start worker processes
2023/10/03 23:12:23 [notice] 1#1: start worker process 29
2023/10/03 23:12:23 [notice] 1#1: start worker process 30
2023/10/03 23:12:23 [notice] 1#1: start worker process 31
2023/10/03 23:12:23 [notice] 1#1: start worker process 32
2023/10/03 23:12:23 [notice]![Devops1](https://github.com/OogwayKP/first-contributions/assets/129097838/0f22acc9-b850-43a8-bef9-d4d0fed2829a)
 1#1: start worker process 33
2023/10/03 23:12:23 [notice] 1#1: start worker process 34
2023/10/03 23:12:23 [notice] 1#1: start worker process 35
2023/10/03 23:12:23 [notice] 1#1: start worker process 36

![Devops1](https://github.com/OogwayKP/first-contributions/assets/129097838/bbbbbdbd-778b-4c11-a183-0757dde468dc)


![Devops2](https://github.com/OogwayKP/first-contributions/assets/129097838/07d7bfc9-7d0b-4046-a6b1-c3a8aabeb2c4)

![Devops3](https://github.com/OogwayKP/first-contributions/assets/129097838/1dfa41fc-0ece-4416-9136-8395cc89f1bb)




