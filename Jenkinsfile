pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git 'https://github.com/evism1054/static-website.git'
            }
        }

        stage('Build and Deploy with Docker Compose') {
            steps {
                sh 'docker-compose down || true'
                sh 'docker-compose up --build -d'
            }
        }
    }
}
