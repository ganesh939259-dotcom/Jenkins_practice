pipeline {
    agent any 
    stages {
        stage ('check agent') {
            steps {
                sh 'hostname'
                sh 'whoami'
                sh 'pwd'
            }
        }
    }
}
