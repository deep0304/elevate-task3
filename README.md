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

  - `terraform init`
  - <img width="737" height="299" alt="terraform init" src="https://github.com/user-attachments/assets/b4f39723-9877-4eef-994c-6315fbe4fa7b" />

  - `terraform plan`
  - <img width="759" height="451" alt="terraform plan" src="https://github.com/user-attachments/assets/957057e0-c6c0-4bd1-bbcc-80cd3f721196" />

  - `terraform apply`
  - <img width="740" height="435" alt="terraform apply" src="https://github.com/user-attachments/assets/b30b2cf9-4499-4f13-b63d-31fbf5cb6bb1" />
  
  - Container running on browser
  - <img width="948" height="423" alt="running image" src="https://github.com/user-attachments/assets/781fb5bc-4446-4fec-977b-74be48ac9983" />

  - `terraform destroy`
  - <img width="704" height="436" alt="terrraform destroy" src="https://github.com/user-attachments/assets/b4c846ec-6fec-4430-8b4f-e8b8410efbd1" />


## Result
The workflow was successful. Terraform provisioned the Docker container, served the application in the browser, and destroyed the resources when instructed.

