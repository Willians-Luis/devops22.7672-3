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
                bat 'npm run test'
                bat 'npm run test:ci'
            }
        }
    }
}
