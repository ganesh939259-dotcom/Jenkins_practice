pipeline {
    agent any
    stages {
        stage ('Build') {
            steps {
                echo "Building application"
            }
        }
    }
    post {
        always {
            echo "pipeline executed successfully"
        }
        success {
            echo "pipeline successed"
        }
        failure {
            echo "pipeline failed"
        }
    }
}
