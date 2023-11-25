pipeline {
    agent {
        docker {
            image 'docker' // usa a imagem docker como agente
            args '-v /var/run/docker.sock:/var/run/docker.sock' // monta o socket do docker no contêiner
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'docker-compose build' 
            }
        }
        stage('Run') {
            steps {
                sh 'docker-compose up -d' // executa os contêineres definidos no docker-compose
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
