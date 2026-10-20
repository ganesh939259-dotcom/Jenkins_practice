pipeline {
    agent any
    stages {
        stage('parralel checking') {
            parallel {
                stage('Linux Testing') {
                    steps {
                        echo "Linux environment checking"
                    }
                }
                stage('Docker Testing') {
                    steps {
                        echo "Docker environment checking"
                    }
                }
            }
        }
    }
}

