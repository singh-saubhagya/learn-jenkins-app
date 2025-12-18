pipeline {
    agent any

    stages {
        stage('Build') {
            agent {
                image 'node:18-alpine'
                reuseNode true
            }
            steps {
                sh '''
                ls -la
                node --version
                npm ---version
                npm c1
                npm run build
                ls -la
                '''
            }
        }
    }
}
