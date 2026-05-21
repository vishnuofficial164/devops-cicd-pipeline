# End-to-End CI/CD Pipeline using GitHub, Jenkins, Docker and Kubernetes

## Project Overview

This project demonstrates an End-to-End CI/CD Pipeline using GitHub, Jenkins, Docker and Kubernetes for automated application deployment. The pipeline automates code integration, application build, Docker image creation, image storage in Docker Hub and deployment to Kubernetes.

## Architecture Diagram

```text
+------------+
| Developer  |
+------------+
       |
       v
+------------+
|   GitHub   |
+------------+
       |
       v
+------------+
|  Jenkins   |
| Build/Test |
+------------+
       |
       v
+------------+
|   Docker   |
| Build Img  |
+------------+
       |
       v
+------------+
| Docker Hub |
+------------+
       |
       v
+------------+
| Kubernetes |
| Deployment |
+------------+
       |
       v
+------------+
| ReplicaSet |
+------------+
       |
       v
+------------+
|    Pods    |
+------------+
       |
       v
+------------+
|  Service   |
| NodePort   |
+------------+
       |
       v
+------------+
|  Browser   |
+------------+
```

## Tools Used

- Linux
- Git
- GitHub
- Jenkins
- Docker
- Docker Hub
- Kubernetes

## Workflow

1. Developer pushes source code to GitHub repository
2. Jenkins automatically triggers the CI/CD pipeline
3. Jenkins builds the application
4. Docker image is created using Dockerfile
5. Docker image is pushed to Docker Hub
6. Kubernetes Deployment pulls the latest image
7. ReplicaSet maintains the desired number of Pods
8. Service exposes the application
9. Users access the application through browser

## Jenkins Pipeline Stages

- Source Code Checkout
- Build Application
- Create Docker Image
- Push Docker Image to Docker Hub
- Deploy Application to Kubernetes

## Kubernetes Components Used

### Deployment

Manages application deployment and updates.

### ReplicaSet

Maintains the required number of Pod replicas.

### Pods

Runs containerized applications.

### Service

Provides stable network access to Pods.

## Benefits

- Automated application deployment
- Faster release process
- Reduced manual effort
- Consistent deployments
- Improved reliability
- Easy scalability
- Better collaboration between Development and Operations teams

## Sample Access Flow

```text
Developer
   ↓
GitHub
   ↓
Jenkins
   ↓
Application Build
   ↓
Docker Image
   ↓
Docker Hub
   ↓
Kubernetes Deployment
   ↓
ReplicaSet
   ↓
Pods
   ↓
Service (NodePort)
   ↓
Public IP + Port
   ↓
Browser
```

## Author

Vishnu M
