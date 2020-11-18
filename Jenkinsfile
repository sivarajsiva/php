pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                echo 'build the application'
            }
        }
        stage('Test') { 
            steps {
               echo 'test the application'
            }
        }
		stage('SSH transfer') {
		 script {
		  sshPublisher(
		   continueOnError: false, failOnError: true,
		   publishers: [
			sshPublisherDesc(
			 configName: "testing",
			 verbose: true,
			 transfers: [
			  sshTransfer(
			   sourceFiles: "**/*",
			   removePrefix: "",
			   remoteDirectory: "",
			   execCommand: ""
			  )
			 ])
		   ])
		 }
		}
        stage('Deploy') { 
            steps {
                echo 'deploy the application'
            }
			
        }
    }
}
