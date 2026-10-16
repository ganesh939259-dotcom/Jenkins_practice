pipeline {
    agent any 
    stages {
        stage('validate login') {
            steps {
                withCredentials([usernamePassword (
                    credentialsId: 'app-login',
                    usernameVariable: 'APP_USER',
                    passwordVariable: 'APP_PASSWORD'
                )]) {
                    sh 'test -n "$APP_USER"'
                    sh 'test -n "$APP_PASSWORD"'
                    echo 'Application Credentials configored Successfully'
                }
            }
        }
    }
}
