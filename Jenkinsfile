pipeline {

    agent any

    stages {

        stage('Stage 1') {
            steps {
                echo "Pipeline started..."
            }
        }

        stage('Stage 2') {
            steps {
                echo "This is running on Ubuntu Jenkins server."
            }
        }

        stage('Stage 3') {
            steps {
                echo "Build stage completed."
            }
        }
    }

    post {
        success {
            echo "Pipeline completed successfully."
        }
        failure {
            echo "Pipeline failed."
        }
    }
}
