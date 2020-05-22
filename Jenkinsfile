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
    post {
        always {
            archiveArtifacts artifacts: 'package.json', onlyIfSuccessful: true
        }
    }
}
