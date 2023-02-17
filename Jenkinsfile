pipeline {
    agent any
    stages {
        stage('AFerski - Build Docker Image') {
            steps {
                script {
                    sh 'docker build -t python-t22dev01 .'
                }
            }
        }
        stage('AFerski - Login to Docker Hub') {
            steps {
                echo 'Hello World'
            }
        }
        stage('AFerski - Push Image to Docker Hub') {
            steps {
                echo 'Hello World'
            }
        }
    }
}
