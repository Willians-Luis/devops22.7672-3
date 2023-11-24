pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                git 'https://seu-repositorio.git'
            }
        }
        
        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }
        
        stage('Run Tests') {
            steps {
                sh './node_modules/.bin/cypress run --config-file cypress.json'
            }
        }
        
        
    }
    
}
