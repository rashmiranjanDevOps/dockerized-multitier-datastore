# 🚀 Dockerized Multi-Tier DataStore Application

## 📌 Overview

This project demonstrates an **end-to-end containerized multi-tier architecture** using Docker and Docker Compose. It simulates a real-world application with a frontend, backend, and database communicating over a custom Docker network.

---

## 🏗️ Architecture

```
Browser → Frontend (Streamlit) → Backend (Spring Boot) → MySQL
```

* **Frontend** handles user interaction
* **Backend** exposes REST APIs
* **Database** persists application data

---

## ⚙️ Tech Stack

* 🐳 Docker & Docker Compose
* 🐍 Python (Streamlit)
* ☕ Java Spring Boot (JAR)
* 🐬 MySQL
* 🔗 REST API Communication

---

## 📂 Project Structure

```
datastore-project/
│
├── frontend/
│   ├── app.py
│   ├── requirements.txt
│   └── Dockerfile
│
├── backend/
│   ├── Dockerfile
│   └── (place your app.jar here)
│
├── docker-compose.yml
├── .env
└── README.md
```

---

## 🚀 Getting Started

### 🔹 Prerequisites

* Docker installed and running
* Docker Compose installed

---

### 🔹 Run the Application

```bash
docker-compose up --build
```

---

## 🌐 Access the Application

* Frontend → http://localhost:8080
* Backend → http://localhost:8081

---

## 🔗 Service Communication

| Service            | Endpoint               |
| ------------------ | ---------------------- |
| Frontend → Backend | http://backend:8081    |
| Backend → MySQL    | jdbc:mysql://mydb:3306 |

---

## ⚠️ Important Note

The backend JAR file is **not included** in this repository due to size limitations.

👉 Please place your JAR file inside the `backend/` directory before running:

```
backend/app.jar
```

---

## 📦 Key Features

* Multi-container architecture using Docker Compose
* Service-to-service communication via Docker networking
* Environment variable-based configuration
* Database integration with MySQL
* Scalable and modular design

---

## 🔒 Best Practices Followed

* Separation of concerns (frontend, backend, database)
* Lightweight Docker images
* Environment-based configuration
* Ignoring unnecessary files using `.gitignore`
* Standardized artifact naming (`app.jar`)

---

## 🔮 Future Enhancements

* 🔁 CI/CD pipeline using Jenkins
* ☁️ Deployment on AWS EC2
* ☸️ Kubernetes (EKS) deployment
* 📊 Monitoring with Prometheus & Grafana

---

## 🧠 Learnings

* Docker containerization & networking
* Multi-tier application architecture
* Service orchestration using Docker Compose
* Backend-frontend integration
* Database connectivity in containerized environments

---

## 👨‍💻 Author

**Rashmi Ranjan Panigrahy**
Aspiring DevOps Engineer | AWS & Cloud Enthusiast 🚀

---
