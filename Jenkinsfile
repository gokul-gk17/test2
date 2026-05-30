pipeline{
    agent any
    stages{
        stage('Dependencies'){
            steps{
                bat 'mvn clean package'
            }
        }

        stage('build'){
            steps{
                bat 'docker build -t springapp .'
            }
        }

        stage('Run'){
            steps{
                bat 'docker run -d -p 8080:8080 --name spring-app1 springapp'
            }
        }
    }
}