pipeline {
    agent any

    environment {
        PATH = "/usr/local/bin:/opt/homebrew/bin:/usr/bin:/bin:/usr/sbin:/sbin"
    }

    stages {
        stage('Check Docker') {
            steps {
                sh '''
                echo "Checking Docker..."
                which docker
                docker --version
                '''
            }
        }

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
