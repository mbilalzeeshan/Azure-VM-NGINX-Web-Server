Azure Virtual Machine Deployment & NGINX Web Server
Overview

This project demonstrates the deployment of an Ubuntu Server Virtual Machine on Microsoft Azure, secure remote administration using SSH, installation and configuration of the NGINX web server, and hosting of a custom webpage.

This project was completed as part of my Cloud Computing (AWS/Azure) Internship at DecodeLabs.

Objectives
Deploy an Ubuntu Virtual Machine on Microsoft Azure
Configure secure SSH access using key-based authentication
Install and configure NGINX
Host a custom webpage
Configure Azure networking and firewall rules
Verify successful deployment
Technologies Used
Microsoft Azure
Ubuntu Server 24.04 LTS
NGINX
Linux
SSH
Azure Virtual Machines
Azure Networking
Network Security Groups
Architecture
Internet
     │
     ▼
Azure Public IP
     │
     ▼
Azure Network Security Group
     │
     ▼
Ubuntu Virtual Machine
     │
     ▼
NGINX Web Server
     │
     ▼
Custom HTML Page

Steps Performed:

Phase 1 — Provisioning
Created Resource Group
Created Ubuntu Virtual Machine
Generated SSH key pair
Assigned Public IP
Phase 2 — Securing the Server
Configured Network Security Group
Allowed HTTP (80)
Restricted SSH (22) to my public IP
Enabled SSH key authentication
Phase 3 — Installing NGINX
sudo apt update
sudo apt upgrade -y
sudo apt install nginx -y
sudo systemctl enable nginx
sudo systemctl start nginx
Phase 4 — Deploying the Website

Replaced the default NGINX page with a custom HTML landing page.

Phase 5 — Verification

Verified:

SSH Connectivity
NGINX Service
Public Website
Azure Resource Deployment
Learning Outcomes
Azure Virtual Machines
Linux Administration
SSH Authentication
Azure Networking
NGINX Configuration
Cloud Infrastructure Deployment
Basic Cloud Security

Future Improvements
HTTPS using Let's Encrypt
Custom Domain
Reverse Proxy
Docker Deployment
CI/CD Pipeline
Monitoring with Azure Monitor
