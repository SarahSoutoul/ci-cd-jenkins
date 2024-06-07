pipeline {
    // agent any
    agent {
        docker {
            image 'maven:3.6.3'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'mvn --version'
                echo 'Build'
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