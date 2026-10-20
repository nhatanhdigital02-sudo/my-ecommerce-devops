# 🚀 E-Commerce Microservices DevOps Infrastructure

[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](LICENSE)
[![Terraform](https://img.shields.io/badge/Terraform-1.5+-purple.svg)](https://www.terraform.io/)
[![Kubernetes](https://img.shields.io/badge/Kubernetes-EKS-blue.svg)](https://kubernetes.io/)
[![CI/CD](https://img.shields.io/badge/CI%2ECD-GitHub%20Actions-orange.svg)](https://github.com/features/actions)

## 📌 Project Overview
This repository implements a production-grade, automated DevOps infrastructure for an enterprise-level e-commerce microservices architecture. 

* **Application Base:** The core microservices application layer is referenced from the open-source [OpenTelemetry Demo](https://github.com/open-telemetry/opentelemetry-demo) project.
* **DevOps Focus:** The primary scope of this repository focuses on **Infrastructure as Code (IaC), container orchestration, automated CI/CD pipelines** 

---

## 🏗️ Architecture & Tech Stack

* **Cloud Provider:** AWS (Amazon Web Services)
* **Infrastructure as Code (IaC):** Terraform (Modularized VPC, EKS Cluster, IAM, S3 Remote State Backend)
* **Containerization & Orchestration:** Docker, Kubernetes (EKS), Helm Charts, Kubernetes Manifests
* **CI/CD Automation:** GitHub Actions (Automated build, test, security scanning, and deployment pipelines)

---

## 📂 Repository Structure

```text
├── .github/
│   └── workflows/          # CI/CD pipelines (Build, Push to ECR, Deploy)
├── deploy/                 # Infrastructure and Deployment Manifests
│   ├── terraform/          # AWS VPC, EKS cluster, and node group provisioning
│   └── k8s-manifests/      # Kubernetes deployments, services, and ingress rules
├── src/                    # Microservices source code (Application layer)
├── scripts/                # Automation and helper shell scripts
├── README.md               # Project documentation
└── LICENSE                 # Apache 2.0 License
