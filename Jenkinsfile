pipeline {
agent {
    label 'build-server-agent'
}

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build Docker Image') {
            steps {
                sh '''
                    docker build -t company-website:latest .
                '''
            }
        }

        stage('Verify Image') {
            steps {
                sh '''
                    docker images
                    docker image inspect company-website:latest
                '''
            }
        }
    }
}
