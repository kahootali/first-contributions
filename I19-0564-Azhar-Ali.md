
Question#01

Docker containers are lightweight and efficient, sharing the host operating system kernel with other containers.
Virtual machines are more resource-intensive, but provide complete isolation from the host operating system and other VMs.
The best technology for you will depend on your specific needs. Consider the level of isolation required, resource usage, startup time, and portability.


Question#02

Creating the required network using:
 ->docker network create assignment-2

Launch the designated container using:
 ->docker run -d --name assignment-2-I19-0564 --network assignment-2 -p 9090:80 nginx:1.24.0