# 🚀 Cloud & DevOps Production Engineering Portfolio

Welcome to my DevOps & Cloud Engineering repository! 👋  
This repository showcases end-to-end, production-grade DevOps projects focusing on **Infrastructure as Code (IaC)**, **DevSecOps pipelines**, **GitOps**, **Container Orchestration**, and **Full-Stack Observability** primarily built on **Microsoft Azure** and **Kubernetes**.

---

## 👨‍💻 About Me

I am a Cloud & DevOps Engineer certified in **Microsoft Azure (AZ-104 & AZ-900)** with hands-on experience designing automated CI/CD pipelines, provisioning multi-environment cloud infrastructure, and deploying scalable containerized workloads.

* 🌐 **LinkedIn:** [linkedin.com/in/archit-gandotra-517831204](https://www.linkedin.com/in/archit-gandotra-517831204.
* 🐙 **GitHub:** [github.com/Archit213](https://github.com/Archit213.
* 📧 **Email:** architgandotra9@gmail.com.

---

## 🛠️ Tech Stack & Tooling

| Category | Tools & Technologies |
| :--- | :--- |
| **Cloud Platforms** | Microsoft Azure (AKS, ACR, Key Vault, Virtual Networks, Blob Storage, NSGs)[cite: 1] |
| **Infrastructure as Code** | Terraform, Ansible, Vagrant|
| **Containers & Orchestration** | Docker, Kubernetes (AKS, Minikube, Helm)|
| **CI/CD & GitOps** | GitHub Actions, Jenkins, ArgoCD|
| **DevSecOps & Security** | SonarQube, Trivy, Checkov, GitLeaks, Azure Key Vault |
| **Observability & Logging** | Prometheus, Grafana, Alertmanager, Tempo, Loki |
| **Scripting & OS** | Bash, Python, Linux (Ubuntu)|

---

## 📂 Featured Production Projects

### 🔒 1. End-to-End DevSecOps & GitOps Pipeline on Azure (AKS)
> Automated multi-stage CI/CD and GitOps delivery workflow with shift-left security analysis.

* **Tech Stack:** Azure Kubernetes Service (AKS), GitHub Actions, SonarQube, Trivy, Checkov, GitLeaks, ACR, ArgoCD, Prometheus & Grafana.
* **Key Highlights:**
  * Automated secret detection using **GitLeaks** and IaC misconfiguration scanning with **Checkov**.
  * Integrated **SonarQube** for code quality gates and **Trivy** for vulnerability scanning of container images prior to registry push.
  * Configured GitOps deployment via **ArgoCD** ensuring automated synchronization, canary/rolling updates, and quick rollbacks.
  * Deployed full-stack monitoring using **Prometheus & Grafana** to track pod resource saturation and ingress latency.
* **Folder:** `/projects/devsecops-aks-pipeline`

---

### 🏗️ 2. Modular Multi-Environment Infrastructure as Code (Terraform)
> Production-ready, modular cloud infrastructure automation on Microsoft Azure.

* **Tech Stack:** Terraform, Microsoft Azure, Azure Blob Storage (Remote Backend), Azure Key Vault.
* **Key Highlights:**
  * Created reusable child modules for Virtual Networks, Subnets, NSGs, and AKS clusters.
  * Configured secure remote state locking using Azure Blob Storage and state encryption.
  * Implemented dynamic secret injection directly via **Azure Key Vault** to avoid hardcoded credentials in `.tf` files.
  * Separated environments (`dev`, `staging`, `prod`) using parameterized `.tfvars` workspaces.
* **Folder:** `/projects/terraform-azure-architecture`

---

### ⚡ 3. Microservices Matrix CI/CD & Dynamic Build Optimization
> Monorepo microservices continuous integration pipeline with path-based matrix triggers.

* **Tech Stack:** GitHub Actions Matrix, Docker, Kubernetes, Azure Container Registry (ACR).
* **Key Highlights:**
  * Implemented **GitHub Actions Matrix Builds** with folder-level path filtering to selectively trigger builds only for modified microservices.
  * Reduced CI build execution times and runner compute costs by up to 60%.
  * Automated Docker image tagging, vulnerability scans, and deployment manifest updates.
* **Folder:** `/projects/microservices-matrix-ci`

---

### 🖥️ 4. Automated Multi-Node DevOps Lab Environment
> Multi-VM infrastructure simulation for configuration management and cluster testing.

* **Tech Stack:** Vagrant, VirtualBox, Ansible, Docker, Kubernetes, Linux (Ubuntu).
* **Key Highlights:**
  * Automated VM provisioning using **Vagrant** to create isolated multi-node controller and worker environments.
  * Configured target nodes using modular **Ansible playbooks** for Docker, kubectl, and cluster dependencies.
  * Verified application high-availability, replica scaling, and NodePort routing under simulated network topologies.
* **Folder:** `/projects/automated-devops-lab`

---
