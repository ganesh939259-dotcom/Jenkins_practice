pipeline {
    agent any
    triggers {
        cron('H/2 * * * * ')
    }
    stages {
        stage('Build') {
            steps {
                echo "Building the application"
            }
        }
    }
}
