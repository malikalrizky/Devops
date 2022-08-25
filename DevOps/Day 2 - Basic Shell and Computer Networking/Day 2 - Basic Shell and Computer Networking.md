# Day 2

# Basic Shell and Computer Networking

## 1. Computer Network

Computer network is a system that connects numerous independent computing devices in order to transmit and share information (data) and resources with cable or wireless.

![](./media/computer-networking-lan-service-500x500.jpg)

## 2. Linux Shell

A Linux Shell is a command-line interpreter based on UNIX or Linux, and commonly execute file manipulation, program execution, and text output. 

## 3. Linux Command

![](./media/linux.jpg)

# Setup Computer Network

Setup computer network is a way of System Administrator or DevOps Engineer to change the default IP address on a server

1.  

```
sudo nano /etc/netplan/00-installer-config.yaml
```

![](./media/1.png)

After that: 
`sudo netplan apply`

2. Install putty

![](./media/putty.JPG)

3. Test connection 

`ping google.com`

![](./media/13.png)

# Localtunnel

Localtunnel is a simple tool that provides you a publicly-accessible URL that reroutes every request to your locally-running process

![](./media/lt.png)

## Install Localtunnel

1. Install node.js using nvm

`sudo apt install curl`

Note: curl is a command-line tool to transfer data to or from a server, using any of the supported protocols

![](./media/16.png)

2. Download and install nvm

NVM (Node Version Manager) is a command line tool that allows you to manage different versions of NodeJS.

![](./media/17.png)

![](./media/30.png)

3. Install localtunnel using npm

Note: npm is the package manager for Node.js

![](./media/31.png)

4. Run localtunnel

`lt --port 80`

![](./media/54.png)

![](./media/33.png)


## Install Apache2

1. 

`sudo apt install apache2`

![](./media/35.png)

![](./media/36.png)

2. Allow firewall for Apache2

`sudo ufw app list`

![](./media/37.png)

`sudo ufw allow 'Apache'`

![](./media/38.png)

`sudo ufw status`

![](./media/39.png)

3. Enable Apache2

`sudo systemctl enable apache2.service`

![](./media/42.png)

4. Test using IP address

![](./media/43.png)

5. Make tunnel to port 80 http apache

![](./media/55.png)
![](./media/56.png)
![](./media/57.png)
