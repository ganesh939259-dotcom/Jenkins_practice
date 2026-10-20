pipeline {
    agent any 
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
