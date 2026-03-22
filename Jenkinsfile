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

          stage('test') {
            steps {
                sh 'ls -la'
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
