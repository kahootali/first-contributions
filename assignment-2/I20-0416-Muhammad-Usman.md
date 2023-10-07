Q1 Explain Docker Containers vs VMs

Ans: 
Conatiners are the abstarction at app layer. They share host OS kernel and take less space as compared to vms.
Conatiners can be shipped and run on any machine with no problem of dependencies or versions conflicts as same image with all dependencies is shipped.
Wheresas Vms are the abstarction of physical hardware. each vm has its  full fledge OS and thus takes alot of space and resources.each developer has to install and setup vm which resulted in conflicts of dependencies and versions as slight difference meant that application would not run on new machine.  



Q2 Write command to create a docker container in `detached` mode with name `assignment-2-<ROLL_NUMBER>` running on host port `9090` and container port `80` using image `nginx` with version `1.24.0` on a custom network named `assignment-2`


Ans:  
docker network create assignment-2
docker run -d --name assignment-2-I20-0416 -p 9090:80 --network assignment-2 nginx:1.24.0


Q3 Run the above command and add screenshot of it and share the logs

Ans: All Scrrenshots added in assignment-2 folder.




