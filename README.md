# Multi‑VM DevOps Stack (Vagrant + Provisioning)

This project demonstrates a **multi‑VM DevOps environment** built with Vagrant.  
It provisions five virtual machines automatically, each running a key service in a typical distributed stack:

- Nginx – Reverse proxy / load balancer  
- Tomcat – Application server  
- MySQL – Relational database  
- Memcached – In‑memory caching layer  
- RabbitMQ – Message broker for asynchronous communication  

Provisioning is handled via **shell scripts (`.sh`)**, ensuring each VM is configured consistently and reproducibly.

## 📂 Project Structure
- Vagrantfile------# Defines 5 VMs and provisioning steps 
- backend.sh-------# Backend app setup 
- nginx.sh --------# Nginx reverse proxy setup
- tomcat.sh--------# Tomcat server setup 
- mysql.sh---------# MySQL database setup 
- memcache.sh------# Memcached cache setup 
- rabbitmq.sh------# RabbitMQ broker setup 

## Getting Started

### Prerequisites
- [Vagrant](https://www.vagrantup.com/)  
- [VirtualBox](https://www.virtualbox.org/) or another Vagrant provider  
- Git installed locally  

### Setup
1. Clone the repository:
   git clone https://github.com/<your-username>/Multi-VM-DevOps-Stack.git
   cd Multi-VM-DevOps-Stack
   
2. Start the environment:
   vagrant up
   
3. Login to web01
   vagrant ssh web01
   
4. Check for IP address
   ip addr show
   
5. Copy the IP and run it in your browser
    
6. Browse through various pages and tabs of the site to ensure everything is working fine. 
