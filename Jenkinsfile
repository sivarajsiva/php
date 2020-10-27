pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                echo 'build the application'
                sh """
                ls -ltrh
                """
            }
        }
        stage('Test') { 
            steps {
               echo 'test the application'
            }
        }
        stage('Deploy') { 
            steps {
                echo 'deploy the application'
            }
        }
    }
}
