pipeline {
    agent any
    parameters {
        choice (
            name: 'ENVIRONMENT',
            choices: ['dev','test','prod'],
            defaultValue: 'selecting the environment'
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
