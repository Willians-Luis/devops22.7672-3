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
                bat 'npm teste:e2e'
                bat 'npm test:ci'
            }
        }
    }
}
