pipeline {
    agent any 
    parameters {
        choice (
            name: 'ENVIRONMENT',
            choices: ['dev', 'test', 'prod'],
            description: 'select your environment'
        )
    }
    stages {
        stage('Build') {
            steps {
                echo "Buildig the application"
            }
        }
        stage('Deploy') {
            when {
                expression {
                    params.ENVIRONMENT=='prod'
                }
            }
            steps{
                echo "deploying the application"
            }
        }
    }
}
