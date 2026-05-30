pipeline {

    agent any

    stages {

        stage('Build') {
            steps {
                sh 'echo Building Application'
            }
        }

        stage('Docker Build') {
            steps {
                sh 'echo Building Docker Image'
            }
        }

        stage('Push') {
            steps {
                sh 'echo Pushing Image'
            }
        }

    }

}
