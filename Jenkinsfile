pipeline {
    agent any 
    stages {
        stage('Docker Test') {
            steps {
                sh 'docker run --rm nginx:alpine nginx -v'
            }
        }
    }
}

