pipeline {    
   
	def remote = [:]
    remote.name = 'Admin'
    remote.host = '192.168.12.131'
    remote.user = 'Admin'
    remote.password = 'Admin123'
    remote.allowAnyHosts = true


    agent any
    stages {

        stage('SSH'){
        	when { branch "release/*" }
        	steps{
        		echo 'Hello World'
        	}
        }
     }   

    post {
        always {
            echo 'Text Complete'
        }
        failure {
          echo 'Test Fail'
        }
    }
}
 
 
 
 
