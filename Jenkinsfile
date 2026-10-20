pipeline {
    agent any 
    stages {
        stage('Creating the artifact') {
            steps {
                sh ' echo "Application:nginx" > app.txt'
                sh ' echo "version:1.0" > version.txt'
                sh ' echo "jenkins artifact practice" > readme.log'
                archiveArtifacts artifacts: '*.txt'
            }
        }
    }
}
