//SCRIPTED

// DECLARATIVE
pipeline {
	agent any
	stages {
		stage ('Build') {
			steps { 
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
}post {
	always {
		echo 'Iam awesome. Irun always'
	}
	success {
		echo 'Irun when you are successful'
	}
	failure {
		echo 'Irun when you fail'
	}
}



