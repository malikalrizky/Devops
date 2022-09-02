# Day 7

# Web Server and Load Balancing

A web server is a computer software and underlying hardware (processor and memory) that provides data-based services and to receive requests from client via HTTP or its secure variant HTTPS or usually called by web browser. Later, web server can send response on request in form of web page.

## Running Reverse Proxy and Load Balancing on Web Server

### 1. Setup Environment

This documentation is using [multipass](https://multipass.run/)

![](./media/1.png)

Create server for gateway and then remote into the server

![](./media/2.png)

Update and install nginx

![](./media/3.png)

![](./media/4.png)

Try connection

![](./media/5.png)

![](./media/6.png)

### 2. Create Reverse Proxy Config

Reverse proxy is a type of proxy server that typically sits behind the firewall in a private network and directs client requests to the appropriate backend server. A reverse proxy provides an additional level of abstraction and control to ensure the smooth flow of network traffic between clients and servers.

![](./media/rp.png)

```
server { 
    server_name domain.com; 
    
    location / { 
             proxy_pass http://(ip):(port);
    }
}
```

![](./media/7.png)

![](./media/8.png)

![](./media/26.png)

### 3. Edit nginx config

![](./media/10.png)

![](./media/11.png)

![](./media/12.png)

![](./media/13.png)

### 4. Create virtual host

```
sudo nano /etc/hosts
```

![](./media/15.png)

![](./media/25.png)

Try the virtual host

![](./media/16.png)

### 5. Installing the app

![](./media/17.png)

![](./media/18.png)

![](./media/19.png)

Start app

![](./media/20.png)

![](./media/27.png)

### 6. Create Load Balancing Config

Load Balancing is a technique used to distribute workloads uniformly across servers or other compute resources to optimize network efficiency, reliability and capacity.

![](./media/lb.png)

```
upstream domain { 
    server (ip):(port);
    server (ip):(port);
}
server { 
    server_name domain.com; 
    
    location / { 
             proxy_pass http://domain;
    }
}
```

![](./media/22.png)

![](./media/28.png)

One of the server died

![](./media/27.png)

Both server died

![](./media/24.png)

### 7. Install PM2 on Web Server

PM2 used so that the app can run in background without remote the server.

```
sudo npm install pm2@latest -g
```

![](./media/29.png)

```
pm2 start npm --name "name" -- start
```

![](./media/30.png)

Try exit the remote server

![](./media/31.png)

![](./media/27.png)