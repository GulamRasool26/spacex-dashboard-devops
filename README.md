# 🚀 SpaceX Dashboard CI/CD Pipeline

## 📖 Overview

This project is an interactive **SpaceX Launch Records Dashboard** built using **Python Dash**, **Plotly**, and **Pandas**. The dashboard provides insights into SpaceX launch outcomes and payload performance through interactive visualizations.

The application is containerized using Docker and deployed through an automated CI/CD pipeline using GitHub Actions, Docker Hub, and AWS EC2.

---

## ✨ Features

* Interactive launch site selection
* Success vs. failure visualization using pie charts
* Payload range filtering
* Payload vs. launch success correlation analysis
* Interactive dashboard built with Dash and Plotly

---

## 🛠️ Tech Stack

### Application

* Python
* Dash
* Plotly
* Pandas

### DevOps & Cloud

* Docker
* GitHub Actions
* Docker Hub
* AWS EC2
* Linux (Ubuntu)

---

## 🔄 CI/CD Pipeline

```text
Developer Push
      ↓
GitHub Repository
      ↓
GitHub Actions
      ↓
Docker Image Build
      ↓
Docker Hub
      ↓
AWS EC2 Deployment
```

### Continuous Integration (CI)

* Automatically triggers on every push to the `main` branch
* Installs project dependencies
* Builds the Docker image
* Verifies successful image creation

### Continuous Deployment (CD)

* Pushes Docker images to Docker Hub
* Deploys containerized application on AWS EC2

---

## 📁 Project Structure

```text
.
├── .github/
│   └── workflows/
│       └── ci.yml
├── Datasets/
│   └── spacex_launch_dash.csv
├── app.py
├── Dockerfile
├── requirements.txt
└── README.md
```

---

## ▶️ Run Locally

### Clone Repository

```bash
git clone https://github.com/<your-username>/spacex-dashboard-devops.git
cd spacex-dashboard-devops
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Run Application

```bash
python app.py
```

Open:

```text
http://localhost:8050
```

---

## 🐳 Run with Docker

### Build Image

```bash
docker build -t spacex-dashboard .
```

### Run Container

```bash
docker run -d -p 8050:8050 spacex-dashboard
```

Open:

```text
http://localhost:8050
```

---

## ☁️ AWS Deployment

The application is deployed on an AWS EC2 Ubuntu instance using Docker containers.

### Pull Image

```bash
docker pull gulam1159/spacex-dashboard:latest
```

### Run Container

```bash
docker run -d -p 8050:8050 --name spacex-dashboard gulam1159/spacex-dashboard:latest
```

### Access Application

```text
http://<EC2-PUBLIC-IP>:8050
```

---

## 🎯 Skills Demonstrated

* Docker Containerization
* CI/CD Pipeline Automation
* GitHub Actions Workflows
* Docker Hub Image Management
* AWS EC2 Deployment
* Linux Server Administration
* Git & GitHub Version Control
* Cloud Application Deployment

---

## 📌 Project Highlights

* Built and deployed a containerized Python Dash analytics dashboard.
* Implemented CI/CD automation using GitHub Actions.
* Automated Docker image publishing to Docker Hub.
* Deployed application on AWS EC2 using Docker containers.
* Reduced deployment effort through automated build and deployment workflows.

---

## 👨‍💻 Author

**Gulam Rasool**

Aspiring DevOps Engineer | Python • Docker • GitHub Actions • AWS | CI/CD & Cloud Deployment

