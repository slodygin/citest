pipeline {
    agent none
    stages {
        stage('build') {
            agent { docker "node:14-alpine" }
            }
            steps {
                sh 'env'
                sh 'npm --version'
            }
        stage('build') {
            agent { docker "golang" }
            steps {
                sh 'go version'
            }
        }
    }
}
