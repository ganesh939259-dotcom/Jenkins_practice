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
                echo "Testing the application"
            }
        }
    }
    post {
        always {
                echo "pipeline finished"
        }
    }
}

