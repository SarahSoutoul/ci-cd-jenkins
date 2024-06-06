pipeline {
	agent {
		docker {
			image 'node:21.7'
		}
	}
	stages {
		stage('Build') {
			steps {
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
			echo 'I always run'
		}

		success {
			echo 'I run when successful'
		}

		failure {
			echo 'I run when failed'
		}
	}
}