# Dockerized Python App → Docker Hub + AWS ECR

## Purpose
Containerize a Python Flask app and automatically push it to Docker Hub and AWS ECR using GitHub Actions. Demonstrates deployment to AWS ECS with CI/CD automation.

## Tech Used
- Python 3.10+ (Flask)  
- Docker (containerization)  
- Docker Hub & AWS ECR (image registries)  
- AWS ECS (deployment)  
- GitHub Actions (CI/CD pipeline, secrets, caching, artifacts)  

## Issues & Solutions
| Issue | Solution |
|-------|---------|
| Docker login failed in GitHub Actions | Ensure Docker Hub username/token secrets are correct and referenced properly |
| AWS ECR push denied | Use IAM user with full ECR permissions and correct AWS secrets |
| Slow pip install | Use caching in GitHub Actions to speed up builds |

## Outcomes
- Flask app successfully containerized with Docker  
- Docker image automatically pushed to Docker Hub & AWS ECR  
- CI/CD pipeline handles automated deployment to AWS ECS  
- Demonstrates real-world DevOps practices with caching, secrets, and artifacts
