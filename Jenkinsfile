pipeline {
    agent any
    stages {
        stage('Creating Multiple Artifacts') {
            steps {
                sh ' echo "Hello From Jenkins" > app.txt'
                sh ' echo "version 1.0" > version.txt'

                archiveArtifacts artifacts: 'app.txt,version.txt'
            }
        }
    }
}
