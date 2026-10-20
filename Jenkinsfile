pipeline {
    agent any
    parameters {
        string (
            name: 'PERSON',
            defaultValue: 'Ganesh',
            description : 'Enter your name'
        )
    }
    stages {
        stage('Greeting') {
            steps {
                echo "Hello, ${params.PERSON}!"
            }
        }
    }
}

