pipeline {
  agent any
  stages{
    stage('Testing') {
    steps {
        sh '''
            mkdir -p test-results
            echo '<?xml version="1.0" encoding="UTF-8"?>' > test-results/results.xml
            echo '<testsuite name="SampleTests" tests="2" failures="0">' >> test-results/results.xml
            echo '  <testcase classname="DemoTest" name="testOne"/>' >> test-results/results.xml
            echo '  <testcase classname="DemoTest" name="testTwo"/>' >> test-results/results.xml
            echo '</testsuite>' >> test-results/results.xml
        '''
        junit 'test-results/results.xml'
    }
}
