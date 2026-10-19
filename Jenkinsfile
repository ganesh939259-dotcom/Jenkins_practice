pipeline {
    agent any
    stages {
        stage('parallel Testing') {
            parallel {
                stage('Linux check') {
                    steps {
                        echo "checking linux environment"
                    }
                }
                stage('Docker Check') {
                    steps {
                        echo "Checking Docker environment"
                    }
                }
            }
        }
    }
}
