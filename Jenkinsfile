pipeline {
    agent any
    parameters {
        string (
            name: 'APP_NAME',
            defaultValue: 'nginx',
            description: 'select your parameters'
        ) 
    }
    stages{
        stage('Build') {
            steps {
                echo "Building the application"
            }
        }
    }
}
