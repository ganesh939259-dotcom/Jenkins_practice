pipeline {
    agent any 
    stages{
        stage('Username and Password') {
            steps{
                withCredentials([usernamePassword (
                    credentialsId: 'demo-credentials',
                    usernameVariable: 'APP_USER',
                    passwordVariable: 'APP_PASSWORD'
                )]) {
                    sh 'test -n $APP_USER'
                    sh 'test -n $APP_PASSWORD'
                    echo "never print password"
                }
            }
        }
    }
}
