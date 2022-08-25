# Day 1

# Intro to DevOps

## 1. Fundamental DevOps

DevOps is a culture or method that shifts the way that Development and Operations team members work together. DevOps culture aims to maintain trust, collaboration, problem resolution, and continuous improvement across the entire team.

![](./media/devops.jpg)

## 2. Operating System Concept

An Operating System is the software which manages physical computing resources, interfaces between the hardware and the applications on a computer.

![](./media/os.png)

## 3. Virtualization

Virtualization is the process that enables teams to create a useful virtual or simulated version/instance of the software on a single server.
The benefits of virtualization include: More agility, flexibility, and scalability during development.

![](./media/virtualization.JPG)

# Making environment for server (CPU, Memory, Storage dan Network)

## Install Ubuntu Server 20.x with VMware
### Download Ubuntu Server
[Download](https://ubuntu.com/download/server)

![](./media/ubuntu.png)

### Download VMware
[Download](https://www.vmware.com/products/workstation-player/workstation-player-evaluation.html)

![](./media/vmware.JPG)

### Install VMware
1. Open the VMware and then Create a new virtual machine

![](./media/1.png)

2. Choose the Ubuntu Server

![](./media/2.png)

3. Insert user and password

![](./media/3.png)

4. Choose the Virtual Machine's name and location

![](./media/4.png)

5. Specify Disk Capacity

![](./media/5.png)

6. Choose customize hardware

![](./media/6.png)

7. Change the network adapter to Bridged

Note:
- Memory: virtual memory provides many function, including multitasking (multiple tasks executing at once on one CPU), allowing multiple processes to access the same shared library in memory, swapping, and others.
- Processors: virtual processor is a CPU core that is assigned to a virtual machine. There can be more virtual processors assigned than actual cores available, which allows virtual machines to share the same core.
- Network adapter: to connect virtual machine server into network

![](./media/7.png)

8. Increasing the system swap memory of the virtual machine

![](./media/8.png)

9. Choose language

![](./media/9.png)

10. Configure the network connection of the virtual machine

Note:
- DHCP (Dynamic Host Protocol Configuration) : The IP address change automatically following the network of the device
- Static : The IP address doesn't change and being set by admin

![](./media/10.png)

11. Edit ens33 IPv4 configuration to manual

![](./media/11.png)

12. Input the Subnet, Address, Gateway, and Name Servers

![](./media/12.png)

13. If successful click done

![](./media/13.png)

14. Configure proxy

![](./media/14.png)

15. Configure ubuntu archive mirror

![](./media/15.png)

16. Configure storage

Choose custom storage layout

![](./media/16.png)

17. Add GPT partition

![](./media/17.png)

18. Swap = backup storage

![](./media/18.png)

19. Ext4 = main storage

![](./media/19.png)

20. After succesful create partition click done

![](./media/20.png)

21. Confirm destructive action

![](./media/21.png)

22. Profile setup

![](./media/22.png)

23. SSH Setup

Check Install OpenSSH server

![](./media/23.png)

24. Install snaps if needed

![](./media/24.png)

25. Installing system

![](./media/25.png)

26. Reboot the virtual machine 

![](./media/26.png)

27. Login and then test the connection

![](./media/27.png)

![](./media/28.png)
