# 🚀 Cloud & DevOps Production Engineering Portfolio (AWS)

Welcome to my DevOps & Cloud Engineering repository! 👋  
This repository showcases end-to-end, production-grade DevOps projects focusing on **Infrastructure as Code (IaC)**, **DevSecOps pipelines**, **GitOps**, **Container Orchestration**, and **Full-Stack Observability** built on **Amazon Web Services (AWS)** and **Kubernetes**.

---

## 👨‍💻 About Me

I am a Cloud & DevOps Engineer with hands-on experience designing automated CI/CD pipelines, provisioning multi-environment cloud infrastructure, and deploying scalable containerized workloads.

* 🌐 **LinkedIn:** [linkedin.com/in/archit-gandotra-517831204](https://www.linkedin.com/in/archit-gandotra-517831204)
* 🐙 **GitHub:** [github.com/Archit213](https://github.com/Archit213)
* 📧 **Email:** architgandotra9@gmail.com

---

## 🛠️ Tech Stack & Tooling

| Category | Tools & Technologies |
| :--- | :--- |
| **Cloud Platforms** | Amazon Web Services (EKS, ECR, VPC, S3, DynamoDB, Secrets Manager, KMS, IAM) |
| **Infrastructure as Code** | Terraform, Ansible, Vagrant|
| **Containers & Orchestration** | Docker, Kubernetes (Amazon EKS, Minikube, Helm, kubectl)|
| **CI/CD & GitOps** | GitHub Actions, Jenkins, ArgoCD|
| **DevSecOps & Security** | SonarQube, Trivy, Checkov, GitLeaks, AWS Secrets Manager |
| **Observability & Logging** | Prometheus, Grafana, Alertmanager, Tempo, Loki |
| **Scripting & OS** | Bash, Python, Linux (Ubuntu)|

---

## 📂 Featured Production Projects

### 🔒 1. End-to-End DevSecOps & GitOps Pipeline on AWS (EKS)
> Automated multi-stage CI/CD and GitOps delivery workflow with shift-left security analysis.

* **Tech Stack:** Amazon Elastic Kubernetes Service (EKS), GitHub Actions, SonarQube, Trivy, Checkov, GitLeaks, Amazon Elastic Container Registry (ECR), ArgoCD, Prometheus & Grafana.
* **Key Highlights:**
  * Automated secret detection using **GitLeaks** and IaC misconfiguration scanning with **Checkov**.
  * Integrated **SonarQube** for code quality gates and **Trivy** for vulnerability scanning of container images prior to pushing to **Amazon ECR**.
  * Configured GitOps continuous delivery via **ArgoCD** ensuring automated synchronization, blue/green or canary updates, and rapid rollbacks on **Amazon EKS**.
  * Deployed full-stack monitoring using **Prometheus & Grafana** to track node/pod resource saturation, ingress latency, and cluster health in real time.
* **Folder:** `/projects/devsecops-eks-pipeline`

---

### 🏗️ 2. Modular Multi-Environment Infrastructure as Code (Terraform & AWS)
> Production-ready, modular cloud infrastructure automation on Amazon Web Services (AWS).

* **Tech Stack:** Terraform, AWS (VPC, Subnets, Security Groups, IAM, NAT Gateways, EKS, RDS), Amazon S3 (Remote Backend), AWS DynamoDB (State Locking), AWS Secrets Manager / KMS.
* **Key Highlights:**
  * Created reusable Terraform child modules for custom VPCs, Public/Private Subnets, Security Groups, IAM Roles, and **Amazon EKS** clusters.
  * Configured secure remote state management with server-side encryption on **Amazon S3** and distributed state locking using **DynamoDB**.
  * Implemented dynamic secret injection directly via **AWS Secrets Manager** and **KMS** to avoid hardcoding sensitive credentials in `.tf` files.
  * Separated isolated environments (`dev`, `staging`, `prod`) using parameterized `.tfvars` and Terraform workspaces.
* **Folder:** `/projects/terraform-aws-architecture`

---

### ⚡ 3. Microservices Matrix CI/CD & Dynamic Build Optimization
> Monorepo microservices continuous integration pipeline with path-based matrix triggers.

* **Tech Stack:** GitHub Actions Matrix, Docker, Kubernetes (EKS), Amazon Elastic Container Registry (ECR), Trivy.
* **Key Highlights:**
  * Implemented **GitHub Actions Matrix Builds** with folder-level path filtering to selectively trigger builds and tests only for modified microservices.
  * Reduced CI build execution times and GitHub runner compute costs by up to 60%.
  * Automated container image builds, **Trivy** vulnerability scans, version tagging, and dynamic pushing to dedicated **Amazon ECR** repositories.
  * Automated Kubernetes manifest updates with new image tags for continuous synchronization to the **EKS** cluster.
* **Folder:** `/projects/microservices-matrix-ci-aws`

---

### 🖥️ 4. Automated Multi-Node DevOps Lab Environment
> Multi-VM infrastructure simulation for configuration management and cluster testing.

* **Tech Stack:** Vagrant, VirtualBox, Ansible, Docker, Kubernetes, Linux (Ubuntu).[cite: 1]
* **Key Highlights:**
  * Automated VM provisioning using **Vagrant** to create isolated multi-node controller and worker environments.[cite: 1]
  * Configured target nodes using modular **Ansible playbooks** for Docker, kubectl, and cluster dependencies.[cite: 1]
  * Verified application high-availability, replica scaling, and NodePort routing under simulated network topologies.[cite: 1]
* **Folder:** `/projects/automated-devops-lab`

---
