pipeline{
    agent any
    stages{
        stage('login') {
            steps {
                withCredentials([usernamePassword(
                    credentialsId: 'app-login',
                    usernameVariable: 'APP_USER',
                    passwordVariable: 'APP_PASSWORD'
                )]) {
                    sh 'test -n "$APP_USER"'
                    sh 'test -n "$APP_PASSWORD"'
                    echo 'app login configured successfully'
                }
            }
        }
    }
}
