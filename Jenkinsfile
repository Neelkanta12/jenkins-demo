pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'mvn clean package'   // This will FAIL (no maven installed)
            }
        }
    }
}
