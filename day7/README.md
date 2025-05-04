# DevOps Project - Day 7: End-to-End CI/CD Pipeline with AWS CodePipeline

This project is part of a 7-day DevOps learning series focused on building a CI/CD pipeline. On Day 7, I implemented a complete end-to-end CI/CD pipeline using AWS CodePipeline to automate deployments from GitHub to production via CodeBuild and CodeDeploy.

## 📄 View PDF Report

<a href="https://docs.google.com/viewer?url=https://raw.githubusercontent.com/Kalukwo/nextwork_CICD_project/main/day7/day7.pdf" target="_blank" rel="noopener noreferrer">
  Click here to view Day7 PDF in your browser
</a> (right click to open in a new tab)

## 🔧 Tools & Technologies

- AWS CodePipeline
- AWS CodeBuild
- AWS CodeDeploy
- GitHub
- CodeConnections
- IAM Roles
- VSCode
- Webhooks
- appspec.yml
- Deployment Scripts

## 🗂️ What I Did

- Set up a CodePipeline to automate the flow from GitHub (source) to CodeDeploy (production deployment)
- Configured three CI/CD pipeline stages:
  - **Source**: Connected GitHub as the source repository with webhook events for automatic triggers
  - **Build**: Used AWS CodeBuild to compile and package the Java web app using artifacts from GitHub
  - **Deploy**: Deployed build artifacts to EC2 using AWS CodeDeploy and an existing deployment group
- Enabled superceded execution mode in CodePipeline to prioritize the latest run and cancel outdated ones
- Verified the pipeline by pushing changes to the GitHub repository and observing successful live deployment

## 💡 Key Learnings

- How to connect all stages (source, build, deploy) into a streamlined CI/CD workflow using CodePipeline
- The role of webhook events in
