pipeline {
    agent any
    options {
        // Timeout counter starts AFTER agent is allocated
        timeout(time: 1, unit: 'SECONDS')
    }
    stages {
        stage('Dev') {
            steps {
               sh 'echo In Development Environment'
            }
        }
        stage('Staging') {
            steps {
                sh 'echo In Stagging'
            }
        }
        stage('Production') {
            steps {
                sh 'echo In Production'
            }
        }
    }
}