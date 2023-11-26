Answer 1:
Docker Containers: 
1. Docker Containers are lighweight & efficent.
2. They share kernel with Host OS.
3. Docker Containers offer process level isolation.
4. They offer burstable compute.
5. Docker comes with all the required dependencies & configuration files.
6. Alot of pre-build images are available on docker hub.
   
VMs:
1. Resource intensive as compared to docker containers.
2. Each VM has its own OS.
3. VM offers static compute of resources.
4. VMs can provide strong isolation at OS level.
5. Deploying an app from developers machine to a VM can be a problem as there can be configuration problems.


Answer 2:
docker run -d --name assignment-2-I19-2192 -p 9090:80 --network assignment-2 nginx:1.24.0


Answer 3:
The command execution & the logs for the docker container are shown in the below picture.
![docker run](https://github.com/kahootali/first-contributions/assets/86046697/870b4dc0-300b-46c1-96d0-720722f61717)

In the below image, we can see that on port 9090, nginx is running.
![port 9090](https://github.com/kahootali/first-contributions/assets/86046697/09e4b2b6-a03b-4e27-bd5f-dfd9eb1b5a81)




