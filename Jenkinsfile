pipeline {
    agent any
    stages {
        stage('Run on Any Agent') {
            agent any 
            steps {
                echo 'hello-world'
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
