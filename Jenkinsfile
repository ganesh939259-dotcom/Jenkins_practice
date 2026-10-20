pipeline {
    agent any 
    stages {
        stage('Build') {
            steps {
                echo "Building the application"
            }
        }
        stage('Test'){
            steps {
                echo "Testing the application"
            }
        }
        stage('Approve') {
            steps {
                input message: 'Approve the deploying'
            }
        }
        stage('Deploy') {
            steps {
                echo "Deploying the application"
            }
        }
    }
}
