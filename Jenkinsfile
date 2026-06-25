pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build Backend') {
            steps {
                sh 'docker build -t micro-backend ./backend'
            }
        }

        stage('Build Frontend') {
            steps {
                sh 'docker build -t micro-frontend ./frontend'
            }
        }
    }
}

