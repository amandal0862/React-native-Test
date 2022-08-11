pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                bat 'yarn install'
            }
        }
        stage('test') {
            steps {
                bat 'cd android'
                bat 'dir'
            }
        }
    }
}