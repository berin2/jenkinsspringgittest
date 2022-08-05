pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Starting build steps..'
                sh '${mvn_bin}/mvn clean'
                sh '${mvn_bin}/mvn install'
            }
        }
        stage('Test') {
            steps {
                echo 'Running mvn tests...'
                sh '${mvn_bin/mvn test}'
            }
        }
        stage('Pack jar into docker') {
            steps {
                echo 'Deploying....'
            }
        }

    }
}