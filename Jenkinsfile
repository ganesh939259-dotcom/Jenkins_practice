pipeline {
    agent any
    environment {
        APP_ENV='nginx'
        APP_NAME='demo-app'
        APP_VERSION='1.0'
    }
    stages {
        stage('checking environment') {
            steps {
                echo "application: ${env.APP_NAME}"
                echo "ENVIRONMENT: ${env.APP_ENV}"
                echo "VERSION: ${env.APP_VERSION}"

                sh '''
                echo "build number:$BUILD_NUMBER"
                '''
            }
        }
    }
}
