pipeline{
  agent any
  stages{
    stage('Checkout'){
      steps{
        echo 'Code Checkout stage'
      }
    }
    stage('Build'){
      steps{
        echo 'Building the appliaction'
      }
    }
    stage('Test'){
      steps{
        echo 'Testing the appliaction'
      }
    }
    stage('Deploy'){
      steps{
        echo 'deploying the application'
      }
    }
    stage('Use Credentials'){
      steps{
        withCredentials([string(
          credentialsId: 'practice-secret',
          variable: 'MY_SECRET'
        )]) {
          sh 'echo Credentials is available'
          sh 'test -n "$MY_SECRET"'
          sh 'echo  "secret is configured successfully"'
        }
      }
    }
  }
}
