pipeline {
    agent { node { label 'AGENT-1' } } 

    stages {
        stage('Build') {
            steps {
                echo 'Building..Stage....OKKKKKKKKKKKKKK'

                sh '''
                   ls -l
                   date
                   pwd
                   echo "Hello this is from github webhook push"

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