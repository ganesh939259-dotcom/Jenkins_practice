pipeline {
    agent any 
    parameters {
        string (
            name: 'APP_NAME',
            defaultValue: 'nginx',
            description: "Enter application name"
        )
        choice (
            name: 'ENVIRONMENT',
            choices: ['dev','test','prod'],
            description: "select deployment application"
        )
    }
    stages {
        stage('Deploy') {
            steps {
                echo "deploying: ${params.APP_NAME}"
                echo "deploying: ${params.ENVIRONMENT}"
            }
        }
    }
}
