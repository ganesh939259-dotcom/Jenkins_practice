pipeline {
    agent { label 'linux-agent' }
    stages {
        stage('system information') {
            steps {
                sh '''
                echo "Current User: $pwd"
                echo "Hostname: $hostname"
                echo "Current Working directory: $pwd"
                echo "Build number: $BUILD_NUMBER"
                echo "Workspace: $WORKSPACE"
                '''
            }
        }
    }
}
