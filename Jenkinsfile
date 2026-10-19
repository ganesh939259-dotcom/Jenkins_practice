pipeline {
    agent any
    stages {
        stage('Creating Artifacts') {
            steps {
                sh ' echo "Hello From Jenkins" > hello'
                sh ' echo "DevOps practice" > app'
                archiveArtifacts artifacts: 'hello,app'
            }
        }
    }
}
