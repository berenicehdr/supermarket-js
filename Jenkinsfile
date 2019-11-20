pipeline {
    agent any
    stages {
        stage('Buil') {
            steps {  sonar-scanner \
                    -Dsonar.projectKey=supermarket_js \
                    -Dsonar.sources=. \
                    -Dsonar.host.url=http://13.52.180.37:9000 \
                    -Dsonar.login=46dec775c1773312bf9bb5bb641f5796de6800b3
            }
        }
        stage('Test') {
            steps {
                 sh ' echo "testing"'
            }
        }
        stage('Deploy') {
            steps {
                sh 'echo "Deploying"'
            }
        }
    }
}
