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
        	sh' echo "hola code analysis" '
            }
        }
        stage('Deploy') {
            steps {
                sh 'echo "Deploying"'
            }
        }
    }
}
