pipeline  {
    agent any
    stages {
        stage('Build') {
            steps {
                echo "Building the application"
            }
        }
        stage('Approval') {
            steps {
                input message: 'Approve deployment?'
            }
        }
        stage('Deploy') {
            stage {
                steps {
                    echo "Deploying the applications"
                }
            }
        }
    }
}
