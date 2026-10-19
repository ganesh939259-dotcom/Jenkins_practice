pipeline {
    agent any
    environment {
        APP_NAME='nginx'
        APP_ENV='test'
    }
    stages {
        stage('Deploy application') {
            when {
                environment name: "APP_ENV", value: 'test'
            }
            steps {
                echo "application: ${env.APP_NAME}"
                echo "environment: ${env.APP_ENV}"
                echo "Deploying application Test environment"
            }
        }
    }
}

                
