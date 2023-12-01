pipeline {
    agent any

    stages {
        
        stage('Run') {
            steps {
                bat 'docker-compose up -d'
        }
        /*
        stage('Test') {
            steps {
                // insira aqui os comandos para testar a sua aplicação
            }
        }
        stage('Stop') {
            steps {
                sh 'docker-compose down' // para os contêineres definidos no docker-compose
            }
        }
        */
    }
}
