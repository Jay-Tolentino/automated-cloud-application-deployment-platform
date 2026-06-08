# Automated Cloud Application Deployment Platform (AWS, Linux & GitHub Actions)

## Overview

This project implements a basic CI/CD deployment pipeline using GitHub Actions and AWS EC2 to automate application deployments.

The objective was to reduce manual deployment work and create a repeatable process that updates a live Linux environment directly from source control.

---

## Architecture

Developer

↓

GitHub Repository

↓

GitHub Actions

↓

SSH Deployment

↓

AWS EC2 (Ubuntu)

↓

Live Application

---

## Technologies Used

- AWS EC2
- Ubuntu Linux
- GitHub Actions
- Git
- GitHub
- SSH
- Bash

---

## Features

- Provisioned Linux infrastructure in AWS
- Configured secure SSH access
- Automated deployment workflow
- Triggered deployments through GitHub pushes
- Reduced manual update process

---

## Deployment Workflow

### 1. Push Code

```bash
git push
```

### 2. GitHub Actions Trigger

Workflow automatically starts.

### 3. Connect to EC2

```bash
ssh ubuntu@server
```

### 4. Deploy

```bash
git pull
```

---

## Repository Structure

```
automated-cloud-application-deployment-platform
│
├── screenshots
├── notes
├── .github
│   └── workflows
└── README.md
```

---

## CI/CD Benefits

- Faster deployments
- Reduced human error
- Repeatable infrastructure process
- Continuous delivery workflow

---

## Future Improvements

- Docker deployment
- Blue/Green deployment
- CloudWatch monitoring
- Terraform provisioning
- Deployment notifications
