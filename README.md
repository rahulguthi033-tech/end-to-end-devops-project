# End-to-End DevOps Project 🚀

## Tools
- Maven
- Jenkins
- Docker
- Kubernetes
- Prometheus
- Grafana

## Work-Flow
Developer pushes code to GitHub
Jenkins pulls code
Maven Builds WAR/JAR File
Docker Builds Images
Push Image To Docker Hub
Kubernetes Deploys Container
Prometheus Monitoring
Grafana shows Dashboards

## Run
mvn clean package
docker build -t yourdockerhub/devops-app:v1 .
docker run -p 8080:8080 yourdockerhub/devops-app:v1

## Access
http://<node-ip>:30007

## Health Check
/actuator/health
