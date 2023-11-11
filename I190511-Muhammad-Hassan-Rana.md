Q1: Explain Docker Containers vs VMs?
Docker containers are lightweight, isolated environments that share the host OS kernel, making them more efficient in terms of resource usage and faster to start compared to virtual machines (VMs). VMs, on the other hand, run full OS instances, making them heavier and slower to start but providing stronger isolation and compatibility with different OSes.

Q2: Write command to create a docker container in detached mode with name assignment-2-<ROLL_NUMBER> running on host port 9090 and container port 80 using image nginx with version 1.24.0 on a custom network named assignment-2
docker run -d --name assignment-2-I190511 -p 9090:80 --network assignment-2 nginx:1.24.0

Q3: Run the above command and add screenshot of it and share the logs
