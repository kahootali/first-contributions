### Q1) Explain Docker Containers vs VMs


### Q2) Write command to create a docker container in `detached` mode with name `assignment-2-<ROLL_NUMBER>` running on host port `9090` and container port `80` using image `nginx` with version `1.24.0` on a custom network named `assignment-2`
Commmand -> docker run -d -p 9090:80 --name assignment-2-I20-2445 --network assignment-2 nginx:1.24.0

### Q3) Run the above command and add screenshot of it and share the logs
