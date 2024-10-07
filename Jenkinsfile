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
 post { 
        always { 
            echo 'I will always say Hello again!'
        }

        success{

            echo "I will run only in success scenario"
        }

        failure{

            echo "i will run in failure case only"
        }
    }

}