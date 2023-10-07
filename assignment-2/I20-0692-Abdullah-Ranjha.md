Architecture:
containers: share same os kernel as host os and isolate the application processes from each other
vm: provide a full virtualized system with its own hardware resources including operating system it runs on a hypervisor.
size:
containers: light weight as they share the host os kernel
vms: large as they include full os instance
performance
containers: offer better performance as they share host os kernel
vms: provide worse performance in comparison because they have their own os
isolation
containers: provide process level isolation
vms: provide hardware level isolation
portability
containers: highly portable
vms: less portable
security
containers: less secure as vulnerabilities in kernel can affect all the containers on host
vms: offer stronger isolation so they are more secure

Q2
docker run -d --name assignment-2-I20-0692 -p 9090:80 --network assignment-2 nginx:1.24.0
Q3
