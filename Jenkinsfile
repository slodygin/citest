pipeline {
    agent { docker { image 'node:14-alpine' } }
    stages {
        stage('build') {
            def dockerHome = tool 'docker'
            env.PATH = "${dockerHome}/bin:${env.PATH}"
            steps {

                sh 'env'
                sh 'npm --version'
            }
        }
    }
}
