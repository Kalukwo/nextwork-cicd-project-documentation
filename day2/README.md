## 📄 View PDF Report

[Click here to view Day 2 PDF in your browser](https://docs.google.com/viewer?url=https://raw.githubusercontent.com/Kalukwo/nextwork_CICD_project/main/day2/day2.pdf) *(right click & open in a new tab)*


# Connect a GitHub Repo with AWS

**Author:** Shadrack Kalukwo  
**Platform:** [NextWork.org](https://nextwork.org)  
**Project Date:** April 13th, 2025  


## 📌 Project Overview

This project focuses on storing a web application's code in a Git repository and connecting that repository to AWS. It is part two of a DevOps project series aimed at building a CI/CD pipeline.

**Estimated Time:** ~2 hours  
**Most Challenging Part:** Setting up and using GitHub access tokens  
**Most Rewarding Part:** Solving each error faced during the process  



## 🧰 Key Tools and Concepts

- **Tools Used:** GitHub, Git, AWS EC2, VSCode  
- **Key Concepts:**
  - GitHub Access Tokens
  - Pushing Changes to GitHub
  - Connecting GitHub Repo to Local Repo

---

## 🔧 Git and GitHub Basics

**Git** is a distributed version control system that tracks changes in files over time.  
Installation on Linux (Fedora-based distros):

```bash
sudo dnf install git -y
git --version
```

**GitHub** is a cloud-based hosting service for Git repositories. It allows remote collaboration and access from anywhere.

---

## 📂 My Local Repository

A Git repository contains all project files and their version history.

- Initialized repository using:
  ```bash
  git init
  ```
- Directory used: `nextwork-web-project`

### Branching
Git branches represent alternate versions of a project and act as lightweight, movable pointers to specific commits.

---

## 🚀 Pushing Changes to GitHub

Commands used:

```bash
git add .
git commit -m "Updated index.jsp with new content"
git push -u origin master
```

- `git add .`: Stages all changes
- `git commit`: Saves a snapshot of staged changes
- `git push`: Sends committed changes to GitHub
- `-u`: Sets the upstream (origin/master)

---

## 🔐 Authentication

When pushing to GitHub, Git requests credentials to verify identity.

### Local Git Identity

Set up your Git identity to track who made each change:

```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

Use `git log` to see commit history.

---

## 🧾 GitHub Tokens

GitHub no longer supports password authentication over HTTPS. Use a **Personal Access Token (PAT)** instead.

### How to Create a Token:

1. Go to GitHub > **Settings**
2. Navigate to **Developer Settings**
3. Generate a new token with the required scopes

Tokens are used in place of passwords for HTTPS Git operations.

---

## ✍️ Making More Changes

To test Git tracking:

1. Update your code (e.g., `index.jsp`)
2. Save changes locally
3. Push to GitHub using:

```bash
git add .
git commit -m "Updated a line to my index.jsp"
git push
```

Changes appeared on GitHub after pushing.



```

---

Would you like me to save and send this as a `.md` file too?
