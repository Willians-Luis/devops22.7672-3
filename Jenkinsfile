pipeline {
    agent any
    
    stages {
        
        stage('Install Dependencies') {
            steps {
                sh '''
                cd NodeGoat
                cd NodeGoat
                docker-compose build
                docker-compose up
                '''
            }
        }
        
        stage('Run Tests') {
            steps {
                sh './node_modules/.bin/cypress run --config-file cypress.json'
            }
        }
        
        
    }
    
}
