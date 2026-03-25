# 🚀 DataStore Multi-Tier Application (Dockerized)

## 📌 Overview
This project demonstrates a containerized multi-tier architecture using Docker and Docker Compose. The application consists of a frontend (Streamlit), backend (Spring Boot), and MySQL database.

## 🏗️ Architecture
Browser → Frontend → Backend → MySQL

## ⚙️ Tech Stack
- Docker & Docker Compose
- Python (Streamlit)
- Java Spring Boot (JAR)
- MySQL

## 🚀 How to Run

```bash
docker-compose up --build

Access:

Frontend: http://localhost:8080
Backend: http://localhost:8081
🔗 Service Communication
Frontend → http://backend:8081
Backend → mysql://mydb:3306
📦 Features
Multi-container architecture
Service-to-service communication
Environment-based configuration
Database integration
🔮 Future Enhancements
CI/CD with Jenkins
Deployment on AWS EC2
Kubernetes (EKS)