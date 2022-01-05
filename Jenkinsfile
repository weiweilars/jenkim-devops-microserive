pipeline {
	agent any
	// agent {
	// 	docker { image 'maven:3.6.3'}
	// }
	stages {
		stage('Build'){
			steps {
				// sh 'mvn --version'
				echo "$PATH"
				echo "BUILD_NUMBER -- $env.BUILD_NUMBER"
				echo "BUILD_ID -- $env.BUILD_ID"
				echo "BUILD_TAG -- $env.BUILD_TAG"
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