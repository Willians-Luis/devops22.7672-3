pipeline {
    agent any

    stages {

        stage('Instalar dependencias') {
            steps {
                bat ' npm install'
            }
        }

        stage('Rodar testes') {
            steps {
                bat 'npm test'
                bat 'test:e2e'
                bat 'test:ci'
            }
        }
    }
}
