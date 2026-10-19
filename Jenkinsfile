pipeline {
    agent any
    stages {
        stage('Creating Artifact') {
            steps {
                sh 'echo "Really become to devops engineer" > devops
                archiveArtifacts artifacts: 'devops'
            }
        }
    }
}
