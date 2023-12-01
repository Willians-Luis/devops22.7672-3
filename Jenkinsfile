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
                bat '''
                npm  test
                npm test:ci
                npm teste:e2e
                '''
            }
        }
    }
}
