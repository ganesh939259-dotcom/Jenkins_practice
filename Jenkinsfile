pipeline {
    agent any 
    stages {
        stage('Docker Test') {
            steps {
                sh 'docker run --rm nginx:alpin nginx -v'
            }
        }
    }
}

