pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                echo 'build the application'
                sh """
                pwd
                ls -ltrh
                sudo -u ec2-user cp index.php /var/www/html/
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
