DevSecOps Project: Netflix Clone Deployment on the Cloud using Jenkins and ArgoCD

Successfully deployed a Netflix clone on the cloud using Jenkins for CI and ArgoCD for CD, implementing DevSecOps practices.

Here's a quick overview of the project:

Initial Setup:
Launched an EC2 instance (Ubuntu 22.04) on AWS.
Cloned the project code from GitHub.
Installed Docker and ran the application in a container.
Obtained an API key from TMDB.
Security:
Integrated SonarQube for code quality and security analysis.
Used Trivy for vulnerability scanning.
CI Pipeline:
Set up Jenkins for automation.
Installed necessary plugins.
Created a pipeline to automate build, test, and code analysis.
Pushed Docker images to a registry.
CD (Continuous Deployment) with ArgoCD:
Deployed ArgoCD on an EKS cluster.
Configured ArgoCD to sync with the Git repository containing the application manifests.
Enabled ArgoCD to automatically deploy new versions of the application based on changes in the Git repository.
Monitoring:
Installed Prometheus and Grafana for monitoring.
Integrated Jenkins with Prometheus for pipeline monitoring.
Notification:
Implemented email notifications using Jenkins.

Tools
Jenkins: 🛠️ Automation server
Docker: 📦 Containerization platform
SonarQube: 🔍 Code quality and security analysis
Trivy: 🛡️ Vulnerability scanner
Prometheus: 📊 Monitoring system
Grafana: 📈📉 Visualization tool
Kubernetes: 🐳 Container orchestration
ArgoCD: 🔄 Continuous deployment

Overall Flow:
Code is pushed to GitHub.
Jenkins triggers the pipeline.
Code is analyzed for quality and security.
Dependencies are checked.
Application is built and Docker images are pushed to a registry.
ArgoCD detects changes in the Git repository and deploys the new application version to the Kubernetes cluster.
Metrics are collected and visualized using Prometheus and Grafana.
Notifications are sent for issues or successful deployments.
This project demonstrates the power of DevSecOps in delivering secure and efficient applications. 🚀
