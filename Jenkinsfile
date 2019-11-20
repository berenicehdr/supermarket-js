pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                sh' echo"building application"'
            }
        }
        stage('Test') { 
            steps {
                 sh ' echo "testing"' 
            }
        }
        stage('Deploy') { 
            steps {
                sh 'echo "Deploying' 
            }
        }
    }
}
