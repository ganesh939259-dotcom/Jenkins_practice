pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                retry(2) {
                    sh ' echo "Building application"'
                }
            }
        }
    }
}
