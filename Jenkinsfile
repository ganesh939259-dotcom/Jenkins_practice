pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo "Building the application"
            }
        }
        stage('Test') {
            steps {
                echo "Test running"
                sh 'exit 0'
            }
        }
        stage('Deploy') {
            steps {
                echo "Deploying Application"
            }
        }
    }
    post {
        success {
            echo "pipeline successed"
        }
        failure {
            echo "pipeline failure"
        }
    }
}

        
