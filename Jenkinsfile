pipeline {
    agent any 
    stages {
        stage('Test') {
            steps{
                catchError (
                    buildResult: 'Success',
                    stageResult: 'Faliure',
                ) {
                    sh 'exit 1'
                }
            }
            stage('Deploy') {
                steps {
                    echo "Deploying the application"
                }
            }
        }
    }
}


                        
