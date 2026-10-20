pipeline {
    agent any 
    stages {
        stage('Build') {
            steps {
                sh ' echo "Job name:$JOB_NAME"'
                sh ' echo "Build number:$BUILD_NUMBER"'
                sh ' echo "Workspace:$WORKSPACE"'
            }
        }
    }
}
