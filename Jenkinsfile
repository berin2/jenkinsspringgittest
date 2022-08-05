pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Starting build steps..'
                sh '${mvn_bin} clean'
                sh '${mvn_bin} install'
            }
        }
        stage('Test') {
            steps {
                echo 'Running mvn tests...'
            }
        }
        stage('Pack jar into docker') {
            steps {
                echo 'Deploying....'
            }
        }

    }
}