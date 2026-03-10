# Automated Cloud Deployment with AWS, Kubernetes, and Jenkins

This project demonstrates an automated CI/CD pipeline that builds, containerizes, and deploys a web application to a Kubernetes cluster on AWS. The pipeline uses Jenkins to automate the entire workflow from code commit to production deployment.

The goal of the project is to showcase how modern DevOps practices can be used to build scalable, reliable deployment pipelines using containerization and cloud-native infrastructure.

---

## Overview

Modern software systems require reliable deployment pipelines that allow teams to ship updates quickly and safely. This project implements a CI/CD pipeline that automates the process of building, packaging, and deploying applications to a Kubernetes environment.

The pipeline performs the following tasks:

1. Detects code changes from a Git repository
2. Builds the application
3. Creates a Docker container image
4. Pushes the image to Amazon Elastic Container Registry (ECR)
5. Deploys the containerized application to a Kubernetes cluster running on Amazon EKS
6. Exposes the application through a Kubernetes LoadBalancer

This setup ensures that application updates can be deployed consistently and efficiently.

---

## Architecture

The system follows the workflow below:

Developer Pushes Code  
↓  
GitHub Repository  
↓  
Jenkins CI/CD Pipeline  
↓  
Docker Image Build  
↓  
Push Image to AWS ECR  
↓  
Kubernetes Deployment on AWS EKS  
↓  
Application Exposed via LoadBalancer

---

## Key Features

- Automated CI/CD pipeline using Jenkins
- Containerized application using Docker
- Kubernetes orchestration for scalable deployments
- AWS cloud infrastructure for hosting and deployment
- Automated build and deployment workflow
- Infrastructure designed for reliability and scalability

---

## Tech Stack

**Cloud Platform**  
AWS

**Containerization**  
Docker

**Container Orchestration**  
Kubernetes (Amazon EKS)

**CI/CD Automation**  
Jenkins

**Container Registry**  
Amazon Elastic Container Registry (ECR)

**Version Control**  
Git / GitHub

---

## AWS Services Used

- Amazon EC2 – Jenkins server hosting
- Amazon EKS – Kubernetes cluster
- Amazon ECR – Docker image storage
- AWS IAM – Access control
- AWS VPC – Network configuration
- AWS Load Balancer – Service exposure

---

## CI/CD Pipeline Workflow

1. Code is pushed to the GitHub repository.
2. Jenkins pipeline is triggered automatically.
3. Jenkins builds the application and creates a Docker image.
4. The Docker image is pushed to Amazon ECR.
5. Kubernetes deployment files are updated.
6. The new container image is deployed to the EKS cluster.
7. The application becomes available through a LoadBalancer.

---

## Repository Structure

