pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                echo 'build the application'
                sh """
                pwd
                ls -ltrh
                sudo cp index.php /var/www/html/
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
