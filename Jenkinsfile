pipeline {
    agent {
        docker {
            image 'node:lts-buster-slim'
        }
    }
    environment {
        CI = 'true'
    }
    stages {
        stage('Build') {
            steps {
                sh 'yarn install'
            }
        }
        stage('test') {
            steps {
                sh 'yarn react-native start &'
            }
            steps {
                sh 'npx react-native run-android'
            }
        }
    }
}
