pipeline {
    agent any 
    stages {
        stage('Creating Artifact') {
            steps {
                sh 'echo "Hello From Jenkins" > hello.txt'
                achiveArtifacts artifacts: 'hello.txt'
            }
        }
    }
}
