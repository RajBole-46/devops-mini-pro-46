Malvan torisum Website

This project is a photography website developed using HTML and CSS. The website showcases photography collections, gallery images, services, and contact information related to Malvan Photography.

Features
Responsive Design
Photography Gallery
Services Section
Contact Information
Dockerized Application
CI/CD Pipeline using Jenkins
Project Structure
index.html : Main webpage
styles.css : Website styling
img/ : Image resources
Dockerfile : Docker configuration
Jenkinsfile : CI/CD pipeline configuration
deploy.yml : Ansible deployment file
How to Run the Project
Clone Repository
git clone https://github.com/RajBole-46/devops-mini-pro-46.git
cd devops-mini-pro-46
Run with Docker

Build Docker Image:

docker build -t malvan-photography .

Run Docker Container:

docker run -d -p 8080:80 --name malvan-photography malvan-photography

Access Website:

http://localhost:8080
CI/CD Pipeline

The Jenkins pipeline performs:

Clone project from GitHub
Build Docker image
Deploy Docker container
Verify deployment
Technologies Used
HTML
CSS
GitHub
Jenkins
Docker
Ansible
Author

Raj Dilip Bole

MCA - DevOps Mini Project
