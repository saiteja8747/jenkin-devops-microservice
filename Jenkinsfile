//DECLARATIVE
pipeline {
	// agent any
	agent { docker { image 'node:3.21'} }
	stages {
		stage('Build') {
			steps {
				//sh 'mvn --version'
				sh 'node --version'
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