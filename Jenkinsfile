pipeline {
    agent any 
    stages {
        stage('secrete key') {
            steps {
                withCredentials([string (
                    credentialsId: 'practice-secret',
                    variable: 'API_TOKEN'
                )]) {
                    sh 'test -n "$API_TOKEN"'
                    echo 'api token taken successfully'
                }
            }
        }
    }
}
