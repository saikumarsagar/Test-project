Please find updated repo in gitlab( ++ Var, shared library Docker build for jenkins)
https://gitlab.com/saikumarsagar/project1-docker.git
git@gitlab.com:saikumarsagar/project1-docker.git


Testing Project to perform 
1. Maven build
2. Docker Build
3. Kubernetes deploy 
4. Helm implentation 

To access the App- instance_ip:8080/WebAppCal-1.3.7

Docker repo-
docker pull saidocker2048/project1-docker
(or)

docker pull saidocker2048/project1-docker:latest



Project1 Docker - Jenkins Integration and CI/CD Pipeline

Welcome to Project1 Docker! This repository showcases the integration of Jenkins with Docker, Kubernetes, and Helm for seamless CI/CD implementation. The purpose of this project is to automate the building, deployment, and management of applications using Maven, Docker, and Helm.

🚀 Features
Maven Build: Automate Java project builds using Maven.
Docker Build: Create and manage Docker images for your applications.
Kubernetes Deployment: Deploy Docker containers to Kubernetes clusters.
Helm Implementation: Manage Kubernetes applications with Helm charts.
📦 Prerequisites
Before you begin, ensure that the following software/tools are installed on your machine:

Docker (version 20.10 or higher)
Kubernetes (with kubectl configured)
Helm (version 3 or higher)
Maven
Git
🛠️ Setup Instructions
1. Clone the Repository
bash
Copy
Edit
git clone https://gitlab.com/saikumarsagar/project1-docker.git
or

bash
Copy
Edit
git clone git@gitlab.com:saikumarsagar/project1-docker.git
2. Maven Build
Navigate to the project directory and execute the following Maven command to build the project:

bash
Copy
Edit
cd project1-docker
mvn clean install
This will compile and build the application. Ensure that the build succeeds before moving to the next steps.

3. Docker Build
Build the Docker image for the project:

bash
Copy
Edit
docker build -t saidocker2048/project1-docker .
Alternatively, you can pull the pre-built image from Docker Hub:

bash
Copy
Edit
docker pull saidocker2048/project1-docker:latest
4. Kubernetes Deployment
Deploy the application on your Kubernetes cluster. First, ensure your Kubernetes cluster is set up, and then apply the Kubernetes deployment configuration:

bash
Copy
Edit
kubectl apply -f kubernetes-deployment.yaml
5. Helm Implementation
To manage your Kubernetes applications more efficiently, install and deploy with Helm. First, ensure Helm is installed, and then deploy the app using:

bash
Copy
Edit
helm install my-app ./helm-chart
This will deploy your application on Kubernetes using Helm, enabling better management and scaling.

🌐 Accessing the Application
Once deployed, you can access the application by navigating to the following URL in your browser:

cpp
Copy
Edit
http://<instance_ip>:8080/WebAppCal-1.3.7
Make sure the instance_ip is the public IP of the node where your app is hosted.

🐳 Docker Image
The Docker image for the project is available on Docker Hub. You can pull it using the following command:

bash
Copy
Edit
docker pull saidocker2048/project1-docker
Or pull the latest tag:

bash
Copy
Edit
docker pull saidocker2048/project1-docker:latest
📖 Usage
Build the Maven project.
Create a Docker image.
Deploy the application using Kubernetes and Helm.
🔧 Troubleshooting
If you encounter any issues during the build or deployment process, please refer to the logs or raise an issue in the GitHub repository. Common problems could include:

Incorrect Dockerfile paths
Kubernetes deployment configuration issues
Missing Helm charts
For further assistance, feel free to check the official Kubernetes documentation, Helm documentation, or create a GitHub issue.

📜 License
This project is licensed under the MIT License - see the LICENSE file for details.

🤝 Contributing
We welcome contributions! If you'd like to improve the project, feel free to fork the repo and create a pull request.

🔗 Links
GitLab Repo
Docker Hub - Project Image
