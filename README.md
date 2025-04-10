## 🚀 Overview
This project uses **Terraform** to provision a **Docker container** running **NGINX** on an **Amazon EC2 Ubuntu instance**.

## 🔧 Tools Used
- Terraform
- Docker
- AWS EC2 (Ubuntu)
- NGINX

## 🛠️ What It Does
- Installs Docker on EC2
- Uses Terraform with the Docker provider
- Pulls the latest NGINX image
- Exposes NGINX on port 8080
- Destroys everything cleanly after testing

## 📁 Files
- `main.tf`: Terraform configuration
- `execution_logs.md`: Command logs and outputs
- `.gitignore`: Prevents Terraform cache files from being tracked

## 🧪 How to Run
```bash
terraform init
terraform plan
terraform apply -auto-approve
# Access via http://<EC2-Public-IP>:8080
terraform destroy -auto-approve

