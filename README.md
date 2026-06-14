# Three-Tier Microservices Deployment on AWS EKS

## Project Overview

This project demonstrates the deployment of a three-tier microservices application on AWS Elastic Kubernetes Service (EKS) using Kubernetes. The application consists of multiple microservices along with frontend and backend components deployed inside an EKS cluster.

The project includes Kubernetes manifests, EKS configuration, IAM OIDC setup, ALB Ingress configuration, and persistent storage integration using the EBS CSI Driver.

---

## Architecture

The application follows a three-tier architecture:

- Frontend Web Application
- Backend Microservices
- Database Layer (MySQL and MongoDB)

The application is deployed on AWS EKS using Kubernetes resources and exposed using AWS Application Load Balancer (ALB).

---

## Technologies Used

- AWS EKS
- Kubernetes
- Docker
- Helm
- IAM OIDC
- AWS ALB Ingress Controller
- EBS CSI Driver
- GitHub
- YAML

---

## Project Structure

EKS/           -> EKS cluster setup and configuration
K8s/           -> Kubernetes manifests
cart/          -> Cart microservice
catalogue/     -> Catalogue microservice
dispatch/      -> Dispatch microservice
mongodb/       -> MongoDB database configuration
mysql/         -> MySQL database configuration
payment/       -> Payment microservice
ratings/       -> Ratings microservice
shipping/      -> Shipping microservice
user/          -> User microservice
web/           -> Frontend application

---

## Features

-Deployment of microservices on AWS EKS
-Kubernetes-based orchestration
-ALB Ingress configuration for external access
-IAM OIDC integration
-Persistent storage using EBS CSI Driver
-Containerized application deployment using Docker

---

##Deployment Steps:

1. Create EKS Cluster
Create the AWS EKS cluster using eksctl.
2. Configure IAM OIDC Provider
Associate IAM OIDC provider with the EKS cluster.
3. Install ALB Ingress Controller
Configure AWS Load Balancer Controller for ingress traffic management.
4. Configure EBS CSI Driver
Install and configure EBS CSI Driver for persistent volumes.
5. Deploy Kubernetes Resources
Apply Kubernetes manifests for all services.


kubectl apply -f .

---

7. Verify Deployments

   
kubectl get pods

kubectl get svc

kubectl get ingress

---

##Screenshots
Screenshots of cluster setup, running pods, services, and application UI will be added here.

##Key Learnings

-Understanding Kubernetes architecture

-Deploying workloads on AWS EKS

-Working with Kubernetes manifests

-Configuring ALB ingress routing

-Managing persistent storage using EBS CSI Driver

-Deploying microservices-based applications

---
