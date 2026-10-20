pipeline {
    agent any 
    stage('Build Docker Image') {
    steps {
        sh 'docker build -t myapp-ganesh:latest .'
    }
}
stages {
        stage('Deploy') {
            steps {
                sh '''
                docker rm -f mycontainers || true
                docker run --name mycontainers -d -p 8085:80 myapp-ganesh
                '''
            }
        }
    }
}
