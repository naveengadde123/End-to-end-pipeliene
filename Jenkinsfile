pipeline {
    agent any

    stages {
        stage('Build Docker Image') {
            steps {
                bat 'docker build -t myapp:latest .'
            }
        }

        stage('Run Container') {
            steps {
                bat 'docker run -d -p 8088:8088 myapp:latest'
            }
        }
    }
}
