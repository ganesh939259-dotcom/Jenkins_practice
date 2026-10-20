pipeline {
    agent any 
    stages {
        stage('Build') {
            steps {
                echo "Building the application"
            }
        }
        stage('Approve') {
            steps {
                input message: 'Approve development?'
            }
        }
        stage('Deploy') {
            steps {
                echo "Deploying the application"
            }
        }
    }
}
