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
        failed {
            echo "pipeline failed"
        }
    }
}
