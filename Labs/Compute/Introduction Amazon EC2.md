# Amazon Elastic Compute Cloud (Amazon EC2)

## 📚 Overview

Amazon Elastic Compute Cloud (Amazon EC2) is a web service that provides resizable compute capacity in the cloud. It was specifically designed to make web-scale cloud computing easier for developers by offering flexible, on-demand computing resources.

---

## 🎯 What I Accomplished

During this lab, I completed the following practical tasks:

### ✅ I Launched a Web Server with Termination Protection Enabled
I learned how to provision an EC2 instance and configure protection against accidental termination, a critical security measure for production applications.

### ✅ I Monitored My EC2 Instance
I gained experience viewing metrics and monitoring the performance of my instances in real-time through the AWS CloudWatch console.

### ✅ I Modified the Security Group to Allow HTTP Access
I configured firewall rules in security groups to open port 80, allowing HTTP traffic to reach my web server and making it publicly accessible.

### ✅ I Resized My Amazon EC2 Instance to Scale
I learned how to change the instance type to adjust computing capacity according to performance and cost requirements.

### ✅ I Tested Termination Protection
I validated that termination protection was working correctly, preventing accidental deletion of the instance.

### ✅ I Terminated My EC2 Instance
I completed the instance lifecycle by disabling termination protection and properly shutting down the instance.

---

## 📊 Lab Activity Result

![EC2 Lab Screenshot](https://github.com/user-attachments/assets/65bea16f-73c5-4a9f-99fb-92b16ac2fe27)

*Screenshot showing the configuration and monitoring of my EC2 instance during the lab.*

---

## 🎓 Key Learnings

This hands-on lab provided me with a solid understanding of the complete EC2 instance management lifecycle, from creation and configuration through monitoring and termination. These skills are fundamental for working with AWS cloud infrastructure.

### Topics Covered:
- EC2 Instance Launch & Configuration
- Termination Protection
- Instance Monitoring & Performance Metrics
- Security Group Management
- Instance Resizing & Scaling
- Instance Lifecycle Management

---

**Lab Completed:** 2026-03-11 13:07:40  
**Status:** ✨ Successfully Completed



<b>My AWS Web Server Configuration Success</b>
I just finished setting up a web server on an AWS EC2 instance. Initially, when I tried to visit the website using the instance's public IP address, the page wouldn't load. This was a great hands-on lesson in how Security Groups work as a virtual firewall.

By default, AWS blocks all inbound traffic for security. Since my web server uses Port 80 (HTTP), I had to manually update my security group to permit requests on that specific port from anywhere on the internet. Once I added the inbound rule and saved the settings, the connection worked instantly.

The result is shown in the screenshot below!

<img width="943" height="472" alt="image" src="https://github.com/user-attachments/assets/617dd173-b98e-40eb-9389-a26f53c1e0f4" />
