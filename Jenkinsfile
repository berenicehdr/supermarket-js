pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'echo "Building application"'
            }
        }
        stage('Test') {
            steps {
                sh 'echo "Running test"'
                 sh '''
                    npm test
                '''
            }
        }
         stage('Code Analysis') {
            steps {
                    sh 'echo "Running tests"'
                    sonar-scanner
                    -Dsonar.projectKey=supermarket_js
                    -Dsonar.sources=.
                    -Dsonar.host.url=http://13.52.180.37:9000
                    -Dsonar.login=46dec775c1773312bf9bb5bb641f5796de6800b3
            }
        }
        stage('Deploy') {
            steps {
                sh 'echo "Deploying"'
            }
        }
    }
}
