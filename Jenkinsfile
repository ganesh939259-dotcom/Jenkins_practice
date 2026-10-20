pipeline {
    agent any 
    stages {
        stage('Building Docker image') {
            steps {
                sh ' docker build -t myapp-ganesh .'
            }
        }
        stage('Deploy the container') {
            steps {
                sh '''
                docker rm -f mycontainers || true
                docker run --name mycontainers -d -p 8085:80 myapp-ganesh
                '''
            }
        }
    }
}
