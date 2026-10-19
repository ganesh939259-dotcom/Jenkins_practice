pipeline {
    agent any
    stages {
        stage('ssh-privatekey') {
            steps {
                withCredentials([sshUserPrivateKey (
                    credentialsId: 'privatekey-authentication',
                    keyFileVariable: 'SSH_KEY',
                    usernameVariable: 'SSH_USER'
                )]) {
                    sh 'test -n "$SSH_KEY"'
                    sh 'test -n "$SSH_USER"'
                    echo "shh private key successfully configures"
                }
            }
        }
    }
}
