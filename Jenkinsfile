pipeline {
    agent any 
    stages {
        stage('Building'){
            steps {
                echo "Buildig the application"
            }
        }
        stage('Testing'){
            steps {
                echo "Testing the application"
            }
        }
    }
    post {
        success{
            echo "pipeline executed successfully"
        }
        failure {
            echo "pipeline failure"
        }
    }
}
