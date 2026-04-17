# End-to-End DevOps Project 🚀

## Stack
- Java 17
- Spring Boot 3
- Jenkins
- Docker
- Kubernetes

## Flow
GitHub → Jenkins → Maven → Docker → Kubernetes

## Run
mvn clean package
docker build -t yourdockerhub/devops-app:v1 .
docker run -p 8080:8080 yourdockerhub/devops-app:v1

## Access
http://<node-ip>:30007

## Health Check
/actuator/health
