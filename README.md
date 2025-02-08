# E-MART E-Commerce Application

A full-stack e-commerce application built with microservices architecture using Angular, Node.js, Java Spring Boot, and deployed on Kubernetes using Helm.

## Architecture Overview

### Frontend
- Angular 12.2.0
- Bootstrap for styling
- Font Awesome icons
- Running on port 4200

### Backend Services
1. **Node.js API (Main Service)**
   - Express.js framework
   - MongoDB integration
   - JWT authentication
   - Running on port 8000

2. **Java API (Books Service)**
   - Spring Boot 2.3.1
   - MySQL database
   - Running on port 9000

### Databases
- MongoDB 4.0 (port 27017)
- MySQL 8.0.33 (port 3306)

## Prerequisites

- Node.js 14.x
- Java JDK 8
- Docker
- Kubernetes cluster
- Helm 3.x
- Maven
- Angular CLI

## Local Development Setup

1. **Clone the repository**
```bash
git clone https://github.com/mohammadshaad/emartapp.git
cd emartapp
```

2. **Docker Setup**

```bash
docker compose up -d
```


## Project Structure

```bash
e-mart/
├── client/ # Angular frontend
├── nodeapi/ # Node.js main service
├── javaapi/ # Java Spring Boot books service
├── kkartchart/ # Helm charts
├── nginx/ # Nginx configurations
└── docker-compose.yaml
```

## Features

- User authentication and authorization
- Product catalog
- Shopping cart functionality
- Order management
- Book management
- Responsive design
- Microservices architecture
- Containerized deployment
- Persistent storage
- Load balancing
- SSL/TLS support

## CI/CD Pipeline

The project uses Jenkins for continuous integration and deployment:
- Automated builds for all services
- Docker image creation and pushing
- Helm chart deployment
- Environment-specific configurations

## Configuration

Environment configurations can be modified in:
- `client/src/environments/`
- `nodeapi/config/`
- `javaapi/src/main/resources/`
- `kkartchart/values.yaml`
