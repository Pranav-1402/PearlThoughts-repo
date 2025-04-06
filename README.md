# Medusa Backend Deployment on AWS ECS Fargate

This project demonstrates deploying a containerized Medusa backend to AWS ECS using Terraform and GitHub Actions for CI/CD.

## Folder Structure

- `docker/` - Dockerfile for Medusa backend
- `terraform/` - Infrastructure as Code for ECS, VPC, etc.
- `.github/workflows/` - GitHub Actions workflow

## How It Works

1. Medusa backend is containerized using Docker.
2. Infrastructure is provisioned using Terraform.
3. GitHub Actions automates the deployment process.

## CI/CD

- Trigger: On push to `main`
- Actions:
  - Terraform Init/Plan/Apply
  - Docker Build & Push
  - ECS Deploy

## Author

Your Name
