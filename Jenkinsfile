pipeline {
    agent any
    parameters {
        string (
            name: 'PERSON',
            defaultValue: 'Ravi',
            description: 'Enter your name'

            )
    }
    stages {
        stage('greeting') {
            steps {
                echo "Hello, ${params.PERSON}!"
            }
        }
    }
}
