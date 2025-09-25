# Task 3: Infrastructure as Code (IaC) with Terraform

## Objective
Provision a local Docker container using Terraform and manage its lifecycle.

## Tools Used
- Terraform  
- Docker  

## Workflow
1. **Terraform Configuration**  
   - Wrote `main.tf` using the Terraform **Docker provider**.  
   - Defined a Docker image (nginx) and container resource.  

2. **Initialize**  
   - Ran `terraform init` to download provider plugins.  

3. **Plan**  
   - Executed `terraform plan` to preview resources to be created.  

4. **Apply**  
   - Ran `terraform apply` to provision the Docker container.  
   - Verified with `docker ps`.  
   - Accessed the container on `http://localhost:8080` in the browser.  

5. **State Check**  
   - Used `terraform state list` to confirm Terraform is tracking the resources.  

6. **Destroy**  
   - Ran `terraform destroy` to remove the container and clean up infrastructure.  

## Deliverables
- `main.tf` file (Terraform configuration).  
- Execution screenshots of:  
  - `terraform plan`  
  - `terraform apply`  
  - Container running on browser  
  - `terraform destroy`  

## Result
The workflow was successful. Terraform provisioned the Docker container, served the application in the browser, and destroyed the resources when instructed.

