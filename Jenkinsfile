  pipeline {
      agent any
      stages {
          stage('Creating Artifact') {
              steps {
                  sh ' echo "I want to become a DevOps Engineer" > devops.txt'
                  archiveArtifacts artifacts: 'devops.txt'
              }
          }
      }
  }
