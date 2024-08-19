pipeline {
    agent none
    stages {
        stage('Run on Any Agent') {
            agent any 
            steps {
                echo 'hello-Pedro-2'
            }
        }

        stage('Run in Docker Image') {
            agent {
                docker {
                    image 'maven:3.9.8'
                }
            }
            steps {
                sh 'mvn --version'
            }
        }
    }
}
