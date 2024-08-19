pipeline {
    agent {
        docker {
            image 'maven:3.9.8'
        }
    }
    stages {
        stage('Test') {
            steps {
                sh 'mvn --version'
            }
        }
    }
}