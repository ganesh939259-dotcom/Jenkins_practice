pipeline {
    agent { label 'linux-agent' }
    stages {
        stage('Verify agent') {
            steps {
                sh 'hostname'
                sh 'whoami'
                sh 'pwd'
            }
        }
    }
}

              
