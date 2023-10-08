- Q1)  Explain Docker container vs VMs

- Ans)  

Docker Containers:
- Lightweight.
- Share the host OS kernel.
- Process-level isolation.
- Minimal resource overhead.
- Fast startup time.
- Ideal for microservices and containerized applications.

Virtual Machines (VMs):
- Heavier.
- Run their own OS.
- Strong isolation.
- Greater resource overhead.
- Slower startup time.
- Suitable for running diverse workloads with different OS requirements.


Q2) Write command to create a docker container in `detached` mode with name `assignment-2-<ROLL_NUMBER>` running on host port `9090` and container port `80` using image `nginx` with version `1.24.0` on a custom network named `assignment-2`

ans) 

docker run -d --name assignment-2-i20-0406 -p 9090:80 --network assignment-2 nginx:1.24.0


Q3) Run the above command and add screenshot of it and share the logs


ans) 


/DockerLog.png
