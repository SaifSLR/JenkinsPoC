pipeline {    


    agent any
    stages {

        stage('SSH'){
        	when { branch "release/*" }
        	steps{
                step{
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
 
 
 
 
