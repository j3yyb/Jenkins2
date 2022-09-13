pipeline {
    agent any
    parameters {
        booleanParam(name: 'Refresh',
                    defaultValue: false,
                    description: 'Read Jenkinsfile and exit.')
            }
    stages {
        stage('unit test') {
            steps {
                sh
                    python3 -pytest ./converter/tests/test_unit.py
                    python3 -pytest ./prime/tests/test_unit.py
            }
         }
        stage('integration test') {
            steps {
                
            }
        }
    }
}
