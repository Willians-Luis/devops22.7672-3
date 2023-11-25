pipeline {
    agent any
    
    stages {
        stage('teste') {
            steps {
                sh '''
                git --version
                java --version
                docker --version
                '''
            }
        }
        
    }
    
}
