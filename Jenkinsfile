pipeline {
    agent any
    parameters {
        choice (
            name: "ENVIRONMENT",
            choices: ['dev', 'test', 'prod'],
            description: 'Select deployment environment'
        )
    }
    stages {
        stage('Deploy') {
            steps {
                echo "Deploying to ${params.ENVIRONMENT}"
            }
        }
    }
}
