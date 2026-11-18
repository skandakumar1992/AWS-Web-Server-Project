<<<<<<< HEAD
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
=======
# 🚀 AWS Web Server Deployment Project

\<p align="center">   \<b>Deploying a Static Website Using Amazon EC2 and Apache Web Server\</b> \</p>

---

## 📌 1. Project Overview

This project demonstrates how to deploy a static HTML website using an **Apache Web Server hosted on Amazon EC2**.

It covers AWS IAM configuration, EC2 instance creation, Security Group configuration, Apache installation, website deployment, GitHub version control and Netlify hosting.

## 🎯 2. Project Objectives

- Understand AWS IAM users, groups, roles and policies.
- Launch and configure an Amazon EC2 instance.
- Configure AWS Security Groups.
- Connect to EC2 using SSH.
- Install and configure Apache Web Server.
- Deploy a static HTML and CSS website.
- Upload source code to GitHub.
- Deploy the website using Netlify.

## 🛠️ 3. Technologies Used

| Technology         | Purpose                        |
| :----------------- | :----------------------------- |
| ☁️ AWS IAM         | Identity and Access Management |
| 🖥️ Amazon EC2     | Virtual server hosting         |
| 🔐 Security Groups | Network access control         |
| 🐧 Linux           | Server operating system        |
| 🌐 Apache          | Web server                     |
| 🎨 HTML            | Website structure              |
| 🎨 CSS             | Website styling                |
| 📦 Git             | Version control                |
| 🐙 GitHub          | Source code management         |
| 🚀 Netlify         | Static website hosting         |

## 📁 4. Project Structure

```text
AWS-Web-Server-Project/
│
├── index.html
├── style.css
└── README.md

```

## ☁️ 5. AWS EC2 Configuration

| Configuration    | Details                              |
| :--------------- | :----------------------------------- |
| Cloud Provider   | Amazon Web Services                  |
| Region           | Asia Pacific (Mumbai)                |
| Region Code      | ap-south-1                           |
| Service          | Amazon EC2                           |
| Operating System | Amazon Linux                         |
| Instance Type    | t2.micro (if available and eligible) |
| Web Server       | Apache HTTP Server                   |

## 🔐 6. Security Group Configuration

The following inbound rules are configured to access the EC2 instance and website.

| Type | Protocol | Port | Source    |
| :--- | :------- | :--: | :-------- |
| SSH  | TCP      |  22  | My IP     |
| HTTP | TCP      |  80  | 0.0.0.0/0 |

**Security Note:** SSH access should be restricted to your own IP address. HTTP is publicly accessible to allow visitors to view the website.

## ⚙️ 7. Apache Installation and Configuration

### Step 1: Update system packages

```bash
sudo yum update -y
```

### Step 2: Install Apache

```bash
sudo yum install httpd -y
```

### Step 3: Start Apache

```bash
sudo systemctl start httpd
```

### Step 4: Enable Apache

```bash
sudo systemctl enable httpd
```

### Step 5: Check Apache status

```bash
sudo systemctl status httpd
```

## 🌐 8. Website Deployment on AWS EC2

Copy the website files into the Apache web directory.

```bash
sudo cp index.html /var/www/html/
sudo cp style.css /var/www/html/
```

Restart Apache:

```bash
sudo systemctl restart httpd
```

Open the website using your EC2 public IP:

**Live EC2 Website:** `http://YOUR-EC2-PUBLIC-IP`

## 🐙 9. GitHub Repository

The project source code is available on GitHub.

🔗 [**View AWS Web Server Project Repository**](https://github.com/skandakumar1992/AWS-Web-Server-Project)

## 🚀 10. Netlify Deployment

The static website can also be deployed using Netlify by connecting the GitHub repository.

**Live Netlify Website:** Add your Netlify URL after deployment.

## 📸 11. Project Screenshots

Add your actual project screenshots here.

| Screenshot        | Description                    |
| :---------------- | :----------------------------- |
| IAM Configuration | AWS IAM users and policies     |
| EC2 Instance      | Running EC2 instance           |
| Security Group    | Inbound security rules         |
| Apache Server     | Apache installation and status |
| Live Website      | Website hosted on AWS          |
| Netlify           | Website deployed on Netlify    |

## 📚 12. Learning Outcomes

Through this project, I gained practical knowledge of:

- AWS IAM users, groups, roles and policies.
- Amazon EC2 instance creation and configuration.
- AWS Security Group configuration.
- Linux server administration.
- Apache web server installation and management.
- Static website deployment.
- Git and GitHub version control.
- Website hosting using Netlify.

## 👨‍💻 13. Author

**Skanda Kumar**

- GitHub: https://github.com/skandakumar1992/AWS-Web-Server-Project
- Project: AWS Web Server Deployment

---

\<p align="center">   ⭐ If you find this project useful, consider giving it a star! \</p>

\<p align="center">   \<b>Created as part of my AWS and DevOps learning journey.\</b> \</p>
>>>>>>> 9b8efcb (Update README with professional project documentation)
