pipeline {
    agent any

    stages {

        stage('Clone') {
            steps {
                git 'https://github.com/Neelkanta12/devops-demo-repo.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t my-app .'
            }
        }

        stage('Run Container') {
            steps {
                sh 'docker run -d -p 8081:80 my-app'
            }
        }
    }
}
