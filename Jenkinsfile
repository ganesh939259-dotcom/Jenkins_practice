pipeline {
    agent any 
    stages {
        stage('validate secret') {
            steps {
                withCredentials([string (
                    credentialsId: 'practice-secret',
                    variable: 'DB_PASSWORD'
                )]) {
                    sh 'test -n "$DB_PASSWORD"'
                    echo 'Database password configured successully'
                }
            }
        }
    }
}
