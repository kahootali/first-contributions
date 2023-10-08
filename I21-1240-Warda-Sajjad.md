

VMS:
->VM has Hardware level virtualization i.e. abstraction of physical hardware
->It share Hardware but has own OS
->Each VM has a full copy of an operating system + application + binaries + libraries
-> It can take up to tens of GBs.
-> VMs are isolated, apps are not Complete OS, Static Compute, Static Memory, High Resource Usage

Containers: 
-> Container has OS level virtualization i.e. abstraction at the app layer (code + dependencies)
-> It share hardware, host OS kernel but can have own OS
-> It take up less space (typically tens to hundreds of MBs in size)
-> containers are isolated, so are the app.
-> Container Isolation, Shared Kernel,Burstable Compute, Burstable Memory,Low Resource Usage


![Alt Text](https://imgur.com/a/m9WmRz9)
