pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
               sh '''
                echo "Current user:"
                whoami
                echo "Current directory:"
                pwd
                '''
            }
        }

        stage('Test') {
            steps {
                echo "Running tests..."
            }
        }
    }
}
