# CI/CD Pipeline with Jenkins, SonarQube, and Trivy for Spring Boot Application

## Overview

This repository contains a complete CI/CD pipeline setup using Jenkins for automating builds, SonarQube for code quality analysis, and Trivy for container security scanning.  
The pipeline is designed for a Java Spring Boot application managed with Maven, and containerized using Docker.

---

## Features

- Automated build and test with Jenkins pipeline (`Jenkinsfile`)
- Static code analysis with SonarQube integration
- Security vulnerability scanning of Docker images using Trivy
- Dockerized Spring Boot application for consistent deployment
- Maven for build and dependency management

---

## Prerequisites

- Jenkins installed and configured
- SonarQube server running and accessible
- Docker installed and running
- Trivy installed for image scanning
- Java JDK and Maven installed
- Git installed

---

## Getting Started

### Clone the repository

```bash
git clone https://github.com/DHEVIKA/my-ci-pipeline.git
cd my-ci-pipeline
Jenkins Setup
Create a new pipeline job in Jenkins.

Connect your GitHub repository.

Use the included Jenkinsfile as your pipeline script.

Configure SonarQube plugin and credentials.

Ensure Jenkins nodes have Docker and Trivy installed.

Pipeline Stages
Build: Compile and package the Spring Boot app with Maven.

Test: Run unit tests.

SonarQube Analysis: Scan codebase for quality and bugs.

Docker Build: Build Docker image for the application.

Security Scan: Run Trivy vulnerability scan on Docker image.

(Optional) Deploy: Extend pipeline to deploy images to registry or environment.

