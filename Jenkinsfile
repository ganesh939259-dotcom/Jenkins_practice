pipeline {
    agent any 
    stages {
        stage ('Checkout') {
            steps {
                echo "code checkout the application"
            }
        }
        stage ('Build') {
            steps {
                echo "Building the application"
            }
        }
        stage ('Test') {
            steps {
                echo "Testing the application"
            }
        }
        stage ('Deploy') {
            steps {
                echo "Deploying the application"
            }
        }
        stage ('app-login') {
            steps {
                withCredentials([string (
                    credentialsId: 'practice-secret',
                    variables: 'API_TOKEN'
                )]) {
                    sh 'test -n "$API_TOKEN"'
                    echo 'API token configured successfully'
                }
            }
        }
    }
}
