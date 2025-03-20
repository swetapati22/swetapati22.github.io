---
layout: page
title: MultiCloud, DevOps & AI eCommerce Platform
description: A multi-cloud powered eCommerce platform leveraging AWS, Google Cloud, and Azure, featuring automated CI/CD pipelines, Kubernetes orchestration, AI-driven recommendations, customer support, and Azure Text Analytics with Google BigQuery Integration.
img: assets/img/devops.png
importance: 3
category: cloud-devops
---
    ---
    Source Code available in the repository
    Github handle: swetapati22
    Project: CloudMart - MultiCloud, DevOps & AI eCommerce Platform
    ---

📂 **Source Code**: <a href="https://github.com/swetapati22/MultiCloud_DevOps_AI_Project" target="_blank">GitHub Repository</a>  
🎥 **Demo Video**: <a href="https://youtu.be/_LvKL2LE5qU" target="_blank">Watch Demo</a>

---

## **Overview**
CloudMart is an AI-powered eCommerce platform designed to operate seamlessly across AWS, Google Cloud, and Azure. This project demonstrates expertise in multi-cloud infrastructure, CI/CD automation, Kubernetes orchestration, and AI-powered integrations leveraging Amazon Bedrock, OpenAI Assistants, and Azure Text Analytics. Additionally, Google BigQuery Integration for Order Tracking & Analytics. 

It covers in:

- **Automated Infrastructure Deployment** using Terraform  
- **Containerized App Deployment** with Docker & Kubernetes  
- **CI/CD Pipeline** using AWS CodePipeline & CodeBuild  
- **AI-Powered Product Recommendations** with Amazon Bedrock  
- **AI Chatbot for Customer Support** powered by OpenAI  
- **Order Tracking & Analytics** using Google BigQuery  
- **Sentiment Analysis** with Azure Text Analytics  

This project **automates the entire cloud deployment lifecycle**—from **infrastructure provisioning** using Terraform to **end-to-end CI/CD deployment** and **AI-driven analytics**.

---

## **Tech Stack**
- **Cloud Providers:** AWS, Google Cloud, Azure  
- **Infrastructure as Code:** Terraform  
- **CI/CD Automation:** AWS CodePipeline, AWS CodeBuild  
- **Containerization & Orchestration:** Docker, Kubernetes (EKS)  
- **AI & ML Services:** Amazon Bedrock, OpenAI, Azure Text Analytics  
- **Data Processing & Storage:** AWS DynamoDB, Google BigQuery  

---

## **Deployment Steps**
Each task is **detailed in individual GitHub README files (link can be found within each task description below)**:

### **1️⃣ Provision AWS Infrastructure using Terraform**
📄 [See Detailed Steps](https://github.com/swetapati22/MultiCloud_DevOps_AI_Project/blob/main/task_specific_README/Task1_README.md)

- Deploy **EC2 instances, IAM roles, and DynamoDB** using Terraform.  
- Initialize Terraform and apply configuration:
  ```bash
  cd terraform-project
  terraform init
  terraform apply
  ```

---

### **2️⃣ Build & Deploy CloudMart Application**
📄 [See Detailed Steps](https://github.com/swetapati22/MultiCloud_DevOps_AI_Project/blob/main/task_specific_README/Task2_README.md)

- **Dockerize Backend & Frontend**:
  ```bash
  docker build -t cloudmart-backend application_source_code/backend/
  docker build -t cloudmart-frontend application_source_code/frontend/
  ```
- **Push images to AWS ECR**:
  ```bash
  docker push <ECR_REPO_URI>/cloudmart-backend:latest
  docker push <ECR_REPO_URI>/cloudmart-frontend:latest
  ```

---

### **3️⃣ Deploy Kubernetes Cluster on AWS EKS**
📄 [See Detailed Steps](https://github.com/swetapati22/MultiCloud_DevOps_AI_Project/blob/main/task_specific_README/Task3_README.md)

- Create an **EKS Cluster**:
  ```bash
  eksctl create cluster --name cloudmart --region us-east-1 --nodes 1
  aws eks update-kubeconfig --name cloudmart
  ```
- Deploy the backend & frontend using Kubernetes manifests:
  ```bash
  kubectl apply -f application_source_code/backend/cloudmart-backend.yaml
  kubectl apply -f application_source_code/frontend/cloudmart-frontend.yaml
  ```

---

### **4️⃣ Set Up CI/CD Pipeline**
📄 [See Detailed Steps](https://github.com/swetapati22/MultiCloud_DevOps_AI_Project/blob/main/task_specific_README/Task4_README.md)

- **Configure AWS CodePipeline** to automate builds & deployments.  
- Add `buildspec.yml` to repositories for CI/CD automation.  
- Push changes to GitHub to trigger deployment.

---

### **5️⃣ Integrate AI & Data Processing**
📄 [See Detailed Steps](https://github.com/swetapati22/MultiCloud_DevOps_AI_Project/blob/main/task_specific_README/Task5_README.md)

#### **Amazon Bedrock for AI-Driven Product Recommendations**
- Deploy AWS Lambda function: `application_source_code/backend/src/lambda/list_products.zip`
- Configure **Amazon Bedrock Agent** via Terraform in `terraform-project/main.tf`

#### **OpenAI Assistant for AI-Powered Customer Support**
- Store API Key in **`application_source_code/backend/.env`**
- Modify Kubernetes deployment file **`application_source_code/backend/cloudmart-backend.yaml`** to integrate the assistant.

#### **Google Cloud BigQuery for Order Tracking & Data Analytics**
- Set up a **BigQuery Dataset** and create an **orders table**.
- Deploy AWS Lambda: `application_source_code/backend/src/lambda/addToBigQuery.zip`

#### **Azure Text Analytics for Sentiment Analysis**
- Update `application_source_code/backend/cloudmart-backend.yaml` with Azure API credentials.

---

## **Major Takeaways**
- **Cloud-Native eCommerce**: Fully automated deployment of a multi-cloud AI-powered eCommerce system.  
- **Multi-Cloud Deployment**: Seamless integration with AWS, Google Cloud, and Azure.  
- **End-to-End CI/CD**: Automated application builds & deployments via AWS CodePipeline.  
- **AI-Powered Recommendations**: Intelligent customer assistance using Amazon Bedrock for Product Recommendation Agent & OpenAI for Customer Support Agent.  
- **Scalable Kubernetes Orchestration**: Running backend & frontend on AWS EKS with Terraform.  
- **Data Analytics Integration**: Leveraging **Google BigQuery** & **Azure Text Analytics** for business insights.

