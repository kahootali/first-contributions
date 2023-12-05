Q1) Explain Docker Containers vs VMs?

Containers:

1.Abstraction Type: Containers work like a special kind of software that focuses on running just one application and all the things it needs.

2.Sharing Resources: Even though they can have a tiny version of an operating system, containers share the main computer's parts and the brain of the operating system.

3.Size: Containers are usually not too big, somewhere between a few megabytes to a few gigabytes.

4.Keeping Things Separate: Containers are like individual rooms; they keep different software apart so that they don't interfere with each other.

5.Key Features: Containers are great at using resources efficiently, sharing the computer's main brain, and they can easily use more computer power or memory when needed. They also make sure that each application stays in its own space.

Virtual Machines (VMs):

1.Abstraction Type: VMs are like full-fledged virtual computers that pretend to be real ones.

2.Sharing Resources: Even if they use the same computer, VMs act like they each have their own complete operating system, apps, and files.

3.Size: VMs can be quite big, often taking up a lot of storage space, like a few gigabytes each.

4.Keeping Things Separate: VMs are like separate houses; they have their own space, but the programs inside them can sometimes talk to each other.

5.Key Features: VMs come with a full operating system, they always use the same amount of computer power and memory, and they need a lot of computer resources to work.

                        ---------------------------------------------------------------

Q2) Write command to create a docker container in detached mode with name assignment-2-<ROLL_NUMBER> running on host port 9090 and container port 80 using image nginx with version 1.24.0 on a custom network named assignment-2?

docker network create assignment-2

docker run -d --name assignment-2-I20-0766 -p 9090:80 --network assignment-2 nginx:1.24.0

                        --------------------------------------------------------------

Q3) Run the above command and add screenshot of it and share the logs?

![Alt text](Terminal.png) 
![Alt text](Docker.png)

