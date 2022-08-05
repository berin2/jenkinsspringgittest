pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Starting build steps..'
                mvn  clean
                mvn  install
            }
        }
        stage('Test') {
            steps {
                echo 'Running mvn tests...'
                mvn test
            }
        }
        stage('Pack jar into docker') {
            steps {
                echo 'Deploying....'
            }
        }

    }
}