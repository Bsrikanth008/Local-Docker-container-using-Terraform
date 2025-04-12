
# **Terraform Docker Container Provisioning**

This repository demonstrates how to provision a local Docker container using **Terraform**, running an **Nginx** web server. It showcases Infrastructure as Code (IaC) principles for automated, consistent, and scalable container deployment.

---

## **📚 Table of Contents**

- [Project Overview](#project-overview)  
- [Requirements](#requirements)  
- [Setup Instructions](#setup-instructions)  
- [Usage](#usage)  
- [Destroying Resources](#destroying-resources)  
- [Troubleshooting](#troubleshooting)  
- [Contributing](#contributing)  
- [License](#license)  
- [Acknowledgements](#acknowledgements)  

---

## **📌 Project Overview**

This project uses **Terraform** to automate the provisioning of a local **Docker** container running the **Nginx** web server. By leveraging Terraform, infrastructure becomes reproducible and manageable — a core practice in DevOps.

---

## **✅ Requirements**

Ensure the following tools are installed:

- [Terraform](https://www.terraform.io/downloads.html) (v0.12 or later)  
- [Docker](https://docs.docker.com/get-docker/) (running locally)  
- Internet connection to fetch Terraform provider plugins  

---

## **⚙️ Setup Instructions**

1. **Clone the Repository**  
   ```bash
   git clone https://github.com/Bsrikanth008/Local-Docker-container-using-Terraform.git
   cd Local-Docker-container-using-Terraform
   ```

2. **Initialize Terraform**  
   ```bash
   terraform init
   ```

3. **Plan the Configuration (Optional but Recommended)**  
   ```bash
   terraform plan
   ```

4. **Apply the Configuration**  
   ```bash
   terraform apply
   ```
   Type `yes` when prompted to proceed.

5. **Verify Docker Container**  
   ```bash
   docker ps
   ```
   Open your browser and visit: [http://localhost:9090](http://localhost:9090)

---

## **▶️ Usage**

- **Start Container (if stopped):**  
  ```bash
  docker start my-nginx-container
  ```

- **Stop Container:**  
  ```bash
  docker stop my-nginx-container
  ```

- **Access Web Server:**  
  Navigate to: [http://localhost:9090](http://localhost:9090)

---

## **🧹 Destroying Resources**

To clean up all Terraform-managed resources:

```bash
terraform destroy
```
Type `yes` to confirm.

---

## **🛠 Troubleshooting**

- **Reinitialize Terraform:**  
  ```bash
  terraform init -reconfigure
  ```

- **Check Docker Status:**  
  ```bash
  docker info
  ```

- **Permission Issues (Linux):**  
  Run with elevated permissions:  
  ```bash
  sudo terraform apply
  ```

- **Manual Cleanup (if needed):**  
  ```bash
  docker stop my-nginx-container
  docker rm my-nginx-container
  ```

---

## **🤝 Contributing**

Contributions are welcome! To contribute:

1. Fork the repository  
2. Create a feature branch  
3. Commit your changes  
4. Open a pull request  

---
## Author

Created as part of the **Elevate Labs DevOps Internship** by Srikanth Berla.

## License

This project is intended for educational purposes.

## **🙏 Acknowledgements**

- [Terraform](https://www.terraform.io/)  
- [Docker](https://www.docker.com/)  
- [Nginx](https://www.nginx.com/)
