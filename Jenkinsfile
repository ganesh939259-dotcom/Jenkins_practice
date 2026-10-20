pipeline {
    agent any
    environment {
        APP_NAME = 'myapp'
    }
    stages{
        stage('Build') {
            steps {
                sh ' echo $APP_NAME'
            }
        }
    }
}
