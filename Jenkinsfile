pipeline {
    agent { node { label 'AGENT-1' } } 

    stages {
        stage('Build') {
            steps {
                echo 'Building..Stage'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..Stage'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....Stage'
            }
        }
    }
}