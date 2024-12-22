# PROJECT-2-SECOND-SEMESTER-FOR-JESSICA-NWALOKA-

A PROJECT GIVEN BY ALTSCHOOL FOR CLOUD ENGINEERING STUDENTS.

# Nginx Web Hosting on Ubuntu EC2 Instance with HTTPS and Free SSL Certificate
___

## Project Overview

The goal of this project is to provision a server and deploy a prototype web application with a sleek and professional landing page. This landing page highlights the team's technical expertise and vision, serving as a compelling tool to engage potential investors. By combining efficient server setup, web development, and design, the project delivers a functional and visually impressive preview of the application.

---
## Repository Highlights

This repository offers a detailed roadmap for:  
✅ Launching and configuring an Ubuntu EC2 instance for web hosting.  
✅ Setting up and optimizing Nginx to deliver the  web content efficiently.  
✅ Securing the  site with HTTPS using a free SSL certificate from "Let’s Encrypt"  
✅ Integrating a custom domain with advanced, professional-grade configurations. 

---
Step-by-Step Documentation: 
__

Server Provisioning and Deployment
More than just a step-by-step guide, this project equips you with a robust toolkit for building a secure, scalable, and dependable web server that meets contemporary web standards. Whether you're a beginner in web hosting or a seasoned developer, this repository will refine your skills and deepen your expertise in hosting and web security.
---
## Prerequisites 

Before you begin, make sure you meet the following prerequisites to ensure a seamless setup experience:

🔧 **Basic Linux Command Knowledge**: A good grasp of fundamental Linux commands will make it easier to manage and interact with the server.

☁️ **EC2 Instance Preparation**: Familiarity with launching an EC2 instance and configuring security groups to allow HTTP and HTTPS traffic.

💻 **Development Tools**: Access to tools like Git Bash or Visual Studio Code (VSCode) for file management and executing commands.

__
With these essentials covered, you’re ready to jump in and get started! 🚀
---
### Step-by-Step Guide: Server Provisioning and Deployment  

##. Crafting the Web Page##

- Developed a lightweight HTML page enhanced with minimal CSS for styling, using Visual Studio Code as the primary editor.  
- Prioritized a clean, professional aesthetic to ensure a sleek and straightforward user experience.  

##2. Provisioning the Server##

- Set up a virtual server instance using AWS EC2:  
  - Created an instance with a custom name, generated a key pair for secure access, and established a security group.  
  - Configured the security group to permit HTTP traffic on port 80 for web accessibility.  
- Successfully launched the EC2 instance and accessed the server via SSH, using Termius as the terminal client.
  
### 3. **Installing and Configuring Nginx##

Installed Nginx on the server using the following commands:
sudo apt update  
sudo apt install nginx -y  
sudo systemctl start nginx  
sudo systemctl enable nginx  

Verified the installation by accessing the server's public IP address in a web browser to confirm the default Nginx welcome page was successfully displayed.


### 4. **Transferring Project Files##


Leveraged WinSCP, a file transfer tool, to manually upload the project folder (cloudproject) to the server. Alternatively, the following command can be used:
sudo cp -r ~/cloudproject/* /var/www/html/  
Verified the successful transfer by listing the contents of Nginx's root directory with:
ls -l /var/www/html  

---
### 5. **Enabling HTTPS with Let’s Encrypt##
Installed the necessary tools for managing SSL certificates:

sudo apt update  
sudo apt install certbot python3-certbot-nginx -y  
Secured the domain dubem.web.jumpingcrab.com by obtaining and installing a free SSL certificate:
sudo certbot --nginx -d jessica.web.strangled.net 
This command seamlessly configured the Nginx server to enable HTTPS, ensuring secure and encrypted communication.

---
### 6. **Verifying the SSL Certificate##

Verified the SSL certificate by visiting https://jessica.web.strangled.net
Ensured the secure connection was active by checking for the padlock icon in the browser’s address bar.
---
### 7. **Running the Web Page**  

Refreshed the browser using the public IP address or domain to display the deployed landing page.

---
## IP Address  
The project is accessible temporarily at **[13.53.99.32](http://13.53.99.32)**  13.53.99.32 for verification purposes only.

