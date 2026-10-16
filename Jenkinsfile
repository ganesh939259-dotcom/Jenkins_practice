pipeline {
    agent any
    stages {
        stage('Test pipeline') {
            steps {
                sh 'echo "Running Pipeline"'
            }
        }
    }
    post {
        success {
            echo "pipeline completed successfully"
        }
        failure {
            echo "pipeline failed"
        }
    }
}
