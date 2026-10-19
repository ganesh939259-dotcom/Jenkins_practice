@Library('devops-library') _

pipeline {
    agent any 
    stages {
        stage('shared testing libraries') {
            steps {
                greet('Linux !')
                greet('docker !')
                greet('Jenkins !')
                greet()
            }
        }
    }
}
