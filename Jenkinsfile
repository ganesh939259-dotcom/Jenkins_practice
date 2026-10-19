pipeline {
    agent any
    stages {
        stage('api-token') {
            steps {
                withCredentials([string (
                    credentialsId: 'practice-secret',
                    Variable: 'API_TOKEN'
                )]) {
                    sh 'test -n "$API_TOKEN"'
                    echo "API configured Successfully"
                }
            }
        }
    }
}
