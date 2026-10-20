pipeline {
    agent any
    parameters {
        string (
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
