pipeline {
    agent any
    stages {
        stage('Creatin Artifact') {
            steps {
                sh 'echo "Hello from Jenkins > hello.txt"'
                archieveArtifact artifacts: 'hello.txt'
            }
        }
    }
}
