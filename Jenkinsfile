pipeline {
    agent none
    tools {
        dockerTool 'docker' 
    }
    stages {
        stage('Initialize'){
            steps {
              def dockerHome = tool 'docker'
              env.PATH = "${dockerHome}/bin:${env.PATH}"
            }
        }
        stage('build') {
            agent { docker { image 'node:14-alpine' } }
            steps {
                sh 'env'
                sh 'npm --version'
            }
        }
    }
}
