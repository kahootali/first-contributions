Answer1:
Virtual machines: create a complete virtualized environment for each application, including a separate operating system, kernel, and hardware resources. This makes VMs very isolated and secure, but it also makes them more resource-intensive and slower to start up.

Docker containers: share the host operating system kernel and resources, but each container has its own isolated file system, processes, and network capabilities. This makes containers much more lightweight and faster to start up than VMs, but it also means that they are not as isolated or secure.

Answer2:
docker run -d --name assignment-2-I19-1746 --network assignment-2 -p 9090:80 nginx:1.24.0

Answer 3:
Coomand:
![Screenshot from 2023-10-08 19-46-56](https://github.com/kahootali/first-contributions/assets/115140827/c9f347b2-50e2-408e-90ef-c44dc8a66a06)


Logs:
![Screenshot from 2023-10-08 19-48-08](https://github.com/kahootali/first-contributions/assets/115140827/59e28a26-17a7-4616-a1b1-bd75f52cf39c)

