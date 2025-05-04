# DevOps Project - Day 4: Continuous Integration with AWS CodeBuild

This project is part of a 7-day DevOps learning series focused on building a CI/CD pipeline. On Day 4, I focused on setting up AWS CodeBuild to compile and package a Java web application directly from a GitHub repository, using CodeArtifact, a `buildspec.yml`, and CloudWatch for monitoring.

## 📄 View PDF Report

<a href="https://docs.google.com/viewer?url=https://raw.githubusercontent.com/Kalukwo/nextwork_CICD_project/main/day4/day4.pdf" target="_blank" rel="noopener noreferrer">
  Click here to view Day4 PDF in your browser
</a> (right click to open in a new tab)

## 🔧 Tools & Technologies

- AWS CodeBuild
- AWS CodeArtifact
- AWS CodeConnections
- IAM Roles & Policies
- GitHub
- buildspec.yml
- CloudWatch Logs
- Amazon S3

## 🗂️ What I Did

- Created a new CodeBuild project and configured it from scratch
- Connected CodeBuild to a GitHub repository using CodeConnections and GitHub App credentials
- Defined the build process in a `buildspec.yml` file with four phases:
  - Installed Java and authenticated with CodeArtifact
  - Compiled the Java web app using Maven
  - Packaged the build output into a ZIP artifact
- Enabled CloudWatch Logs to monitor the build process and debug errors
- Created an S3 bucket to store the resulting build artifacts
- Resolved build errors by updating IAM policies for CodeBuild to access CodeArtifact

## 💡 Key Learnings

- How to configure and connect CodeBuild to GitHub securely using CodeConnections
- The structure and purpose of a `buildspec.yml` file in defining CI workflows
- The importance of IAM roles and permissions in enabling build access to resources like CodeArtifact
- How CodeBuild integrates with S3 to output build artifacts and with CloudWatch for troubleshooting

## 🧠 Reflection

This project took approximately four hours. Troubleshooting build errors was challenging but highly educational. Each failed build helped deepen my understanding of AWS services, especially how IAM roles, CodeBuild, and CodeArtifact work together in a CI pipeline.

## 📅 Timeline

- Time Spent: ~4 hours
- Project Dates: April 16th – April 17th, 2025 (Day 4 completed)
