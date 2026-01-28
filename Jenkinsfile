pipeline {
    agent any
    environment {
        REPO = "app1-flask"
        TAG = "${BUILD_NO}"
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