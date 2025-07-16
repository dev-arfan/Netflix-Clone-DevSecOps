# 📺 Netflix Clone - Kubernetes CI/CD Deployment

This project demonstrates an end-to-end CI/CD pipeline to deploy a **Netflix Clone** web application to a Kubernetes cluster on **AWS EKS**. It integrates containerization, security scanning, GitOps deployment, and monitoring using modern DevOps tools.

---

## 🛠️ Tools & Technologies Used

| Category             | Tools/Technologies                             |
|----------------------|------------------------------------------------|
| Containerization     | Docker                                         |
| CI/CD Pipeline       | Jenkins                                        |
| Security Scanning    | SonarQube, Trivy, OWASP Dependency Check       |
| GitOps Deployment    | ArgoCD                                         |
| Container Orchestration | Kubernetes (K8s), AWS EKS                   |
| Monitoring           | Prometheus, Grafana                            |

---

## ☁️ AWS Infrastructure

- **2 EC2 Instances**  
- **EKS Cluster**
- **2 Elastic IPs**

---

## 🧪 CI/CD Pipeline Workflow

1. **Code Commit**  
   Developers push code to GitHub.

2. **CI Pipeline with Jenkins**  
   - Triggers on code push  
   - Runs security scans with **SonarQube**, **Trivy**, and **OWASP**  
   - Builds Docker image  
   - Pushes image to **Docker Hub**

3. **CD Pipeline with ArgoCD**  
   - Monitors GitHub for Kubernetes manifests  
   - Syncs and deploys application to AWS EKS cluster

4. **Monitoring Setup**  
   - **Prometheus** collects metrics from the application and node exporters  
   - **Grafana** visualizes performance data and system health

---

## ✅ SOP 

Before any deployment, follow this **Standard Operating Procedure (SOP):**
https://docs.google.com/document/d/1-_MNHSLYDYHmUuGGzAsAJobaXW6x7dR2Sf3NxjgxdpA/edit?tab=t.0
---

## 🎥 Video Walkthrough

Watch the complete walkthrough on YouTube:  
📺 [Netflix Clone CI/CD Kubernetes Deployment - Video Guide](https://drive.google.com/file/d/1MvHa97XA1ytzPhfEzEQz3Pn6iL-5zc9_/view?usp=sharing)
---
