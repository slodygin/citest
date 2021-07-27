pipeline {
    agent { docker { image 'node:14-alpine' } }
    stages {
        stage('Initialize'){
            def dockerHome = tool 'docker'
            env.PATH = "${dockerHome}/bin:${env.PATH}"
        }
        stage('build') {
            steps {

                sh 'env'
                sh 'npm --version'
            }
        }
    }
}
