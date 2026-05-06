pipeline {
    agent any

    stages {
        stage('Pull Code') {
            steps {
                git git 'https://github.com/Furqhan55/git-job.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t myapp .'
            }
        }

        stage('Run Container') {
            steps {
                sh 'docker run -d myapp'
            }
        }
    }
}
