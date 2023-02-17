pipeline {
    agent any
    stages {
        stage('AFerski - Pull from Repository') {
            steps {
                checkout scmGit(branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/Biscuit93/T-22-DEV-01.git']])
            }
        }
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
