# 🐳 DPDZero Assignment – NGINX Reverse Proxy with Docker Compose

## 🚀 Overview

This project sets up a reverse proxy system using Docker Compose with:
- Go service (`service1`)
- Python Flask service (`service2`)
- NGINX for reverse proxying routes

## 🧱 Project Structure

.
├── docker-compose.yml
├── nginx/
│ ├── Dockerfile
│ └── nginx.conf
├── service_1/
│ ├── main.go
│ └── Dockerfile
├── service_2/
│ ├── app.py
│ └── Dockerfile
└── README.md

bash
Copy
Edit

## 🔧 Setup Instructions

1. Clone the repo:
   ```bash
   git clone https://github.com/YOUR_USERNAME/dpdzero-Assignment.git
   cd dpdzero-Assignment
Start the services:

bash
Copy
Edit
docker-compose up --build
Access services in browser:

Go Service: http://localhost:8080/service1/ping

Python Service: http://localhost:8080/service2/ping

✅ Features
NGINX reverse proxy for both services

Path-based routing

NGINX access logging with timestamp & path

Works with one command: docker-compose up --build
