pipeline {
    agent {
        docker {
            image 'node:lts' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'npm install' 
            }
        }
    }
}
