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
                dir('${WORKSPACE}/android') {
                    bat 'dir'
                }
            }
        }
    }
}