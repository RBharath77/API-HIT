# ☁️ Cloud-Based API Request Monitoring & Rate Limiting System

![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?logo=fastapi)
![AWS](https://img.shields.io/badge/AWS-Cloud-orange?logo=amazonaws)
![REST API](https://img.shields.io/badge/REST-API-success)
![License](https://img.shields.io/badge/License-MIT-green)

A cloud-based backend application developed using **FastAPI** to monitor API requests, enforce rate limiting, and provide real-time API usage statistics. The project was successfully deployed on **Amazon Web Services (AWS EC2)** to simulate a production-ready environment.

---

# 📌 Overview

Modern applications expose REST APIs that must be protected from excessive traffic and abuse. This project demonstrates how API request monitoring and rate limiting can be implemented using FastAPI and deployed securely on AWS.

The application records every incoming request, validates it against configurable rate limits, automatically resets request counters after a defined interval, and provides real-time monitoring through REST endpoints.

---

# 🎯 Objectives

- Develop REST APIs using FastAPI
- Monitor API request traffic
- Implement request rate limiting
- Deploy applications on AWS EC2
- Understand cloud infrastructure basics
- Simulate production deployment

---

# ✨ Key Features

- API Request Monitoring
- Rate Limiting Mechanism
- Automatic Counter Reset
- Real-Time Statistics
- RESTful API Design
- FastAPI Backend
- AWS EC2 Deployment
- Lightweight Architecture
- Secure Cloud Hosting

---

# 🛠 Technology Stack

## Backend

- Python
- FastAPI
- Uvicorn

## Cloud

- Amazon EC2
- Amazon VPC
- Security Groups
- SSH

---

# ☁️ Cloud Deployment

The application is deployed on **Amazon Web Services (AWS)** to simulate a real-world backend deployment.

### AWS Services Used

- Amazon EC2
- Amazon VPC
- Security Groups
- Ubuntu Server
- SSH
- Uvicorn

---

# 🏗 System Architecture

```
               Client
                  │
                  ▼
           REST API Request
                  │
                  ▼
          FastAPI Application
                  │
        ┌─────────┴─────────┐
        │                   │
        ▼                   ▼
 Request Counter      Rate Limiter
        │                   │
        └─────────┬─────────┘
                  ▼
          API Statistics
                  │
                  ▼
            JSON Response
```

---

# 🔄 Application Workflow

1. Client sends an API request.
2. FastAPI receives the request.
3. API hit counter is incremented.
4. Rate limit is verified.
5. Request is accepted or rejected.
6. Statistics are updated.
7. Counter resets automatically after the configured time window.

---

# 📁 Project Structure

```
cloud-api-request-monitor/
│
├── main.py
├── README.md
└── certificate/
    └── aws-cloud-deployment-certificate.pdf
```

---

# 📡 API Endpoints

## Home

```
GET /
```

Returns the application homepage or status.

---

## Test Endpoint

```
GET /api/test
```

Registers an API request and returns a success response.

---

## Statistics

```
GET /stats
```

Returns the current API usage statistics.

Example Response

```json
{
  "total_requests": 45,
  "remaining_requests": 5,
  "reset_time": 120
}
```

---

## Reset

```
GET /reset
```

Resets the API request counter.

---

# 🚀 Installation

Clone the repository

```bash
git clone https://github.com/your-username/cloud-api-request-monitor.git
```

Navigate into the project

```bash
cd cloud-api-request-monitor
```

Install dependencies

```bash
pip install fastapi uvicorn
```

Run the server

```bash
uvicorn main:app --reload
```

Visit

```
http://127.0.0.1:8000
```

---

# 🔒 Security Features

- Request Rate Limiting
- Secure AWS Security Groups
- SSH Authentication
- Controlled API Access
- Production-Oriented Deployment

---

# ☁️ AWS Deployment

The application was deployed on **Amazon EC2** using Ubuntu Linux.

Deployment steps included:

- Launching an EC2 instance
- Configuring Security Groups
- Connecting through SSH
- Installing Python and dependencies
- Running the FastAPI application using Uvicorn
- Accessing the application through the EC2 Public IP

---

# 💼 Skills Demonstrated

- Backend Development
- REST API Development
- FastAPI Framework
- Python Programming
- Cloud Deployment
- AWS EC2
- Linux Server Administration
- Networking Basics
- API Security
- Rate Limiting

---

# 🌍 Real-World Applications

- Banking APIs
- Payment Gateways
- Authentication Services
- AI APIs
- Cloud Services
- SaaS Platforms
- Enterprise Backend Systems

---

# 📜 AWS Deployment Certificate

The application deployment was completed as part of my cloud computing learning journey.

```
certificate/
└── aws-cloud-deployment-certificate.pdf
```

> 📌 The AWS deployment certificate is included in this repository as proof of successful cloud deployment.

---

# 🚀 Future Enhancements

- JWT Authentication
- Docker Containerization
- Redis Rate Limiting
- PostgreSQL Integration
- Nginx Reverse Proxy
- HTTPS Support
- GitHub Actions CI/CD
- Prometheus Monitoring
- Grafana Dashboard
- Kubernetes Deployment

---

**B.Tech Information Technology**

### Technical Skills

- Python
- FastAPI
- AWS Cloud
- REST APIs
- Java
- HTML
- CSS
- JavaScript
- SQL

---

# 📄 License

This project is licensed under the MIT License.

---

## ⭐ If you found this project helpful, don't forget to Star this repository!
