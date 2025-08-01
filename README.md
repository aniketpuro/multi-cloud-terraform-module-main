# 🌐 Terraform Multi-Cloud Module

**Terraform module to provision multi-cloud infrastructure using Kubernetes services (EKS on AWS, GKE on GCP)**

The goal is to enable a highly available, flexible, and performant infrastructure by deploying workloads across multiple cloud platforms.

---

## 🚀 Prerequisites

- AWS Account
- GCP Project
- CLI Tools:
  - `terraform`
  - `kubectl`
  - `aws`
  - `gcloud`

---

## 🧩 Modules

| Module Name           | Description                              |
|-----------------------|------------------------------------------|
| `aws-eks-vpc`         | EKS-compliant VPC                        |
| `aws-eks-fargate`     | EKS cluster with Fargate profile         |
| `aws-eks-lbc-addon`   | AWS Load Balancer Controller add-on      |
| `aws-ec2-nginx`       | EC2 NGINX server for reverse proxy       |
| `gcp-gke-autopilot`   | GKE cluster in Autopilot mode            |

---

## 🔧 Usage Examples

### ✅ Create EKS Cluster with Fargate and Load Balancer

```bash
cd examples/aws-eks-fargate
cp terraform.tfvars.sample terraform.tfvars

# Edit terraform.tfvars with your AWS credentials
terraform init
terraform apply
✅ Create GKE Autopilot Cluster
bash
Copy
Edit
cd examples/gcp-gke-autopilot
cp terraform.tfvars.sample terraform.tfvars

# Edit terraform.tfvars with your GCP project ID
terraform init
terraform apply
🌐 Deploy Sample App on EKS + GKE
bash
Copy
Edit
cd examples/multi-cloud-sample-app
cp terraform.tfvars.sample terraform.tfvars

# Add AWS & GCP credentials
terraform init
terraform apply
🔁 Provision NGINX Load Balancer on EC2
bash
Copy
Edit
cd examples/multi-cloud-nginx-lb
cp terraform.tfvars.sample terraform.tfvars

# Add AWS & GCP credentials
terraform init
terraform apply
🛣️ Roadmap
✅ AWS EKS Cluster

✅ GKE Autopilot Mode Cluster

🔄 EKS Multi-region (via AWS Global Accelerator)

🔄 GKE Multi-region (via GKE Multi-Cluster Services)

🔄 Multi-cloud load balancing with failover

Clouds Used:
✅ Amazon Web Services (AWS)
✅ Google Cloud Platform (GCP)

vbnet
Copy
Edit

Let me know if you want a project logo, image diagram, or badges added too.
