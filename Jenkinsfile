pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t bistro-site .'
            }
        }

        stage('Deploy Container') {
            steps {
                sh '''
                docker rm -f bistro-container || true
                docker run -d --name bistro-container -p 80:80 bistro-site
                '''
            }
        }
    }
}
