pipeline {
    agent any
    
    stages {
        stage('Build and Push Docker Image') {
            steps {
                script {
                    docker.build("junweill111/mynewimage:latest")
                    docker.withRegistry('', 'docker-hub-credentials-id') {
                        docker.image("junweill111/mynewimage:latest").push()
                    }
                }
            }
        }
    }
}
