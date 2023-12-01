pipeline {
    agent any

    stages {
        
        stage('Run') {
            steps {
                sh 'npm --version' // executa os contêineres definidos no docker-compose
            }
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
