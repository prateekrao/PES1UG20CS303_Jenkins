pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ testj.cpp -o testj'
                 build job: 'PES1UG20CS303-1', wait: false
                 echo 'Build by PES1UG20CS303 is successful!'
            }
        }

        stage('Test') {
            steps {
                sh 'cat testj.cpp'
                echo 'Test by PES1UG20CS303 is successful!'
            }
        }

        stage('Deploy') {
            steps {
               
                echo 'Deploy by PES1UG20CS303 is successful!'
            }
        }
    }

    post {
        failure {
            
                echo 'Pipeline has failed!'
          
        }
    }
}
