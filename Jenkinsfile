pipeline {
    agent any
    
    stages {
        stage('Build Docker Image') {
            steps {
                sh 'docker build -t junweill111/mynewimage:latest .'
            }
        }
        
        stage('Push Docker Image') {
            steps {
                sh 'docker push junweill111/mynewimage:latest'
            }
        }
    }
}
