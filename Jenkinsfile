pipeline {
    agent any
    
    stages {
        stage('inicializacao') {
            steps {
                sh '''
                docker-compose build
                docker-compose up
                '''
            }
        }
        
    }
    
}
