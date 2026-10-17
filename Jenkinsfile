pipeline {
    agent any 
    stages {
        stage ('check agent') {
            steps {
                sh 'date'
                sh 'uname -a'
                sh 'df -h .'
            }
        }
    }
}
