
# Terraform Docker Container Provisioning

This repository demonstrates how to provision a local Docker container using **Terraform**. It includes configuration files and automation workflows to streamline container provisioning.

---

## Features

- Provision Docker container locally using Terraform
- Automate infrastructure as code (IaC)
- Minimal configuration, easy to replicate
- GitHub Actions support (optional)

---

## Project Structure

```
.
├── main.tf                          # Terraform configuration file
├── terraform.tfstate               # Terraform state file
├── terraform.tfstate.backup       # Terraform backup state
├── .terraform.lock.hcl            # Terraform dependency lock file
├── .terraform/                    # Terraform plugin and modules directory
├── .github/
│   └── workflows/
│       └── terraform.yml          # GitHub Actions workflow for CI/CD (optional)
└── README.md                      # Project documentation
```

---

## Terraform Workflow Stages

1. **Initialize Terraform** – Set up Terraform working directory and download required providers  
2. **Plan Infrastructure** – Preview actions Terraform will take to achieve desired state  
3. **Apply Configuration** – Create Docker container using defined resources  
4. **Verify** – Confirm Docker container is running locally  

---

## Prerequisites

- Terraform installed on your system  
- Docker installed and running locally  
- GitHub account (if using Actions for CI/CD)

---

## Getting Started

1. Clone this repository:
   ```bash
   git clone https://github.com/Bsrikanth008/Local-Docker-container-using-Terraform.git
   cd Local-Docker-container-using-Terraform
   ```

2. Initialize Terraform:
   ```bash
   terraform init
   ```

3. Review the plan:
   ```bash
   terraform plan
   ```

4. Apply the configuration:
   ```bash
   terraform apply
   ```

---

## Author

Created as part of the **Elevate Labs DevOps Internship** by [Srikanth Berla](https://www.linkedin.com/in/srikanth-berla-9bb743266)

---

## License

This project is intended for educational purposes.
