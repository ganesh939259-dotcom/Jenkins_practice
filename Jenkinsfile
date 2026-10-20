pipeline {
    agent any
    parameters {
        string (
            name: 'APP_NAME',
            defaultValue: 'nginx',
            description: 'select your option'
        ) {
            stages{
                stage('Build') {
                    steps {
                        sh ' echo $APP_NAME'
                    }
                }
            }
        }
    }
}

  
