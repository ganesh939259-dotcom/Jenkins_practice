pipeline {
    agent any 
    stages {
        stage('Creating Artifact') {
            steps {
                sh ' echo "Hello from jenkins" > app.txt'
                archiveArtifacts artifacts: 'app.txt'
            }
        }
    }
}
