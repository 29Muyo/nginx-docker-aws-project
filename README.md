# Deploying a Website on Nginx Server using Docker on AWS

**Author:** Kathleen Muyoni
**Date:** April 12, 2026

---

### **Table of Contents**
1. [Project Overview](#project-overview)
2. [Architecture Diagram](#Docker.drawio.png)
4. [Prerequisites](#prerequisites)
5. [Step 1: Launch EC2 Instance](#step-1-launch-ec2-instance)
6. [Step 2: Install Docker](#step-2-install-docker)
7. [Step 3: Clone Website Files](#step-3-clone-website-files)
8. [Step 4: Write the Dockerfile](#step-4-write-the-dockerfile)
9. [Step 5: Build Docker Image](#step-5-build-docker-image)
10. [Step 6: Run the Container](#step-6-run-the-container)
11. [Step 7: Access the Website](#step-7-access-the-website)

---

### **Project Overview**
This project demonstrates how to deploy a static website on AWS using Docker and Nginx. The website files are cloned from GitHub, containerised using a Dockerfile, and served through an Nginx web server hosted on an AWS EC2 instance.

---

### **Architecture Diagram**



### **Prerequisites**
- AWS Account
- EC2 Instance running Ubuntu
- Docker installed
- Basic knowledge of Linux commands

## Step by Step Setup

### 1. Launch EC2 Instance
- Log into AWS Console
- Launch Ubuntu EC2 instance
- Connect via SSH

### 2. Install Docker
```bash
sudo apt-get update
sudo apt-get install docker.io
```

### 3. Pull Nginx Image
```bash
docker pull nginx
```

### 4. Create Your Website Files
- Create your HTML file
- Add your content

### 5. Write Your Dockerfile
```dockerfile
FROM nginx
COPY index.html /usr/share/nginx/html/
```

### 6. Build Your Image
```bash
docker build -t my-website .
```

### 7. Run Your Container
```bash
docker run -d -p 80:80 my-website
```

### 8. Access Your Website
- Copy your EC2 Public IP
- Open in browser

  

