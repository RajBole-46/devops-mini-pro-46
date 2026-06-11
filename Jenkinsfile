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
                bat 'wsl ansible-playbook /home/rajbole/devops/deploy.yml'
            }
        }

        stage('Verify Deployment') {
            steps {
                bat 'docker ps'
            }
        }
    }

    post {
        success {
            echo 'Deployment Successful!'
        }
        failure {
            echo 'Deployment Failed!'
        }
    }
}