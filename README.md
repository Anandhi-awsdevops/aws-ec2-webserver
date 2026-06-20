# AWS EC2 Web Server Project

## About This Project
I deployed a web server on AWS EC2 as part of my 
hands-on cloud learning.

## Tools and Services Used
- AWS EC2 (Amazon Linux)
- AWS IAM
- AWS Security Groups
- SSH (To connect to server)
- Apache Web Server

## Steps I Followed

### Step 1 - Created EC2 Instance
- Logged into AWS Console
- Went to EC2 Dashboard
- Clicked Launch Instance
- Selected Amazon Linux 2 AMI
- Chose t2.micro (Free tier)

### Step 2 - Connected to EC2
- Downloaded the Key Pair (.pem file)
- Connected using SSH command:
  ssh -i "keyfile.pem" ec2-user@your-public-ip

### Step 3 - Installed Web Server
- Updated the server: sudo yum update -y
- Installed Apache: sudo yum install httpd -y
- Started Apache: sudo systemctl start httpd

### Step 4 - Configured Security Group
- Opened Port 80 (HTTP) for public access
- Opened Port 22 (SSH) for my IP only

### Step 5 - Tested the Website
- Copied the Public IP of EC2
- Pasted in browser
- Website was live! ✅

## What I Learned
- How to launch EC2 instances on AWS
- How to connect to Linux server using SSH
- How to install and run a web server
- How to configure Security Groups and IAM

## Author
Anandhi Kandhan
AWS & DevOps Fresher
