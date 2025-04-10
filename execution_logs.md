terraform init       | tee -a execution_logs.md
terraform plan       | tee -a execution_logs.md
terraform apply -auto-approve  | tee -a execution_logs.md
terraform state list | tee -a execution_logs.md
terraform destroy -auto-approve | tee -a execution_logs.md
