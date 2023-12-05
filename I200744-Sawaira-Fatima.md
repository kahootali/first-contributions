#Answers to the Questions

Q1) Explain Docker Containers vs VMs

Docker containers are lightweight as compared to the VMs as they share the host machine's OS kernel. VMs on the other hand bring a complete OS with them which makes them much more heavier and requires more time to bootup. Containers allow the user to make use of burstable computing which makes it more responsive even in increased load as it can increase the number of VCPUs required to perform the operations. VMs on the other hand have to be managed manually by the user as it cannot exceed the number of VCPUs assigned. Another difference is the responsibility of the Ops. In case of containers, Ops only need to install the docker container and pull images without needing to worry about compatibility issues. In the case of VMs the responsibility increases as the libraries need to be taken care of as well as latest updates. VMs do not offer latest updated libraries unlike the containers.


Q2) Write command to create a docker container in detached mode with name assignment-2-<ROLL_NUMBER> running on host port 9090 and container port 80 using image nginx with version 1.24.0 on a custom network named assignment-2

docker run -d --name assignment-2-I20-0744 -p 9090:80 --network assignment-2 nginx:1.24.0


Q3) Run the above command and add screenshot of it and share the logs

Attached along the md file

    Create a PR from your branch to this repo i.e. the parent(kahootali/first-contributions) repo main branch with title Assignment 2 - <ROLL_NUMBER> - <FIRST_NAME-LAST_NAME>
   
    In the PR description, mention that this PR will fix the issue number that you created in the above steps. so that the issue gets closed automatically when PR gets merged
   
    Handle any comments on the PR review
   
    Get this PR merged into this parent repo

