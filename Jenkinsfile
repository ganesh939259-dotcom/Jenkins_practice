pipeline {
    agent any 
    stages {
        stage('Test') {
            steps {
                catchError (
                    buildResult: 'Success',
                    stageResult: 'failure'
                ) {
                    sh 'exit 1'
                }
            }
        }
        stage('Deploy') {
            steps {
                echo "Deploying Application"
            }
        }
    }
}
