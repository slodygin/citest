pipeline {
    agent none
    tools {
        dockerTool 'docker' 
    }
    stages {
        stage('build') {
            agent { docker { image 'node:14-alpine' } }
            steps {
                sh 'env'
                sh 'npm --version'
            }
        }
    }
}
