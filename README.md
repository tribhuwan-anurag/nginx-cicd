# Cloud-Native CI/CD Pipeline with Kubernetes

## Project Overview

This project demonstrates a full DevOps CI/CD pipeline that automates the process of building, packaging, and deploying a containerized web application using modern cloud infrastructure.

The system uses GitHub Actions for continuous integration, Docker for containerization, DockerHub as the container registry, and Kubernetes running on AWS EC2 for orchestration and deployment.

The pipeline automatically builds and deploys the application whenever new code is pushed to the repository.

---

## Tech Stack

Cloud Infrastructure
- AWS EC2

Containerization
- Docker

Container Registry
- DockerHub

CI/CD
- GitHub Actions

Container Orchestration
- Kubernetes (Minikube)

Web Server
- Nginx

---

## Architecture

Developer pushes code to GitHub.

GitHub Actions pipeline automatically:

1. Builds a Docker image
2. Pushes the image to DockerHub
3. Connects to EC2
4. Updates the Kubernetes deployment

Kubernetes performs a rolling update to deploy the new application version without downtime.

---

## Project Structure
