pipeline {
    agent any
    stages {
        stage('Creating Artifact') {
            steps {
                sh ' echo "Iam Learning Jenkins Here" > hello.txt'
                archiveArtifacts artifacts: 'hello.txt'
            }
        }
    }
}
