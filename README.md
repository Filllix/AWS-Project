# 🌐 Simple Web Deployment on AWS EC2 using Nginx  
**Professional DevOps Beginner Project**

This repository contains a simple, production-style deployment of a static website hosted on an Amazon EC2 instance using the Nginx web server.  
The purpose of this project is to demonstrate foundational DevOps skills, including Linux server management, web server configuration, and cloud infrastructure provisioning.

---
https://github.com/Filllix/AWS-Project/blob/main/Simple%20Web%20Deployment%20on%20AWS%20EC2%20Project.pdf
---

## 📘 Table of Contents
1. Overview  
2. Architecture  
3. Technologies Used  
4. Prerequisites  
5. Deployment Guide  
6. Testing the Deployment  
7. Project Structure  
8. Key Learnings   

---

## 1️⃣ Overview

This project showcases how to deploy a static webpage on AWS using:
- An EC2 instance (Amazon Linux 2)
- Nginx as the web server
- Linux-based configuration  
 
The project emphasizes cloud environment familiarity, service configuration, and secure deployment workflow—skills essential for entry-level DevOps and cloud roles.

---

## 2️⃣ Architecture

Client Browser
↓
Internet
↓
AWS EC2 Instance (Amazon Linux 2)
↓
Nginx Web Server
↓
Static Website (index.html)


---

## 3️⃣ Technologies Used

| Technology | Description |
|-----------|-------------|
| **AWS EC2** | Cloud compute to host the web server |
| **Nginx** | Lightweight, high-performance web server |
| **Linux (Amazon Linux 2)** | Server OS used for configuration |
| **SSH** | Secure access to the EC2 instance |
| **HTML/CSS** | Static website content |

---

## 4️⃣ Prerequisites

Before deployment, ensure you have:

- AWS Account (Free Tier supported)  
- SSH Key Pair (.pem)  
- Basic understanding of Linux commands  
- Security Group rules:
  - Port **22** → SSH  
  - Port **80** → HTTP  

---

## 5️⃣ Deployment Guide

### **Step 1: Launch EC2 Instance**
- AMI: **Amazon Linux 2**
- Instance Type: **t3.micro**
- Storage: Default (8GB)
- Security Group:
  - Allow **SSH (22)** from anywhere (0.0.0.0/0)
  - Allow **HTTP (80)** from anywhere (0.0.0.0/0)

---

### **Step 2: Access EC2 via EC2 Instance Connect**

### **Step 3: Install Nginx**

Update packages:
sudo yum update -y

Install Nginx:
sudo yum install nginx -y

Start and enable service:
sudo systemctl start nginx
sudo systemctl enable nginx

### **Step 4: Deploy the Static Website**

Replace the default Nginx index page:
sudo nano /usr/share/nginx/html/index.html
*Paste your custom HTML file (e.g., modern landing page).*

## **6️⃣ Testing the Deployment

Open your browser and access:
http://YOUR PUBLIC_IP
You should see your deployed static website.

Recommended browser checks:
Desktop view
Mobile view
Refresh test
HTTP response test using:
curl -I http://PUBLIC_IP

## **7️⃣ Project Structure
├── index.html               # Deployed static webpage
├── README.md                # Documentation

## **8️⃣ Key Learnings

During this project, I gained practical knowledge in:
Launching and configuring AWS EC2
Setting up a Linux-based web server environment
Understanding Nginx directory structure
Managing system services with systemctl
Deploying static content securely
Configuring firewall (Security Group)
Basic web hosting workflow in the cloud

https://github.com/Filllix/AWS-Project/blob/main/Simple%20Web%20Deployment%20on%20AWS%20EC2%20Project.pdf
