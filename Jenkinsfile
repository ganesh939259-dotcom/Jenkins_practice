pipeline {
    agent any
    parameters {
        string (
            name: 'PERSON',
            defaultValue: 'Ganesh',
            description : 'Enter your name'
        )
    }
    stage('Greeting') {
        steps {
            echo "Hello, ${parms.PERSON}!"
        }
    }
}
