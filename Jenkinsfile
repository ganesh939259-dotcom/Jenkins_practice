
pipeline {
    agent any

    parameters {
        string(
            name: 'ARCHIVE_FILES',
            defaultValue: 'true',
            description: 'Set to true to archive app.txt'
        )
    }

    stages {
        stage('Creating Files') {
            steps {
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
}
