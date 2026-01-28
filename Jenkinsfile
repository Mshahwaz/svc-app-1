pipeline {
    agent any
    environment {
        REPO = "app1-flask"
        TAG = "${BUILD_NUMBER}"
        PORT = "5000"
    }
    stages{
        stage('Build'){
            steps{
                sh 'docker build -t "$REPO:$TAG" . '
            }
        }
    }
}