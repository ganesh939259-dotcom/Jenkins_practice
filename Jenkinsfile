pipeline {
    agent any 
    stages {
        stage('Build') {
            steps {
                echo "Building the application"
            }
        }
    }
    post {
        success {
            echo "pipeline executed successfully"
        }
        failure {
            echo "pipeline failed"
        }
    }
}
