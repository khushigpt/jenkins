pipeline {
	agent {
		docker {
			image 'node:18'
			}
		}
	stages {
		stage('Install Dependencies') {
		steps {
			sh 'npm install'
			}
		}
		stage('Run Application') {
		steps {
			sh 'node app.js & sleep 5'
			}
		}
		stage('Test Output') {
			steps {
				sh 'curl -s localhost:3000'
			}
		}
	}
}

