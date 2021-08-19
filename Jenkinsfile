pipeline {
    agent none
    stages {
        stage('build1') {
            agent { docker "node:14-alpine" }
            steps {
                sh 'env'
                sh 'npm --version'
            }
        }
        stage('build2') {
            agent { docker "golang" }
            steps {
                sh 'go version'
            }
        }
    }
}
