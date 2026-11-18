AWS Web Server Deployment Project
1. Project Overview

This project demonstrates how to create and deploy a basic static HTML website using an Apache web server hosted on an Amazon EC2 instance.

The project also includes uploading the source code to GitHub and deploying the website using Netlify.

2. Project Objectives

Understand AWS IAM users, groups, roles and policies.

Launch and configure an Amazon EC2 instance.

Configure AWS Security Groups.

Connect to EC2 using SSH.

Install and configure Apache web server.

Deploy a basic HTML and CSS website.

Upload project source code to GitHub.

Deploy the website using Netlify.
3. Technologies and Services Used

Technology- Purpose

AWS IAM- Identity and access management

Amazon EC2- Virtual server hosting

Security Groups- Network access control

Linux- Server operating system

Apache- Web server

HTML- Website structure

CSS- Website styling

Git- Version control

GitHub- Source code repository

Netlify- Website hosting

. Project Folder Structure

- AWS-Web-Server-Project/
  │
- ├── index.html
- ├── style.css
- └── README.md

5. AWS EC2 Configuration

Cloud Provider: Amazon Web Services

Service: Amazon EC2

Region: ap-south-1 (Mumbai)

Operating System: Amazon Linux

Instance Type: t2.micro or eligible free-tier instance

Web Server: Apache HTTP Server

6. Security Group Configuration

The following inbound rules are required:

Type- Protocol- Port- Source
SSH-   TCP-      22-   My IP
HTTP-  TCP-      80-  0.0.0.0/0

Note: Restrict SSH access to your own IP address. HTTP is publicly accessible to allow visitors to access the website.

7. Apache Installation Steps

Update the Linux packages:

- sudo yum update -y

Install Apache:

- sudo yum install httpd -y

Start Apache:

- sudo systemctl start httpd

Enable Apache:

- sudo systemctl enable httpd

Check Apache status:

- sudo systemctl status httpd

8. Website Deployment Steps

Copy the website files into the Apache web directory:

- sudo cp index.html /var/www/html/
- sudo cp style.css /var/www/html/

Restart Apache:

- sudo systemctl restart httpd

Open the website using:

http://YOUR-EC2-PUBLIC-IP

9. GitHub Repository

GitHub Repository:https://github.com/skandakumar1992/AWS-Web-Server-Project.

10. Learning Outcomes

Learned how to configure AWS IAM.

Gained practical experience with Amazon EC2.

Understood Security Group configuration.

Learned Linux server administration basics.

Installed and configured Apache.

Deployed a static website on AWS.

Practiced Git and GitHub.

Learned website deployment using Netlify.
