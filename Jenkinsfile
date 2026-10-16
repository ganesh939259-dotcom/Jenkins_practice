pipeline {
    agent any 
    stages {
        stage('Build application') {
            steps {
                echo "Building application"
                sh 'exit 1'
            }
        }
    }
    post {
        success {
            echo "Build Completed Successfully"
        }
        failure {
            echo "Build failured"
        }
        always {
            echo "pipeline execution completed"
        }
        aborted {
            echo 'Pipeline was aborted'
        }
    }
}
