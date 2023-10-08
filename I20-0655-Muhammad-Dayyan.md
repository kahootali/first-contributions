
(Q1) Explain Docker Containers vs VMs

Docker Containers:

-Imagine a container as a lightweight, portable box.
-Containers share the same underlying operating system, like everyone using the same computer.
-They are very efficient because they only contain the specific files and settings needed for a single application.
-Containers start up quickly, in seconds.
-Think of them like individual apps on your smartphone; they're isolated and don't interfere with each other.
-Containers are perfect for packaging and running one application at a time, making them efficient and portable.

Virtual Machines (VMs):

-Visualize a VM as a full-fledged computer within your computer.
-VMs have their own complete operating system, like having multiple physical computers on one machine.
-They can be resource-heavy because each VM duplicates the entire OS.
-VMs take longer to start, often minutes.
-It's like running multiple physical computers on your desk, each with its own software.
-VMs are versatile, allowing you to run multiple applications or even different operating systems on the same hardware.


(Q2) Write command to create a docker container in detached mode with name assignment-2-<ROLL_NUMBER> running on host port 9090 and container port 80 using image nginx with version 1.24.0 on a custom network named assignment-2

-docker run -d --name assignment-2-I20-0655 -p 9090:80 --network assignment-2 nginx:1.24.0


(Q3) Run the above command and add screenshot of it and share the logs

![Alt text](first-contributions\screenshot.png)

