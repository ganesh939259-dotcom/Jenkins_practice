
pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Code checkout stage'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the application'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing the application'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the application'
            }
        }

        stage('Use Credentials') {
            steps {
                withCredentials([string(
                    credentialsId: 'practice-secret',
                    variable: 'MY_SECRET'
                )]) {
                    sh 'test -n "$MY_SECRET"'
                    echo 'Credential is configured successfully'
                }
            }
        }
    }
}
