pipeline{
    agent any
    stages{
        stage('Dependencies'){
            step{
                bat 'mvn clean package'
            }
        }

        stage('build'){
            step{
                bat 'docker build -t springapp .'
            }
        }

        stage('Run'){
            step{
                bat 'docker run -p 8080:8080 --name spring-app1 springapp'
            }
        }
    }
}