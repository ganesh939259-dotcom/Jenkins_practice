pipeline {
    agent {
        label 'linux'
    }
    stages {
        stage('Check Agent') {
            steps {
                sh 'whoami'
                sh 'pwd'
                sh 'hostname'
            }
        }
    }
}
