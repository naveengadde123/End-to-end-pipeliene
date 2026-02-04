pipeline {
    agent any

    stages {
        stage('Test Jenkins') {
            steps {
                echo 'Pipeline working'
            }
        }

        stage('Build') {
            steps {
                // Run Maven build
                sh 'mvn clean install'
            }
        }

        stage('Test') {
            steps {
                // Run Maven tests
                sh 'mvn test'
            }
        }
    }
}
