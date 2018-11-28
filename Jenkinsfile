pipeline {    


    agent any
    stages {

        stage('SSH'){
        	when { branch "release/*" }
        	steps{
        		sh echo 'Hello World'
        	}
        }
     }   

    post {
        always {
            sh echo 'Text Complete'
        }
        failure {
          sh echo 'Test Fail'
        }
    }
}
 
 
 
 
