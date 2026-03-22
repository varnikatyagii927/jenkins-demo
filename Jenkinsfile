pipeline {
    agent any

    stages {
        stage('Build Java App') {
            steps {
                sh '''
                echo "Compiling Java..."
                javac App.java
                '''
            }
        }

        stage('Run Java App') {
            steps {
                sh '''
                echo "Running Java App..."
                java App
                '''
            }
        }
    }
}
