# Jenkins CI/CD Pipeline with SonarQube and Snyk

## Description
This project demonstrates a secure Jenkins pipeline for a Python application using SonarQube for code quality and Snyk for vulnerability scanning.

## How to Run
- Start Jenkins:
```bash
docker run -d -p 8080:8080 -v jenkins_home:/var/jenkins_home jenkins/jenkins:lts
```
- Create a Jenkins job and use `Jenkinsfile` from this repo.

## Tools Used
- Jenkins
- SonarQube
- Snyk
