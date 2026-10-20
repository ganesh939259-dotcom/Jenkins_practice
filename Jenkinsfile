
pipeline {
    agent any

    parameters {
        string(
            name: 'APP_NAME',
            defaultValue: 'nginx',
            description: 'Enter application name'
        )

        choice(
            name: 'ENVIRONMENT',
            choices: ['dev', 'test', 'prod'],
            description: 'Select deployment environment'
        )
    }

    environment {
        VERSION = '1.0'
    }

    stages {
        stage('Checkout') {
            steps {
                echo 'Checking out source code'
            }
        }

        stage('Build') {
            steps {
                echo "Building ${params.APP_NAME} version ${env.VERSION}"
            }
        }

        stage('Deploy') {
            when {
                expression {
                    params.ENVIRONMENT == 'test'
                }
            }
            steps {
                echo "Deploying ${params.APP_NAME} to ${params.ENVIRONMENT}"
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully'
        }

        failure {
            echo 'Pipeline failed'
        }
    }
}
