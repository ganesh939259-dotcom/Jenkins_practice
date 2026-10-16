pipeline {
    agent any
    parameters {
        choice(
            name: 'ENVIRONMENT',
            choices: ['dev', 'test', 'prod'],
            description: 'Select deployment environment'
        )
    }
    stages {
        stage('Show environment') {
            steps {
                echo "Selected environment: ${params.ENVIRONMENT}"
                }
            }
        }
    }
}
