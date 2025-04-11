Terraform Docker Container Provisioning

This repository demonstrates how to use *Terraform* to provision a *Docker container* locally, running the *Nginx* web server. The project leverages *Infrastructure as Code (IaC)* to automate the setup and management of Docker containers.

## 📑 Table of Contents

- [Project Overview](#project-overview)
- [Requirements](#requirements)
- [Setup Instructions](#setup-instructions)
- [Usage](#usage)
- [Destroying Resources](#destroying-resources)
- [Troubleshooting](#troubleshooting)
- [Contributing](#contributing)
- [License](#license)

---

## 📝 Project Overview

This project demonstrates how to automate the provisioning of a Docker container using *Terraform. The container runs the **Nginx* web server, and it can be easily scaled and managed with Terraform scripts.

By using Terraform, we make the process of setting up Docker containers reproducible and maintainable, which is essential for DevOps workflows.

---

## 🖥 Requirements

Before you begin, ensure you have the following installed:

- *Terraform* (v0.12 or later)
- *Docker* (installed and running locally)
- A working *internet connection* for Terraform to fetch necessary plugins.

### Install Terraform

To install Terraform, visit the official download page:  
[Terraform Downloads](https://www.terraform.io/downloads.html)

Follow the installation instructions for your operating system.

### Install Docker

To install Docker, visit the official Docker installation page:  
[Install Docker](https://docs.docker.com/get-docker/)

Make sure Docker is running before proceeding.

---

## ⚙ Setup Instructions

### 1. Clone the Repository

First, clone the repository to your local machine:

```bash
git clone https://github.com/Bsrikanth008/Local-Docker-container-using-Terraform.git
cd terraform-docker-provisioning

2. Initialize Terraform

Terraform needs to initialize the working directory and download the necessary provider plugins (such as Docker). Run:

terraform init

3. Apply the Configuration

Now, provision the Docker container by applying the Terraform configuration:

terraform apply

You will be prompted to confirm the action. Type yes to continue.

4. Verify the Docker Container

After Terraform has successfully created the container, check that it's running by using the following Docker command:

docker ps

You should see the Nginx container running. You can access the Nginx web server by visiting:

http://localhost:9090


---

🔧 Usage

Start the Container

After provisioning, you can start the Docker container manually:

docker start my-nginx-container

Stop the Container

To stop the Docker container manually:

docker stop my-nginx-container

Access the Container

Once the container is running, you can access it through a browser:

http://localhost:9090


---

🛑 Destroying Resources

To remove the Docker container and clean up all the resources created by Terraform, run the following command:

terraform destroy

You will be prompted to confirm the destruction of the resources. Type yes to proceed.


---

⚠ Troubleshooting

If you encounter issues during provisioning or destruction, try the following:

1. Reinitialize Terraform

Sometimes Terraform requires reinitialization to download or update the provider plugins:

terraform init -reconfigure

2. Check Docker Status

Ensure Docker is running on your machine:

docker info

3. Permissions Issues

If you're on Linux and facing permission issues, run Terraform with sudo:

sudo terraform apply

4. Manual Cleanup

If the container doesn't destroy automatically, remove it manually:

docker stop my-nginx-container
docker rm my-nginx-container


---

🤝 Contributing

Feel free to contribute to this project! Whether it's reporting bugs, suggesting new features, or improving the documentation, contributions are welcome.

How to Contribute:

1. Fork the repository.


2. Clone your fork:

git clone https://github.com/Bsrikanth008/Local-Docker-container-using-Terraform.git


3. Create a new branch for your changes:

git checkout -b feature/your-feature


4. Make your changes and commit:

git commit -m 'Add your feature'


5. Push your changes:

git push origin feature/your-feature


6. Create a pull request to the main repository.




---
📄 License
---

🙏 Acknowledgements

Terraform

Docker

Nginx
