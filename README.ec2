# 🚀 AWS EC2 Instance Setup & Deployment Guide

This project demonstrates how to launch, configure, and deploy applications on an AWS EC2 instance. It helps you understand cloud-based virtual servers and manage them securely.

---

## 📘 Project Overview

This guide walks you through launching an EC2 instance, connecting via SSH, installing software, deploying applications, and managing security.

---

## 🎯 Project Objectives

* Launch an EC2 instance using AWS Console
* Configure SSH access using key pairs
* Install software (Apache, Nginx, Python, Node.js)
* Deploy a sample application
* Manage Security Groups
* Automate setup using user data scripts

---

## 🧰 Tools & Technologies Used

| Category        | Tools / Services                        |
| --------------- | --------------------------------------- |
| Cloud Platform  | AWS                                     |
| Compute Service | EC2                                     |
| OS              | Ubuntu / Amazon Linux                   |
| Networking      | VPC, Subnet, Security Group, Elastic IP |
| Storage         | EBS                                     |
| Monitoring      | CloudWatch                              |
| Automation      | User Data Script / Shell Script         |
| Access          | SSH (.pem key)                          |

---

## ⚙️ Step-by-Step Setup Guide

### 1️⃣ Launch EC2 Instance

1. Go to AWS Console → EC2
2. Click **Launch Instance**
3. Choose AMI (Ubuntu 22.04 / Amazon Linux 2)
4. Choose Instance Type: **t2.micro**
5. Select / Create Key Pair
6. Configure networking (enable Public IP)
7. Add storage (8GB or more)
8. Configure Security Group:

   * SSH (22)
   * HTTP (80)
   * HTTPS (443)
9. Launch instance

---

### 2️⃣ Connect to EC2 Instance

```bash
chmod 400 your-key.pem
ssh -i your-key.pem ubuntu@<EC2-Public-IP>
```

---

### 3️⃣ Install and Configure Web Server

```bash
sudo apt update -y
sudo apt install apache2 -y
sudo systemctl start apache2
sudo systemctl enable apache2
```

Visit: **http://<EC2-Public-IP>**

---

### 4️⃣ Deploy Your Application

```bash
sudo apt install git -y
git clone https://github.com/username/repo.git
cd repo
```

Run your Node.js / Python / custom app accordingly.

---

### 5️⃣ Configure Firewall / Security

* Use **Security Groups** for inbound rules
* Assign **IAM Roles** for permissions
* Enable HTTPS (Certbot / ACM)

---

### 6️⃣ Stop / Start / Terminate Instance

* **Stop** → Keeps data
* **Start** → Restart same instance
* **Terminate** → Deletes permanently

---

## 📊 Architecture Diagram (Conceptual)

```
User → Internet → AWS EC2 (Public IP)
                     └── Apache / Nginx Web Server
                           └── Application Files
```

---

## 🧩 EC2 User Data Script Example

```bash
#!/bin/bash
sudo apt update -y
sudo apt install apache2 -y
sudo systemctl start apache2
echo "Hello from EC2 User Data Script" > /var/www/html/index.html
```

---

## 📈 Monitoring & Optimization

* Monitor using **CloudWatch**
* Enable **Auto Scaling Groups (ASG)**
* Assign **Elastic IP** for fixed address
* Use **Snapshots** for backups

---

## 📋 Interview Questions on AWS EC2

### 🧠 Basic

* What is EC2?
* What are instance types?
* What is AMI?
* What storage does EC2 use?
* How to connect using SSH?
* What is a key pair?

### ⚙️ Intermediate

* Stop vs Terminate
* Use of Elastic IP
* Instance security methods
* What happens on reboot?
* Can we change instance type?
* On-Demand vs Reserved vs Spot

### 🔒 Advanced

* Automated deployment on EC2
* Troubleshooting SSH issues
* Configure load balancing
* EC2 Metadata vs User Data
* Auto Scaling
* Monitoring instance metrics
* Migrate EC2 across regions
* Attach & mount EBS volume

---

## 🧾 Conclusion

This project covers everything from launching an EC2 instance to hosting applications securely. It is essential for AWS Cloud Engineers, DevOps Engineers, and System Administrators.

---

## 🌐 Author

**👤 Suraj Dhakad**
Aspiring DevOps Engineer
📧 **[surajdhakad80@gmail.com](mailto:surajdhakad80@gmail.com)**
