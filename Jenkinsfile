pipeline {
    agent any

    stages {

        stage('Build Docker Image') {
            steps {
                bat 'docker build -t portfolio-app .'
            }
        }

        stage('Deploy Using Ansible') {
            steps {
                bat 'wsl -d Ubuntu ansible-playbook /home/rajbole/devops/deploy.yml'
            }
        }
    }
}