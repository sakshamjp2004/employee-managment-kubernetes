# Employee Management System - DevOps Deployment

A full-stack Employee Management System deployed using modern DevOps tools and practices.

This project focuses on containerization, orchestration, and cloud deployment rather than application development. The application itself is based on an open-source React + Spring Boot project, while the Docker, Kubernetes, Nginx, and AWS deployment work was implemented as part of my DevOps learning journey.

---

## Tech Stack

- React
- Spring Boot
- MySQL
- Docker
- Docker Compose
- Kubernetes
- Nginx
- AWS EC2

---

## What I Implemented

- Containerized React using a multi-stage Docker build
- Containerized Spring Boot application using multi-stage docker build
- Configured MySQL inside Docker
- Connected all containers using Docker Compose
- Configured Nginx as a reverse proxy
- Deployed the application on AWS EC2
- Migrated the application from Docker Compose to Kubernetes
- Created Kubernetes Deployments
- Created Services for inter-pod communication
- Used ConfigMaps and Secrets for configuration
- Configured Persistent Volumes for MySQL
- Exposed the application using Kubernetes Ingress

---

## Architecture

Docker Compose

Browser
↓
Nginx
↓
React
↓
Spring Boot
↓
MySQL

Kubernetes

Browser
↓
Ingress
↓
Frontend Service
↓
Frontend Pod
↓
Backend Service
↓
Backend Pod
↓
MySQL Service
↓
MySQL Pod

---

## Repository Structure

```
.
├── docker-compose.yml
├── react-hooks-frontend
├── springboot-backend
├── k8s
└── README.md
```

---

## Skills Demonstrated

- Docker
- Docker Compose
- Kubernetes
- Nginx
- AWS EC2
- Linux
- Container Networking
- Persistent Storage
- Reverse Proxy
- Configuration Management

---

## Credits

The application source code is based on the open-source Employee Management System created by Java Guides.

The DevOps implementation, including Docker, Docker Compose, Kubernetes manifests, Nginx configuration, and AWS deployment, was completed as part of my learning and hands-on practice.
