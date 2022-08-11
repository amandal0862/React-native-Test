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
                dir('android') {
                    bat 'dir'
                    bat './gradlew clean'
                }
            }
        }
    }
}