pipeline {
    agent any 
    stages {
        stage('Creating Username') {
            steps {
                withCredentials([usernamePassword (
                    credentialsId: 'demo-credentials',
                    usernameVariable: 'APP_USER',
                    passwordVariable: "APP_PASSWORD"
                )]) {
                    sh ' echo "username:$APP_USER"'
                }
            }
        }
    }
    post {
        always {
            echo "pipeline executed successfully"
        }
    }
}

