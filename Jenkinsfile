pipeline {
    agent any
    environment {
        APP_ENV='test'
        APP_NAME='demo-app'
    }
    stages {
        stage('checking Environment variable') {
            steps {
                echo "application: ${env.APP_NAME}"
                echo "Environment: ${env.APP_ENV}"

                sh '''
                echo "Build number: $BUILD_NUMBER"
                echo "Workspace: $WORKSPACE"
                '''
            }
        }
    }
}
