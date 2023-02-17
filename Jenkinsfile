pipeline {
    agent any
    stages {
        stage('AFerski - Build Docker Image') {
            steps {
                script {
                    sh 'docker build -t biscuit93/python-t22dev01 .'
                }
            }
        }
        stage('AFerski - Login to Docker Hub') {
            steps {
                script{
                    withCredentials([string(credentialsId: 'dockerhubpassword', variable: 'dockerhubpassword')]) {
                              sh 'docker login -u biscuit93 -p ${dockerhubpassword}'
}
                }
            }
        }
        stage('AFerski - Push Image to Docker Hub') {
            steps {
                script{
                    sh 'docker push biscuit93/python-t22dev01'
                }
            }
        }
    }
}
