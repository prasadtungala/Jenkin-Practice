pipeline {
    agent any
    options {
        // Timeout counter starts AFTER agent is allocated
        timeout(time: 1, unit: 'SECONDS')
    }
    stages {
        stage('Dev') {
            steps {
                echo 'In Development Environment'
            }
        }
        stage('Staging') {
            steps {
                echo 'In Stagging'
            }
        }
        stage('Production') {
            steps {
                echo 'In Production'
            }
        }
    }
}