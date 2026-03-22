pipeline {
    agent any

    stages {
        stage('Build Java App') {
            steps {
                sh '''
                echo "Building Java app..."
                /opt/homebrew/bin/mvn clean package
                '''
            }
        }

        stage('Run Java App') {
            steps {
                sh '''
                echo "Running Java app..."
                java -cp target/jenkins-demo-1.0.jar App
                '''
            }
        }
    }
}
