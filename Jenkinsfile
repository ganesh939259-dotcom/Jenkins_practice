pipeline {
    agent any 
    stages {
        stage('Creating Artifact') {
            steps {
                sh 'echo "Hello From Jenkins > hello.txt"'
                achieveArtifact artifacts: 'hello.txt'
            }
        }
    }
}
