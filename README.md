# 🛒 Cloud-Native E-Commerce Application  
### Built with Node.js, Docker & Kubernetes (Kind)


## 📌 Project Overview

This is a cloud-native E-Commerce web application designed to demonstrate modern containerization and Kubernetes orchestration practices.  

The application is built using **Node.js**, containerized with **Docker**, and deployed on a **Kubernetes cluster (Kind)**.

Unlike traditional applications, this project intentionally avoids SQL or NoSQL databases. Instead, it uses file-based JSON storage to focus purely on microservices communication, containerization, and Kubernetes architecture.


## 🏗 Architecture

Frontend Service  →  Backend API  →  products.json (File Storage)

- The frontend communicates with the backend via Kubernetes Service.
- The backend handles product data and stores it inside a JSON file.
- Each component runs inside its own Docker container.
- Kubernetes manages deployments, scaling, networking, and service discovery.


## 🚀 Tech Stack

- Node.js
- Express.js
- Docker
- Kubernetes (Kind)
- File-based JSON Storage


## 📂 Project Structure

ecommerce-k8s-app/
│
├── backend/
│ ├── server.js
│ ├── products.json
│ ├── package.json
│ └── Dockerfile
│
├── frontend/
│ ├── server.js
│ ├── package.json
│ └── Dockerfile
│
└── k8s/
├── backend-deployment.yaml
├── backend-service.yaml
├── frontend-deployment.yaml
└── frontend-service.yaml
