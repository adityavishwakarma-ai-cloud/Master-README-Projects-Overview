## 📂 Complete Portfolio Folder Structure

```
aditya-portfolio/
│-- README.md                       # Master README (with all projects + flows)
│
├── project-1-hms/
│   ├── README.md
│   ├── src/                        # Java Spring Boot project source
│   └── pom.xml / build.gradle
│
├── project-2-task/
│   ├── README.md
│   ├── src/                        # Angular frontend source
│   └── package.json
│
├── project-3-leaves/
│   ├── README.md
│   ├── src/                        # Angular frontend + backend (Node.js)
│   └── package.json
│
├── project-4-lambda/
│   ├── README.md
│   ├── lambda/
│   └── s3-event-handler.js
│
├── project-5-angular-forms/
│   ├── README.md
│   ├── src/                        # Angular Reactive Forms code
│   └── package.json
│
├── project-6-dashboard/
│   ├── README.md
│   ├── src/                        # Angular frontend + chart logic
│   └── package.json
│
├── project-7-ems/
│   ├── README.md
│   ├── src/                        # React frontend + Node.js backend
│   └── package.json
│
├── project-8-k8s-jenkins/
│   ├── README.md
│   ├── Jenkinsfile
│   ├── k8s/
│   ├── Dockerfile
│   └── src/
│
├── project-9-serverless-chatbot/
│   ├── README.md
│   ├── lambda/
│   ├── lex/
│   ├── dynamodb/
│   └── package.json
│
└── mega-project-smart-cloud-platform/
    ├── README.md
    ├── frontend/
    ├── backend/
    ├── chatbot/
    ├── terraform/
    ├── k8s/
    └── ci-cd/
```

---

## ✅ Key Notes for GitHub Push

1. **Master README** at root (`vikram-portfolio/README.md`) linking all projects.
2. Each project has its **own README** describing:

   * Overview
   * Tech stack
   * Folder structure
   * Flow diagram (ASCII text if needed)
   * Deployment instructions
3. `.gitignore` for each project (Node, Angular, Java, Terraform, etc.) to avoid unnecessary files.
4. For **Mega Project** and **Project 8/9**, include sample Lambda, Terraform, Kubernetes, and CI/CD files.
5. Use **consistent naming** across Docker images, GitHub repos, and AWS resources.
6. Include **package.json** or **pom.xml/build.gradle** files for reproducibility.

---

## 📌 Deployment Guide (High-Level)

1. **Clone the repository**:

```bash
git clone https://github.com/<your-username>/vikram-portfolio.git
cd vikram-portfolio
```

2. **Follow each project’s README** to run it locally or deploy to AWS/Kubernetes.

3. **Mega Project Deployment**:

```bash
cd mega-project-smart-cloud-platform/terraform
terraform init
terraform apply

# Docker build & push
cd ../frontend
docker build -t frontend .
docker push <dockerhub>/frontend

cd ../backend
docker build -t backend .
docker push <dockerhub>/backend

# Kubernetes deployment
kubectl apply -f ../k8s/
```

<!---

Once this **ZIP structure** is ready, you can directly **push it to GitHub**, and your portfolio will be:

* **Professional** ✅
* **Complete with 10 deployable projects** ✅
* **Easy for recruiters or collaborators to explore** ✅

--->
