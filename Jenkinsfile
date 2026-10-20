pipeline {
    agent any
    parameters {
        choice (
            name: 'ENVIRONMENT',
            choices: ['dev','test','prod'],
            description: 'selecting the environment'
        )
    }
    stages{
        stage('Build') {
            steps {
                echo "Building the application"
            }
        }
        stage('Deploy') {
            when {
                expression {
                    params.ENVIRONMENT == 'prod'
                }
            }
            steps {
                echo "deploying the application"
            }
        }
    }
}
