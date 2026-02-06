pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'mvn clean package -DskipTests'
            }
        }

        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }

        stage('Docker Build & Push') {
            steps {
                sh '''
                  docker build -t naveenchowdari/myapp:latest .
                  docker push naveenchowdari/myapp:latest
                '''
            }
        }
    }
}
