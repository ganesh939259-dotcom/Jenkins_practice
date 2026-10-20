pipeline {
    agent any
    triggers {
        cron('H/10 * * * * ')
    }
    stages {
        stage('Build') {
            steps {
                echo "Building the application"
            }
        }
    }
}
