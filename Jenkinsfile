pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                echo 'build the application'
                sh """
                whoami
                pwd
                ls -ltrh
                cp index.php /var/www/html/
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
