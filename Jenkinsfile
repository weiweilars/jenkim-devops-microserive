pipeline {
	agent any 
	stages {
		stage('Build'){
			steps {
				echo "Build"
			}
		}
		stage('Test'){
			steps {
				echo "Test"
			}
		
		}
		stage('Integration Test'){
			steps {
				echo "Integration Tests"
			}
		
		}
	} 
	post {
		always {
			echo 'finished'
		}
		success {
			echo 'success'
		}
		failure {
			echo 'failure'
		}
	}
}