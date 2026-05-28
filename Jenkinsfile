pipeline {
    agent any

    stages {

        stage('Clone Code') {
            steps {
                echo 'Cloning repository...'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t aws-devops-project .'
            }
        }

        stage('Check Docker Images') {
            steps {
                sh 'docker images'
            }
        }

    }
}