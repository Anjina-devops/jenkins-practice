pipeline {
    agent { node { label 'AGENT-1' } } 

    stages {
        stage('Build') {
            steps {
                echo 'Building..Stage'

                sh '''
                   ls -l
                   pwd
                   echo "Hello this is from build stage via scripts"

                '''
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

                //error "this is failed..."
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