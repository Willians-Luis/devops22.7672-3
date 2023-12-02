pipeline {
    agent any

    stages {

        stage('Instalar dependencias') {
            steps {
                bat 'npm install'
            }
        }

        stage('iniciar aplicacao') {
            steps {
                bat 'docker-compose up -d'
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
