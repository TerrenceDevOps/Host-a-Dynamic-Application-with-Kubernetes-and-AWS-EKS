# Host-a-Dynamic-Application-with-Kubernetes-and-AWS-EKS

# Hosting Dynamic Applications with Kubernetes and AWS EKS

This repository contains resources and scripts used to deploy a dynamic application using Kubernetes on AWS Elastic Kubernetes Service (EKS). The project demonstrates a complete DevOps pipeline, covering containerization, orchestration, security, and scalability.

## Architecture Overview

The application is deployed on AWS EKS with the following key components:

- **Git and GitHub**: Used for version control and collaboration.
- **Docker**: Installed to build and manage containers.
- **Dockerfiles**: Created to containerize the application.
- **Amazon Elastic Container Registry (ECR)**: Stores Docker images.
- **Amazon Relational Database Service (RDS)**: Stores application data securely.
- **AWS Secrets Manager**: Manages and secures sensitive data.
- **Amazon Route 53**: Handles domain name resolution.
- **AWS Elastic Kubernetes Service (EKS)**: Orchestrates containerized applications.
- **kubectl, eksctl, and Helm**: Essential tools for managing Kubernetes deployments.
- **Kubernetes Manifests**: Define application components.
- **EKS Cluster**: Hosts the Kubernetes workloads.
- **CI/CD Pipeline**: Automates build, test, and deployment processes.

## Deployment Steps

1. **Set Up AWS and Install Necessary Tools**
   - Configure AWS CLI
   - Install Docker, kubectl, eksctl, and Helm
   
2. **Build and Push Docker Images to ECR**
   - Write Dockerfile for the application
   - Build the Docker image
   - Push the image to Amazon ECR

3. **Set Up Amazon RDS**
   - Create an RDS instance
   - Configure the database connection

4. **Store Secrets Securely**
   - Use AWS Secrets Manager to store sensitive credentials
   - Access secrets in Kubernetes using environment variables

5. **Create an EKS Cluster**
   - Use eksctl to create the cluster
   - Configure kubectl to interact with the cluster

6. **Deploy the Application on EKS**
   - Write Kubernetes deployment and service files
   - Apply configurations using `kubectl apply`
   - Expose the application using a Load Balancer

7. **Configure DNS with Route 53**
   - Register a domain and set up DNS records

8. **Monitor and Scale**
   - Use Kubernetes auto-scaling and monitoring tools

## Lessons Learned

- **Containerization Best Practices**: Writing efficient Dockerfiles to optimize application performance.
- **Security Management**: Using AWS Secrets Manager to securely store credentials.
- **Kubernetes Orchestration**: Managing workloads and networking in Kubernetes.
- **CI/CD Automation**: Automating deployment with GitHub Actions.
- **DNS Configuration Challenges**: Overcame issues in setting up Route 53 for smooth domain resolution.

## How to Use

1. Clone this repository to your local machine.
2. Follow the deployment steps to set up AWS services.
3. Run the Kubernetes manifests to deploy the application.
4. Configure Route 53 for DNS resolution.
5. Monitor and scale the application as needed.

## Contributing

Contributions and improvements are welcome! Please fork this repository and submit a pull request with your changes.

