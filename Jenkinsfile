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
                bat 'start "" yarn react-native start &'
            }
        }
        stage('Run') {
            steps {
                bat 'npx react-native run-android'
            }
        }
    }
}