# Deploying a Website on Nginx Server using Docker on AWS

**Author:** Kathleen Muyoni
**Date:** April 12, 2026

---

### **Table of Contents**

## What This Project Does
A step by step deployment of a static website using Nginx as the web server, containerised with Docker, and hosted on an AWS EC2 instance.

## Prerequisites
- AWS Account
- EC2 Instance running Ubuntu
- Docker installed
- Basic knowledge of Linux commands

## Technologies Used
- AWS EC2
- Docker
- Nginx
- Ubuntu

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

## Errors I Encountered and How I Fixed Them


## Screenshots


## What I Learned


## Author
Kathleen Muyoni
- LinkedIn:
- Medium: 
- Hashnode: 
  

