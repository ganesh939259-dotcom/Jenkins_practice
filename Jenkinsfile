pipeline {
    agent any
    stages {
        stage('Create Artifact') {
            steps {
                sh 'echo "Hello from jenkins" > hello.txt'
                archiveArtifacts artifacts: 'hello.txt'
            }
        }
    }
}
