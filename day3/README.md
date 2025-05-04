# DevOps Project - Day 3: Secure Package Management with AWS CodeArtifact

This project is part of a 7-day DevOps learning series focused on building a CI/CD pipeline. On Day 3, I focused on securely retrieving software packages for my Java web application using AWS CodeArtifact, IAM roles, and Maven.

## 📄 View PDF Report

<a href="https://docs.google.com/viewer?url=https://raw.githubusercontent.com/Kalukwo/nextwork_CICD_project/main/day3/day3.pdf" target="_blank" rel="noopener noreferrer">
  Click here to view Day3 PDF in your browser
</a> (right click to open in a new tab)

## 🔧 Tools & Technologies

- AWS CodeArtifact
- IAM Roles & Policies
- Maven
- AWS EC2
- settings.xml configuration

## 🗂️ What I Did

- Created a CodeArtifact domain and repository for storing Java dependencies
- Linked the repository to an upstream source (`maven-central-store`) for fallback packages
- Encountered and resolved authorization issues by:
  - Creating a custom IAM policy
  - Attaching it to an EC2 instance via an IAM role
- Exported a temporary CodeArtifact token to authenticate Maven requests
- Configured Maven’s `settings.xml` to use the CodeArtifact repository
- Successfully compiled the Java web app using dependencies pulled from CodeArtifact

## 💡 Key Learnings

- How AWS CodeArtifact works as a secure, centralized package store
- Why IAM roles and temporary credentials are preferred over static ones
- How Maven integrates with external package repositories using profiles and tokens

## 🧠 Reflection

While setting up the IAM role and debugging permissions was a bit complex, it was satisfying to see the packages compile successfully and verify them in the CodeArtifact console.

## 📅 Timeline

- Time Spent: ~2 hours
- Project Dates: April 13th – April 14th, 2025 (Day 3 completed)
