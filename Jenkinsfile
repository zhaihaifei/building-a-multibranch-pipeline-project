pipeline {
    agent {
        docker {
            image 'node:12-alpine' 
            args '-p 3000:3000' 
        }
    }
    environment {
        CI = 'true' 
    }
    stages {
        stage('Build') { 
            steps {
                sh 'npm -v'
            }
        }
        stage('Test') { 
            steps {
                sh 'npm -v'
            }
        }
        stage('Deliver') { 
            steps {
                sh 'npm -v'
                input message: 'Finished using the web site? (Click "Proceed" to continue)' 
                sh 'npm -v'
            }
        }
    }
}
