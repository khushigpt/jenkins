pipeline {
    agent {
        docker {
            image 'node:18'
        }
    }

    stages {
        stage('Build') {
            steps {
                sh 'node -v'
                sh 'echo Building app'
            }
        }
        stage('Run App') {
            steps {
                sh 'node -e \"console.log('Hello from Docker build')\"'
            }
        }
    }
}
