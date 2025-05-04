# DevOps Project - Day 5: Web App Deployment with AWS CodeDeploy

This project is part of a 7-day DevOps learning series focused on building a CI/CD pipeline. On Day 5, I focused on deploying a Java web application using AWS CodeDeploy, leveraging deployment scripts, CloudFormation, and EC2 tagging to automate the release process.

## 📄 View PDF Report

<a href="https://docs.google.com/viewer?url=https://raw.githubusercontent.com/Kalukwo/nextwork_CICD_project/main/day5/day5.pdf" target="_blank" rel="noopener noreferrer">
  Click here to view Day5 PDF in your browser
</a> (right click to open in a new tab)

## 🔧 Tools & Technologies

- AWS CodeDeploy
- AWS CodeBuild
- AWS EC2
- AWS S3
- AWS CloudFormation
- AWS CodeArtifact
- AWS CodeConnection
- IAM Roles & Policies
- VSCode
- GitHub
- appspec.yml
- Deployment Scripts

## 🗂️ What I Did

- Launched a production EC2 instance and supporting VPC resources using CloudFormation
- Created an IAM role for CodeDeploy to access EC2 instances
- Tagged EC2 instances with `role=webserver` to link them to the deployment group
- Wrote deployment scripts:
  - `install_dependencies.sh` to install Tomcat and other dependencies
  - `start_server.sh` to start Apache and Tomcat servers
  - `stop_server.sh` to stop the servers during deployments
- Created an `appspec.yml` to orchestrate deployment steps
- Updated `buildspec.yml` to package deployment scripts and `appspec.yml` into the build artifact
- Set up a CodeDeploy application and deployment group
- Used S3 as the revision location for the deployment artifact
- Verified successful deployment by accessing the public IPv4 DNS of the EC2 instance

## 💡 Key Learnings

- How to use CloudFormation to automate infrastructure provisioning
- The role of `appspec.yml` in defining deployment instructions for CodeDeploy
- Importance of separating development and production environments
- How EC2 instance tagging streamlines deployment group management
- How deployment scripts automate complex server setup tasks

## 🧠 Reflection

This project took about three hours to complete, including troubleshooting. The most challenging aspect was understanding the separation between development and deployment environments, but seeing the live deployed web app made it worthwhile.

## 📅 Timeline

- Time Spent: ~3 hours
- Project Dates: April 18th – April 19th, 2025 (Day 5 completed)
