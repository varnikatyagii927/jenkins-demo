pipeline {
    agent any

    stages {
        stage('Build Docker Image') {
            steps {
                sh '''
                echo "Building Docker image..."
                docker build -t java-app .
                '''
            }
        }

        stage('Run Docker Container') {
            steps {
                sh '''
                echo "Running Docker container..."
                docker run java-app
                '''
            }
        }
    }
}
