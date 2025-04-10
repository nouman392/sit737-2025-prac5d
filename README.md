Calculator Microservice – Dockerized Deployment  
**SIT737-2025-Prac5P | Cloud-Native Application Development**

## 📘 Overview

This project demonstrates how to Dockerize a Node.js-based calculator microservice using Docker and Docker Compose. It includes advanced arithmetic operations and implements container health checks to ensure service reliability.

---

## Tech Stack

- **Node.js + Express** – RESTful microservice
- **Docker** – Containerization platform
- **Docker Compose** – Multi-container orchestration
- **Winston** – Logging library (already integrated)

---

## Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/sit737-2025-prac4c.git
cd sit737-2025-prac5P
2. Build Docker Image
docker build -t calculator-microservice .
3. Start Docker Compose
docker-compose up --build

Project Structure
sit737-2025-prac5P/
│
├── server.js
├── package.json
├── Dockerfile
├── docker-compose.yml
├── logs/
└── README.md

Push to Docker Hub
docker tag calculator-microservice your-dockerhub-username/calculator-microservice
docker push your-dockerhub-username/calculator-microservice
```
