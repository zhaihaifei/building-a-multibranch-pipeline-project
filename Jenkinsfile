pipeline {
    agent {
        docker {
            image 'node:12-alpine' 
            args '-p 3000:3000' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'npm -v'
                sh 'sudo chown -R `whoami` /'
                sh 'npm install --unsafe-perm=true --allow-root'
            }
        }
    }
}
