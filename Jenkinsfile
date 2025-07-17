pipeline {
    agent any

    stages {
        stage('Build and Deploy with Docker Compose') {
            steps {
                sh 'docker compose down || true'
                sh 'docker compose up --build -d'
            }
        }
    }
}
