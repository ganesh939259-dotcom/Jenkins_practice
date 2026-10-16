pipeline {
    agent any 
    stages {
        stage('validate login') {
            steps {
                withCredentials([
                    string(
                        credentialsId: 'practice-secret',
                        variable: 'API_TOKEN'
                    ),
                    usernamePassword(
                        credentialsId: 'app-login',
                        usernameVariable: 'APP_USER',
                        passwordVariable: 'APP_PASSWORD'
                    )
                ]) {
                    sh 'test -n "$API_TOKEN"'
                    sh 'test -n "$APP_USER"'
                    sh 'test -n "$APP_PASSWORD"'
                    echo 'All Credentials configured Successfully'
                }
            }
        }
    }
}
