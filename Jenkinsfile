pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/naveengadde123/End-to-end-pipeliene'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t myapp:latest .'
            }
        }

        stage('Run Container') {
            steps {
                sh 'docker run -d -p 8080:8080 myapp:latest'
            }
        }
    }
}
