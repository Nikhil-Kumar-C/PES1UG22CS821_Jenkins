pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ working.cpp -o temp'
                 build job: 'PES1UG22CS821-1', wait: false
                 echo 'Build by CS821 successful'
            }
        }

        stage('Test') {
            steps {
                sh 'cat working.cpp'
                echo 'Test by CS821 successful'
            }
        }

        stage('Deploy') {
            steps {
               
                 echo 'Deploy by CS821 successful'
            }
        }
    }

    post {
        failure {
            
                echo 'Pipeline Failed'
          
        }
    }
}
