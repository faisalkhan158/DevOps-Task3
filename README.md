# 🚀 DevOps Task 3 - Infrastructure as Code (IaC) with Terraform

## 📌 Objective  
Provision a local Docker container using Terraform to understand the core principles of Infrastructure as Code.

## 🛠️ Tools & Technologies  
- Terraform  
- Docker  
- NGINX  

## 📦 Infrastructure Overview  
This task provisions an NGINX container on a Docker host using Terraform. The infrastructure is managed entirely through code using the Docker provider.

## 🔄 Terraform Workflow  
- `terraform init` – Initializes Terraform environment  
- `terraform plan` – Previews changes before applying  
- `terraform apply` – Provisions NGINX Docker container  
- `terraform destroy` – Tears down the container  
- `terraform state` – Used to inspect Terraform-managed resources  

## 📁 Project Files  
- `main.tf` – Terraform file defining the Docker provider, image, and container  
- `terraform.tfstate` – Tracks the current infrastructure state (auto-generated)  
- `execution_logs.txt` – Captured terminal outputs of Terraform commands  

## ⚠️ Pre-requisites  
- Docker must be installed and running on the machine  
- Terraform installed (v1.6+ recommended)  
- Add user to Docker group:  
  ```bash
  sudo usermod -aG docker $USER && newgrp docker
