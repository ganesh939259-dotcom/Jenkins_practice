pipeline {
    agent any
    parameters {
        choice (
            name: 'ENVIRONMENT',
            choices: ['dev','test','prod'],
            description: 'select environment'
        )
    }
    stages{
        stage('build') {
            steps {
                sh ' echo $ENVIRONMENT'
            }
        }
    }
}
