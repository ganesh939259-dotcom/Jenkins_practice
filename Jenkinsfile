pipeline {
    agent any 
    stages {
        stage ('Retry Demo') {
            steps {
                retry(3) {
                    sh 'echo "Command executed successfully"'
                }
            }
        }
    }
}
