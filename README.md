# CI/CD Pipeline with Jenkins, SonarQube, Docker, and Kubernetes

This project implements a complete CI/CD pipeline using Jenkins for CI, SonarQube for code analysis, Docker for containerization, and Kubernetes with Helm for deployment.

## CI Process

1. **Checkout code**: Jenkins checks out the code from the version control system.
2. **Run SonarQube analysis**: Jenkins runs a SonarQube analysis to analyze the code quality.
3. **Build application**: Jenkins builds the application using the checked-out code.
4. **Archive the artifact**: Jenkins archives the built artifact for later use in the CD process.

## CD Process

1. **Build Docker image using the artifact**: Jenkins uses the archived artifact to build a Docker image of the application.
2. **Push Docker image to Docker Hub**: Jenkins pushes the built Docker image to Docker Hub for storage and deployment.
3. **Deploy application to Kubernetes using Helm**: Jenkins deploys the application to Kubernetes using Helm charts.

## Installation Required

1. **Jenkins setup**
2. **SonarQube setup**
3. **Kubernetes setup**
4. **Helm setup**
5. **Grefana Monitoring Tool**

## Usage

1. Configure Jenkins to connect to your version control system and SonarQube server.
2. Set up Jenkins pipelines for both the CI and CD processes, defining the stages mentioned above.
3. Run the Jenkins pipeline for your project to trigger the CI/CD process.
4. Monitor the pipeline execution in Jenkins and check the deployed application in your Kubernetes cluster.







