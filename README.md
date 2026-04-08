# Google-Cloud-Infrastructure-Deployment-using-Terraform-VPC-Firewall-VM-
This project demonstrates provisioning a Google Cloud VPC network, firewall rules, and VM instances using Terraform. It was implemented as part of a hands-on lab using Google Cloud Shell and Infrastructure as Code (IaC) best practices.
# Infrastructure as Code with Terraform on Google Cloud

##  Overview
This project demonstrates how to provision and manage Google Cloud infrastructure using Terraform and Infrastructure as Code (IaC) principles.

##  Resources Created
- VPC Network (Auto mode)
- Firewall rule (allow HTTP, SSH, RDP, ICMP)
- Virtual Machine instance using a reusable Terraform module

##  Technologies Used
- Terraform
- Google Cloud Platform (GCP)
- Compute Engine
- VPC Networking

---

##  Architecture Diagram

Terraform

↓

VPC Network (mynetwork)

   ↙       ↘

Firewall     VM Instance

---

## 📂 Project Structure

tfinfra/

├── provider.tf

├── mynetwork.tf

└── instance/

├── main.tf

└── variables.tf

---

##  Sample Terraform Resource

```hcl
resource "google_compute_network" "mynetwork" {
  name                    = "mynetwork"
  auto_create_subnetworks = true
}

 How to Deploy

terraform init
terraform plan
terraform apply

 Screenshots

Terraform Apply Success

VPC Network

Firewall Rule

VM Instance

SSH Connection

Project Structure

 Key Learning Outcomes
 • Understanding Terraform modules
 • Deploying infrastructure using IaC
 • Managing GCP networking and firewall rules
  
