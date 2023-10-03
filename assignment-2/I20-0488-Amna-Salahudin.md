### Q1) Explain Docker Containers vs VMs

1. **Architecture:**
   - **Docker Containers:** 
      - OS level virtualization, i.e. abstraction at the application layer which includes the code and the dependencies. 
      - Shares the hardware, host OS kernel but can have its own OS. 
      - Containers are isolated and the applications as well.
   - **Virtual Machines:** 
      - Shares hardware of the Host OS but has its own operating system. 
      - VMs are isolated but the applications are not.

2. **Resource Efficiency:**
   - **Docker Containers:** 
      - Takes up less space (typically tens to hundreds of MBs in size) and starts almost instantly. 
      - Has burstable compute, burstable memory and low resource usage.
   - **Virtual Machines:** 
      - Each VM includes a full copy of the operating system, one or more apps, necessary binaries and libraries - taking up tens of GBs. 
      - VMs can also be slow to boot. 
      - Has static compute, static memory and high resource usage.

3. **Security:**
   - **Docker Containers:** 
      - Have potential security risks if not properly managed, as a vulnerability in the host OS could potentially impact all containers running on it.
   - **Virtual Machines:** 
      - Provide a more secure boundary, as each VM is completely isolated from the host and other VMs.

### Q2) Write command to create a docker container in detached mode with name assignment-2-<ROLL_NUMBER> running on host port 9090 and container port 80 using image nginx with version 1.24.0 on a custom network named assignment-2

**Answer:**
```bash
docker run -d --name assignment-2-I20-0488 --network assignment-2 -p 9090:80 nginx:1.24.0
```

### Q3) Run the above command and add screenshot of it and share the logs

<a href="https://imgur.com/zDcGUSA"><img src="https://i.imgur.com/zDcGUSA.png" title="source: imgur.com" /></a>


<a href="https://imgur.com/IZpfTLt"><img src="https://i.imgur.com/IZpfTLt.png" title="source: imgur.com" /></a>

**Logs:** 
<a href="https://imgur.com/J6OCrqx"><img src="https://i.imgur.com/J6OCrqx.png" title="source: imgur.com" /></a> 



