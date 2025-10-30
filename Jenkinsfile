//DECLARATIVE
pipeline {
	agent any
	stages {
		stage('Build') {
			steps {
				echo "Build"
			}
		}
		stage('Test') {
			steps {
				echo "Test"
			}
		}
		stage('Integration Test') {
			steps {
				echo "Integration Test"
			}
		}
	} 
	
	post {
		always {
			echo 'Im good, I run always'
		}
		success {
			echo 'Im good, I run always'	
		}
		failure {
			echo 'I run when you are successful'	
		}
	}
}				