🚀 DevOps CI/CD Project – Brain Tasks App (EKS Deployment)

📌 Project Overview

This project demonstrates a complete CI/CD pipeline for deploying a React-based static application using:

- GitHub (Source Control)

- AWS CodeBuild (CI - Build stage)

- Amazon ECR (Docker Image Registry)

- Amazon EKS (Kubernetes Cluster)

- AWS LoadBalancer (Application Exposure)

The application is containerized using Docker and deployed on Kubernetes running on AWS EKS.

**Architecture Flow**

GitHub

   ↓
   
AWS CodeBuild

   ↓
   
Docker Image Build

   ↓
   
Amazon ECR (Image Storage)

   ↓
   
Amazon EKS (Kubernetes Deployment)

   ↓
   
AWS LoadBalancer (Public Access)


---

## 📌 1. Source Code Management (GitHub)

- Created a GitHub repository for version control
- Cloned the repository to EC2 workstation
- Managed application files using Git
- Pushed final codebase to GitHub

---

## 📌 2. Application Build (Static React App)

- The application is already pre-built inside `dist/` folder
- Contains:
  - HTML
  - CSS
  - JavaScript
  - Assets

---

## 📌 3. Docker Containerization

- Created Dockerfile using **Nginx base image**
- Copied `dist/` files into Nginx web directory
- Exposed application on port 80

---

## 📌 4. Amazon ECR (Docker Image Registry)

- Created ECR repository in AWS
- Tagged Docker image
- Pushed image to ECR

---

## 📌 5. AWS CodeBuild (CI Automation)

- Connected GitHub repository to AWS CodeBuild
- Used buildspec.yml for automation
- CodeBuild performs:
- Source download from GitHub
- Docker image build
- Push image to Amazon ECR

---

## 📌 6. Amazon EKS (Kubernetes Cluster)

- Created EKS cluster using eksctl
- Configured kubectl access from EC2
- Verified worker nodes are active

---

## 📌 7. Kubernetes Deployment

- Created Kubernetes manifests:
- deployment.yaml
- service.yaml

---

## 📌 8. Application Exposure (LoadBalancer)
- Service type: LoadBalancer
- AWS automatically creates public endpoint
- Application accessible via external URL
- http://<LoadBalancer-DNS>

---

## 📌 9. CI/CD Pipeline Flow

GitHub → AWS CodeBuild → Amazon ECR → Amazon EKS → LoadBalancer → Browser

---

<img width="1117" height="737" alt="d1" src="https://github.com/user-attachments/assets/cfa78fd8-e501-40c1-bff8-453d51d4ca3b" />

<img width="1882" height="857" alt="d2" src="https://github.com/user-attachments/assets/330ef59b-8405-4ce1-af75-97e6d0a1776e" />

<img width="1917" height="785" alt="d3" src="https://github.com/user-attachments/assets/0fa6dff0-2e65-4b95-9ed9-6ed63e47dae5" />

<img width="1902" height="887" alt="d4" src="https://github.com/user-attachments/assets/66b88f90-3835-418a-b604-664fbc2ecb0b" />

<img width="1890" height="691" alt="d5" src="https://github.com/user-attachments/assets/f77643ce-a75e-4d41-9ace-34340ac71bc6" />

<img width="1102" height="677" alt="d6" src="https://github.com/user-attachments/assets/f58f5040-6f2b-40fa-9d3e-a3b9e4060520" />

<img width="1895" height="862" alt="d7" src="https://github.com/user-attachments/assets/4939ee08-0d72-48a1-a31d-180a8edf4b02" />

<img width="736" height="472" alt="d8" src="https://github.com/user-attachments/assets/436df79c-655e-4fcf-936f-57c9279b079b" />

<img width="1880" height="932" alt="d9" src="https://github.com/user-attachments/assets/88a6dbc0-684d-4c2d-9ac9-f54b2175ade1" />

<img width="1857" height="592" alt="d10" src="https://github.com/user-attachments/assets/dca1d422-0167-4230-af54-9e1bdcc0748e" />

<img width="1866" height="890" alt="d11" src="https://github.com/user-attachments/assets/8bc847ab-a32c-4e58-ae43-2be7953c7627" />

<img width="1170" height="682" alt="d12" src="https://github.com/user-attachments/assets/794691b6-92bd-42d3-83c0-202f4e7320bc" />

<img width="1902" height="516" alt="d13" src="https://github.com/user-attachments/assets/5cfdddc2-ea03-4f97-9d86-c023659a32bd" />

<img width="1867" height="657" alt="d14" src="https://github.com/user-attachments/assets/d70a5a9b-8129-40a6-842f-959b03603a9c" />

<img width="1912" height="605" alt="d15" src="https://github.com/user-attachments/assets/f7c70781-34c2-4130-a322-b4f6ec3139fb" />

<img width="1867" height="860" alt="d16" src="https://github.com/user-attachments/assets/33e9374a-851c-48ea-8f50-3fb16ff1a94f" />

<img width="1546" height="650" alt="d17" src="https://github.com/user-attachments/assets/223d7f06-cecd-4aae-898b-16b0940a4b4b" />

<img width="1907" height="532" alt="d18" src="https://github.com/user-attachments/assets/3b71fa2f-18b1-4344-b305-71066835722b" />

<img width="1847" height="651" alt="d19" src="https://github.com/user-attachments/assets/4033e0ff-8cab-4221-898d-8d07aebc60b3" />

<img width="1887" height="836" alt="d20" src="https://github.com/user-attachments/assets/c9cef3b4-128c-4787-96ab-bd9fdd86490e" />

<img width="1620" height="791" alt="d21" src="https://github.com/user-attachments/assets/54b31c80-8b17-49f4-ab2c-6e628bc09956" />

<img width="1907" height="787" alt="d22" src="https://github.com/user-attachments/assets/078cabb2-1ebc-4323-8c40-df9c25aed73d" />

<img width="1887" height="757" alt="d23" src="https://github.com/user-attachments/assets/64d0eb80-8a64-42cd-8b1c-07a1593da462" />

<img width="1877" height="607" alt="d24" src="https://github.com/user-attachments/assets/f0ea742d-2c3e-49d6-8351-8af82de93b4f" />

<img width="1901" height="820" alt="d25" src="https://github.com/user-attachments/assets/c4056077-5beb-4baa-9006-a5bffbe45f60" />

<img width="1822" height="932" alt="d26" src="https://github.com/user-attachments/assets/815537dc-ade0-40f1-a282-847c6ea8836b" />
