pipeline {
    agent any
    parameters {
        string (
            name: 'ARCHIVE_FILES',
            defaultValue: 'true',
            description: 'Set to tru archive app.txt'
        )
    }
    stages {
        stage('Creating Files') {
            sh 'echo "Application build" > app.txt'
        }
    }
    stage('Archive') {
        when {
            expression {
                params.ARCHIVE_FILES == 'true'
            }
        }
        steps {
            archiveArtifacts artifacts: 'app.txt'
        }
    }
}
