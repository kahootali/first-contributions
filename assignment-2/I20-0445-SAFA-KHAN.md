Answer 1:
Containers are more resource-efficient since they share the host operating system. This results in lighter and more portable containers that consume fewer resources, leading to faster application startup and scaling. In contrast, virtual machines come with a complete operating system, which consumes CPU and memory resources, making them heavier in resource usage due to the overhead of running multiple guest OS instances.
Another distinction lies in how data is managed. Containers do not inherently provide persistent data storage but can achieve it through methods like disk mounting or using volumes. On the other hand, VMs offer dedicated memory for data storage.
The final difference pertains to isolation. VMs provide strong isolation through separate guest OS instances, which is critical for security but comes at the cost of resource intensity. Containers, in contrast, share the host OS kernel, providing lower isolation. This makes them suitable for shared environments but less ideal for handling sensitive or multi-tenant workloads.
Answer 2:
docker network create assignment-2
docker run -d --name assignment-2-I20-0407 -p 9090:80 --network assignment-2 nginx:1.24.0
Answer 3:
![Alt text](image.png)