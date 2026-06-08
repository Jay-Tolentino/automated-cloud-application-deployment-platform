# Deployment Workflow

## Objective
Automatically deploy updates from GitHub to AWS EC2.

## Stack
- AWS EC2
- Ubuntu Linux
- GitHub Actions
- SSH

## Process

1. Push changes to GitHub
2. Trigger GitHub Actions
3. Connect to EC2 through SSH
4. Pull latest code
5. Restart application

## Commands

```bash
git pull
systemctl restart nginx
```
