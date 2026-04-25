## Applicaton screen shot live running

<img width="1920" height="1080" alt="Screenshot (274)" src="https://github.com/user-attachments/assets/ef2d2845-9749-487f-a8bc-a27ae01abaa5" />




# 🚀 DevOps CI/CD Pipeline Project (Node.js + Docker + Jenkins + AWS EC2)

## 📌 Project Overview
This project demonstrates a real-world DevOps CI/CD pipeline that automates building, testing, and deploying a Node.js application using Docker and Jenkins on an AWS EC2 instance.

The goal of this project is to understand how modern applications are deployed in production environments using automation tools.

---

## 🏗️ Architecture Flow

Developer → GitHub → Jenkins → Docker → EC2 → Browser

---

## ⚙️ Technologies Used

- Node.js
- Docker
- Docker Compose
- Jenkins
- Git & GitHub
- AWS EC2
- Linux (Ubuntu)

---

## 🔁 CI/CD Workflow

1. Developer writes code and pushes it to GitHub
2. Jenkins detects changes using GitHub Webhook
3. Jenkins pulls latest code automatically
4. Docker builds the application image
5. Docker container runs the application
6. Application is deployed on AWS EC2
7. App is accessible in browser

---

## 🐳 Docker Setup

### Build Image
docker build -t my-app .

### Run Container
docker run -d -p 5000:3000 my-app

---

## 📦 Docker Compose

services:
  app:
    build: .
    ports:
      - "5000:3000"
    env_file:
      - .env

---

## 🌐 Application Access

http://<EC2-IP>:5000

---

## 📁 Project Structure

Rebuild/
│
├── app/
│   └── server.js
├── Dockerfile
├── docker-compose.yml
├── .env
└── README.md

---

## 🔥 Key DevOps Skills Learned

- CI/CD automation using Jenkins
- Docker containerization
- Port mapping (Host → Container)
- GitHub webhook integration
- AWS EC2 deployment
- Debugging deployment issues

---

## 🧠 What This Project Shows

This project simulates real-world DevOps workflow used in companies:

- Fast deployment
- Automation
- Scalability
- Reduced manual work

---

## 👨‍💻 Author

DevOps Learner (Chaitanya)  
Focused on CI/CD, Docker, Jenkins, AWS

---

## 🚀 Future Improvements

- Kubernetes deployment
- Nginx reverse proxy
- Monitoring (Prometheus + Grafana)
