
pipeline {
    agent any

    stages {
        stage('Testing') {
            steps {
                sh '''
                    mkdir -p test-results
                    echo '<?xml version="1.0" encoding="UTF-8"?>' > test-results/results.xml
                    echo '<testsuite name="DevOpsTests" tests="3" failures="0">' >> test-results/results.xml
                    echo '  <testcase classname="DevOpsTest" name="testLinux"/>' >> test-results/results.xml
                    echo '  <testcase classname="DevOpsTest" name="testDocker"/>' >> test-results/results.xml
                    echo '  <testcase classname="DevOpsTest" name="testJenkins"/>' >> test-results/results.xml
                    echo '</testsuite>' >> test-results/results.xml
                '''
                junit 'test-results/results.xml'
            }
        }
    }
}
