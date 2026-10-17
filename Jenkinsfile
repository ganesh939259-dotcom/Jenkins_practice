pipeline {
    agent any
    stages {
        stage ('app-login') {
            steps {
                withCredentials([string (
                    credentialsId: 'practice-secret',
                    variable: 'API_TOKEN'
                )]) {
                    sh 'test -n "$API_TOKEN"'
                    echo 'app configured successfully'
                }
            }
        }
    }
}
