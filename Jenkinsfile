pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                sh '''

                docker info
                java --version
                docker --version
                docker-compose --version
                '''
            }
        }
    }
}