## 📄 View PDF Report

[Click here to view Day 1 PDF in your browser](https://docs.google.com/viewer?url=https://raw.githubusercontent.com/Kalukwo/nextwork_CICD_project/main/day1/day1.pdf) *(open in a new tab)*



# Set Up a Web App Using AWS and VS Code

**Author:** Shadrack Kalukwo  
**Organization:** NextWork.org  
**Date:** April 11, 2025  
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


Set key permissions:

bash
Copy
Edit
chmod 400 Nextwork-keypair.pem
🔌 SSH Connection to EC2
Connected to EC2 using:

bash
Copy
Edit
ssh -i Nextwork-keypair.pem ec2-user@<your-ec2-ip>
Required the IPv4 address of the EC2 instance.

☕ Java & Maven Setup
Apache Maven: Automates software building.

Java (Amazon Corretto 8): Required to build the web application.

🏗️ Creating the Application
Generated the Java web app using Maven:

bash
Copy
Edit
mvn archetype:generate \
  -DgroupId=com.nextwork.app \
  -DartifactId=nextwork-web-project \
  -DarchetypeArtifactId=maven-archetype-webapp \
  -DinteractiveMode=false
🗂️ Project Structure
src/ and webapp/: Created by Maven, include config and web files.

index.jsp: Edited and customized to reflect my content.

🖱️ Final Thoughts
Using the Remote - SSH extension and VS Code made the development seamless, allowing me to manage and deploy my Java web app directly in the cloud.

css
Copy
Edit

Let me know if you want it styled for a blog post, exported to a PDF, or saved in a file!
