pipeline {
    agent any

    stages {

        stage('Instalar dependências') {
            steps {
                bat ' npm install'
            }
        }

        stage('Run Tests') {
            steps {
                bat 'npm test'
            }
        }
    }
}
