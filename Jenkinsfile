pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/Willians-Luis/devops22.7672-3.git'
            }
        }
        
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
