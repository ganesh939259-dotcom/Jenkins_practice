pipeline {
    agent any
    stages {
        stage('Checking Multiple Credentials') {
            steps {
                withCredentials([
                    string (
                        credentialsId: 'practice-secret',
                        variable: 'API_TOKEN'
                ),
                usernamePassword(
                    credentialsId: 'practice-username',
                    usernameVariable: 'USER_NAME',
                    passwordVariable: 'USER_PASSWORD'
                )]) {
                    sh '''
                    test -n "$API_TOKEN" &&
                    test -n "$USER_NAME" &&
                    test -n "$USER_PASSWORD"
                    '''
                    echo "All credentials loaded successfully"
                }
            }
        }
    }
}

                                
                                
                                
                                
                    
