pipeline {
    agent any

    stages {
        stage('Clonar o repositorio') {
            steps {
                git 'https://github.com/GabriellaBianchi22/modulo-12.git'
            }
        }
                stage('Instalar dependencias') {
            steps {
                bat 'npm install'
            }
        }
                stage('Executar os teste') {
            steps {
                bat 'NO_COLOR=1 npm run cy:run'
            }
        }
    }
}