# ☁️ Cloud-Native API Request Monitoring Platform

<div align="center">

![Python](https://img.shields.io/badge/Python-3.11-blue?style=for-the-badge&logo=python)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi)
![AWS](https://img.shields.io/badge/AWS-Cloud-orange?style=for-the-badge&logo=amazonaws)
![REST API](https://img.shields.io/badge/REST-API-success?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-brightgreen?style=for-the-badge)

# Cloud-Native API Request Monitoring Platform

### A Production-Inspired Backend Application for API Traffic Monitoring, Request Analytics, and Rate Limiting using FastAPI & AWS Cloud

Monitor API traffic, enforce request limits, collect usage statistics, and simulate production-ready backend deployment using **FastAPI** and **Amazon Web Services (AWS EC2).**

---

### 🎥 Project Demonstration

📹 Watch the complete project walkthrough.

```text
Demo/
└── API-HIT.mov
```

---

### 📸 Dashboard Preview

| Light Theme | Dark Theme |
|-------------|------------|
| Screenshots/Light Dashboard.png | Screenshots/Dark Dashboard.png |

---

### ☁️ Cloud Deployment

Successfully deployed and tested on **Amazon EC2**.

</div>

---

# 📚 Table of Contents

- Project Overview
- Problem Statement
- Proposed Solution
- Objectives
- Key Features
- Technology Stack
- System Architecture
- Application Workflow
- Project Structure
- Installation
- API Documentation
- AWS Deployment
- Security Features
- Skills Demonstrated
- Future Enhancements
- License

---

# 📖 Project Overview

Cloud applications communicate with clients through REST APIs. As API traffic increases, backend services must efficiently monitor incoming requests, prevent abuse, and maintain consistent performance.

This project demonstrates how a backend application can monitor API requests, apply request rate limiting, and provide real-time request statistics while being deployed on a cloud environment.

The application has been developed using **FastAPI** and deployed on **Amazon EC2**, allowing users to understand both backend API development and cloud deployment fundamentals.

---

# ❗ Problem Statement

In production environments, APIs frequently encounter:

- High request traffic
- Automated bots
- API abuse
- Resource exhaustion
- Server overload
- Performance degradation
- Unauthorized excessive requests

Without monitoring and request limiting mechanisms, APIs become vulnerable to misuse and unstable performance.

---

# 💡 Proposed Solution

The proposed solution is a lightweight API monitoring platform that performs the following operations:

- Tracks every API request.
- Counts incoming requests.
- Enforces configurable request limits.
- Rejects requests beyond the limit.
- Automatically resets counters after a predefined interval.
- Provides live request statistics.
- Supports production-style deployment on AWS.

---

# 🎯 Objectives

The major objectives of this project include:

- Develop REST APIs using FastAPI.
- Understand backend architecture.
- Learn API request monitoring.
- Implement rate limiting.
- Deploy backend applications on AWS.
- Simulate production deployment.
- Improve API security.
- Learn Linux server deployment.

---

# ✨ Key Features

- ✅ API Request Monitoring
- ✅ API Hit Counter
- ✅ Configurable Rate Limiting
- ✅ Automatic Counter Reset
- ✅ REST API
- ✅ JSON Responses
- ✅ FastAPI Backend
- ✅ Cloud Deployment
- ✅ AWS EC2 Hosting
- ✅ Secure Linux Server
- ✅ Lightweight Architecture
- ✅ Production-Oriented Design

---

# 🚀 Why This Project?

Most backend services receive thousands of requests every day.

This project demonstrates one of the most important backend concepts used by companies such as:

- Amazon
- Netflix
- Google
- Microsoft
- Stripe
- OpenAI

where API requests are monitored continuously to improve availability, prevent abuse, and ensure reliable service.

---

# 🛠 Technology Stack

## Backend

- Python 3
- FastAPI
- Uvicorn

## Cloud

- Amazon EC2
- Amazon VPC
- Security Groups
- Ubuntu Linux
- SSH

## API

- REST Architecture
- JSON Response

## Development Tools

- Visual Studio Code
- Git
- GitHub

---

# 🏗 System Architecture

```text
                   Internet
                       │
                       ▼
                Client Request
                       │
                       ▼
              FastAPI Application
                       │
      ┌────────────────┼────────────────┐
      │                │                │
      ▼                ▼                ▼
 API Counter     Rate Limiter    Statistics Engine
      │
      └────────────────┬────────────────┘
                       ▼
               JSON API Response
                       │
                       ▼
                 Client Dashboard
```

---

# 🔄 Application Workflow

```text
Client
   │
   ▼
REST API Request
   │
   ▼
FastAPI Server
   │
   ├── Receive Request
   ├── Count API Hit
   ├── Check Request Limit
   ├── Update Statistics
   ├── Return JSON Response
   └── Auto Reset Counter
          │
          ▼
 Dashboard / API Response
```

---

# 📁 Project Structure

```text
cloud-api-request-monitor/
│
├── main.py
├── README.md
│
├── Demo/
│   └── API-HIT.mov
│
└── Screenshots/
    ├── Light Dashboard.png
    └── Dark Dashboard.png
```

---

# 🚀 Installation Guide

## Clone Repository

```bash
git clone https://github.com/your-username/cloud-api-request-monitor.git
```

---

## Navigate to Project

```bash
cd cloud-api-request-monitor
```

---

## Install Dependencies

```bash
pip install fastapi uvicorn
```

or

```bash
pip install -r requirements.txt
```

---

## Run Application

```bash
uvicorn main:app --reload
```

---

## Open Browser

```text
http://127.0.0.1:8000
```

---

# 📡 API Documentation

## Home Endpoint

```http
GET /
```

Returns the application homepage.

---

## Test Endpoint

```http
GET /api/test
```

Registers an API request and increments the request counter.

### Example Response

```json
{
    "message": "API Request Successful"
}
```

---

## Statistics Endpoint

```http
GET /stats
```

Returns the current API statistics.

### Example Response

```json
{
    "total_requests": 52,
    "remaining_requests": 8,
    "reset_time": 120
}
```

---

## Reset Endpoint

```http
GET /reset
```

Resets the API request counter manually.

---
# ☁️ AWS Cloud Deployment

The application was successfully deployed on **Amazon Web Services (AWS EC2)** to simulate a production-ready backend environment.

Deploying this project on AWS provided practical experience in cloud infrastructure management, Linux server administration, secure remote access, and REST API hosting.

---

# ☁️ AWS Services Used

| AWS Service | Purpose |
|-------------|---------|
| Amazon EC2 | Hosting the FastAPI Application |
| Amazon VPC | Virtual Private Cloud |
| Security Groups | Firewall & Network Access |
| Ubuntu Server | Operating System |
| SSH | Secure Remote Access |
| Uvicorn | ASGI Server |

---

# 🚀 Deployment Process

The project was deployed using the following workflow:

1. Launch an Ubuntu EC2 instance.
2. Configure Security Groups.
3. Connect through SSH.
4. Update the Ubuntu Server.
5. Install Python and dependencies.
6. Clone the project repository.
7. Install required packages.
8. Start FastAPI using Uvicorn.
9. Verify API endpoints.
10. Monitor request statistics.

---

# 🌐 Cloud Deployment Workflow

```text
Developer
     │
     ▼
 GitHub Repository
     │
     ▼
 Amazon EC2
     │
     ▼
 FastAPI Application
     │
     ▼
 REST API Endpoints
     │
     ▼
 API Request Monitoring
     │
     ▼
 JSON Response
```

---

# 🔒 Security Features

This project includes several backend security mechanisms:

- API Request Monitoring
- Request Rate Limiting
- Automatic Counter Reset
- Configurable Request Limits
- REST API Validation
- Linux Server Deployment
- AWS Security Groups
- SSH Authentication
- Production-Oriented Deployment

---

# ⚡ Performance Highlights

- Lightweight FastAPI Framework
- Low Latency API Responses
- Efficient Request Processing
- Cloud Hosted Backend
- Automatic Request Counter Management
- Optimized REST API Architecture

---

# 📊 Skills Demonstrated

## Backend Development

- Python Programming
- FastAPI Framework
- REST API Development
- JSON Data Handling
- Backend Architecture

---

## Cloud Computing

- Amazon EC2
- Amazon VPC
- AWS Security Groups
- Linux Administration
- SSH
- Cloud Deployment

---

## Software Engineering

- API Monitoring
- Rate Limiting
- Production Deployment
- Backend Security
- Version Control
- Git & GitHub

---

# 🌍 Real-World Applications

The concepts implemented in this project are commonly used in:

- Banking Applications
- Payment Gateways
- AI APIs
- Authentication Systems
- Healthcare Platforms
- SaaS Applications
- Cloud Platforms
- Enterprise APIs
- E-Commerce Applications
- Government Services

---

# 📹 Project Demonstration

The repository includes a complete project walkthrough.

```text
Demo/
└── API-HIT.mov
```

### Project Demonstrates

- FastAPI Application
- API Request Monitoring
- Request Counter
- Rate Limiting
- Statistics Endpoint
- AWS Deployment

---

# 📈 API Statistics

The application provides real-time request analytics including:

- Total Requests
- Remaining Requests
- Request Limit
- Reset Timer
- Live Monitoring

---

# 📜 AWS Cloud Deployment Certificate

The successful deployment of this project on Amazon Web Services demonstrates practical cloud deployment skills.

```text
certificate/
└── aws-cloud-deployment-certificate.png
```

Display inside README:

```html
<p align="center">
<img src="certificate/aws-cloud-deployment-certificate.png"
width="900"
alt="AWS Cloud Deployment Certificate">
</p>
```

---

# 🚀 Future Enhancements

The following features can be implemented in future releases:

- JWT Authentication
- OAuth 2.0
- Docker Support
- Kubernetes Deployment
- Redis Rate Limiting
- PostgreSQL Integration
- API Authentication
- User Management
- Request Logging
- Grafana Dashboard
- Prometheus Monitoring
- AWS CloudWatch
- Nginx Reverse Proxy
- HTTPS (SSL)
- Load Balancer
- Auto Scaling
- GitHub Actions CI/CD
- Email Notifications

---

# 📚 Learning Outcomes

This project helped in understanding:

- Backend Development
- REST API Design
- FastAPI Framework
- Cloud Deployment
- Linux Server Management
- AWS Infrastructure
- API Monitoring
- Request Analytics
- Rate Limiting
- Production Deployment

---

# 💼 Resume Highlights

### Project

**Cloud-Native API Request Monitoring Platform**

### Technologies

- Python
- FastAPI
- REST API
- AWS EC2
- Amazon VPC
- Security Groups
- Linux
- Git
- GitHub

### Role

**Backend Developer & Cloud Deployment Engineer**

---

# 🎯 Project Impact

This project demonstrates industry-relevant backend engineering concepts including:

- REST API Development
- Cloud Deployment
- API Monitoring
- Rate Limiting
- Production-Oriented Architecture

It provides a practical understanding of how cloud-hosted backend systems monitor and manage API traffic efficiently.

---

# 👨‍💻 Author

## R. Bharath Rajagopal

**Bachelor of Technology (Information Technology)**

### Technical Skills

- Python
- FastAPI
- Java
- HTML
- CSS
- JavaScript
- SQL
- AWS Cloud
- Linux
- REST APIs
- Git
- GitHub

---

# 🤝 Contributions

Contributions are welcome!

If you'd like to improve this project:

1. Fork the repository.
2. Create a new feature branch.
3. Commit your changes.
4. Submit a Pull Request.

---

# ⭐ Support

If you found this repository useful:

⭐ Star the repository

🍴 Fork the repository

💬 Share your feedback

---

# 📄 License

This project is licensed under the **MIT License**.

Feel free to use, modify, and distribute this project for educational and personal purposes.

---

<div align="center">

# ⭐ Thank You for Visiting ⭐

### If you found this project helpful, please consider giving it a ⭐ on GitHub.

**Made with ❤️ by R. Bharath Rajagopal**

Backend Developer • Cloud Enthusiast • B.Tech Information Technology

🚀 Happy Coding!

</div>
