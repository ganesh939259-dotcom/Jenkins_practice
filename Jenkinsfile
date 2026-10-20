pipeline {
    agent any
    stages {
        stage('parralel checking') {
            parralel {
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
