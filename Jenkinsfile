//SCRIPTED

// DECLARATIVE
pipeline {
	//agent any
	agent { docker { image 'maven:3.8.5'}}
	stages {
		stage ('Build') {
			steps { 
				sh "mvn --version"
				echo "Build"
			}
	    }
		stage ("Test") {
			steps {
				echo "Test"			
			 }
		}
		stage('Integration Test') {
            steps{
				echo "Integration Test" 
			 }
		}
	}	  	    


    post {
	    always {
		    echo 'Im awesome. Irun always'
	    }
	    success {
		    echo 'I run when you are successful'
	    }
	    failure {
		    echo 'I run when you fail'
	    }
    }
}


