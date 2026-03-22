pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh '''
                echo "Installing Python..."
                python3 --version
                '''
            }
        }

        stage('Run App') {
            steps {
                sh '''
                echo "Running Python app..."
                python3 app.py
                '''
            }
        }
    }
}
