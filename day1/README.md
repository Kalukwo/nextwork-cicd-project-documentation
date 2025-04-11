[View Day 1 PDF](day1/day1.pdf)

# Set Up a Web App Using AWS and VS Code

**Author:** Shadrack Kalukwo  
**Organization:** NextWork.org  
**Date:** April 11–16, 2025  
**Project:** Part 1 of CI/CD Pipeline Series

---

## 📌 Introducing Today's Project

In this project, I laid the foundation for a 7-day CI/CD project by building a web app on AWS using Visual Studio Code (VS Code). I connected to my AWS EC2 instance using SSH directly through VS Code.

---

## 🛠️ Key Tools and Concepts

- **Remote SSH in VS Code**: Connected VS Code to my EC2 instance, enabling direct file editing on the remote server.
- **Terminal Commands**: Used terminal commands to navigate, set permissions, and SSH into the EC2 instance.

---

## 💭 Project Reflection

I faced several unexpected errors during the setup, which turned into valuable learning experiences. This helped me understand the process on a deeper level.

- **Duration**: ~2 hours 15 minutes  
- **Most Challenging**: Connecting VS Code to EC2 using Remote SSH  
- **Most Rewarding**: Solving the errors and gaining broader understanding

---

## 🚀 Launching an EC2 Instance

- The EC2 instance served as the cloud-based server for hosting the web app.
- **SSH Enabled**: For secure access via VS Code.

---

## 🔑 Key Pairs

- Consist of a public key and a private key.
- Private key (`.pem` file) was downloaded during setup for secure SSH login.

---

## 🖥️ Setting up VS Code

- Installed VS Code for editing web app code.
- Installed **Remote - SSH** extension to work on files directly in the EC2 instance.

---

## 💻 My First Terminal Commands

Navigate to the project repository:

```bash
cd ~/Repos/Nextwork-Devops

