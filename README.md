# cloud-secure-webserver
Deploying My first EC2 webserver
🛠️ Secure EC2 Web Server Deployment (AWS + Ubuntu + NGINX)

This project walks through deploying and securing a web server on AWS EC2 using Ubuntu 22.04, NGINX, UFW, Fail2Ban, and HTTPS via Let’s Encrypt.

---

 📚 Table of Contents

1. [Project Overview](#project-overview)
2. [Tools & Technologies](#tools--technologies)
3. [Architecture](#architecture)
4. [Setup Instructions](#setup-instructions)
    - [1. Launch EC2 Instance](#1-launch-ec2-instance)
    - [2. Connect via SSH](#2-connect-via-ssh)
    - [3. Install NGINX](#3-install-nginx)
    - [4. Secure SSH Access](#4-secure-ssh-access)
    - [5. Configure Firewall (UFW)](#5-configure-firewall-ufw)
    - [6. Install Fail2Ban](#6-install-fail2ban)
    - [7. Enable HTTPS (Let’s Encrypt)](#7-enable-https-lets-encrypt)
5. [Validation](#validation)
6. [Screenshots](#screenshots)
7. [Lessons Learned](#lessons-learned)



 🧠 Project Overview

This project simulates a real-world deployment and security hardening of a cloud server. You’ll go from launching an EC2 instance to securing it against brute-force attacks and enabling HTTPS.

Goals:
- Launch an Ubuntu EC2 instance
- Install and configure NGINX
- Enforce SSH key authentication
- Configure UFW firewall
- Protect SSH with Fail2Ban
- Enable HTTPS with Let’s Encrypt

---

## 🧰 Tools & Technologies

| Tool | Purpose |
|------|---------|
| AWS EC2 | Cloud virtual machine |
| Ubuntu 22.04 | Linux OS |
| NGINX | Web server |
| SSH Key | Remote login |
| UFW | Firewall |
| Fail2Ban | SSH brute-force protection |
| Let’s Encrypt + Certbot | TLS/SSL certificates |
| Git & GitHub | Version control |

---

## 🗺️ Architecture


---

 Setup Instructions

Each step below is broken into commands and reasoning.

1. Launch EC2 Instance
We begin by launching an EC2 instance using the AWS Management Console.

Configuration:
Name: secure-nginx-server
-AMI: Ubuntu Server 22.04 LTS (HVM)
- Instance Type:t2.micro (Free Tier)
-*SSH Key Pair: A new key was created and downloaded for secure access.
- Security Group Rules:
  - SSH (port 22) — Only my IP
  - HTTP (port 80) — Open to all
  - HTTPS (port 443) — Open to all

This setup ensures we start with minimal exposure to threats, following the principle of **least privilege**.

_(More steps to be filled as you go along)_

---

## 🖼️ Screenshot
![Screenshot](screenshot/image1.png)s

- EC2 Instance Running ✅
- NGINX Welcome Page ✅
- HTTPS Enabled ✅

(Add these as you proceed.)

---

## 📘 Lessons Learned

_To be completed at the end..._

---

