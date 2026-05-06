pipeline {
    agent any

    stages {
        stage('Build Docker Image') {
            steps {
                sh 'docker build -t furqhan-app .'
            }
        }

        stage('Run Container') {
            steps {
                sh 'docker run -d furqhan-app'
            }
        }
    }
}
