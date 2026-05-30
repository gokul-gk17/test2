pipeline{
    agent any
    tools {
        maven 'maven' 
    }
    stages{
        stage('Dependencies'){
            steps{
                sh 'mvn clean package'
            }
        }

        stage('build'){
            steps{
                sh 'docker build -t springapp .'
            }
        }

        stage('Run'){
            steps{
                sh 'docker run -d -p 8080:8080 --name spring-app1 springapp'
            }
        }
    }
}
