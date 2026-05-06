pipeline {
    agent any

    stages {
        stage('Pull Code') {
            steps {
                git 'https://github.com/<your-username>/<repo>.git'
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
