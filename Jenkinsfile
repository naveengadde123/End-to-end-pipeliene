pipeline {
    agent { label 'docker' }

    stages {
        stage('Test Agent') {
            steps {
                sh 'hostname'
                sh 'whoami'
            }
        }
    }
}
