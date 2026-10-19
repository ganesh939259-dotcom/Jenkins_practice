pipeline {
    agent any 
    stages {
        stage('Checking username and passwd') {
            steps {
                withCredentials([usernamePassword (
                    credentialsId: 'practice-username',
                    usernameVariable: 'APP_USER',
                    passwordVariable: 'APP_PASSWORD'
                )]) {
                    sh 'test -n "$APP_USER"'
                    sh 'test -n "APP_PASSWORD"'
                    echo "Username and password configured successfully"
                }
            }
        }
    }
}
