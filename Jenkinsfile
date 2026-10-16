pipeline{
    agent any
    stages {
        stage('Check secret') {
            steps {
                withCredentials([string (
                    credentialsId: "practice-secret",
                    variable: "MY_SECRET"
                )]) {
                    sh 'test -n "$MY_SECRET"'
                    echo 'configured successfully'
                }
            }
        }
    }
