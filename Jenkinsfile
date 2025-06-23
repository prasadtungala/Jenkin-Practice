pipeline {
    agent any
    options {
        // Timeout counter starts AFTER agent is allocated
        timeout(time: 1, unit: 'SECONDS')
    }
    stages {
        stage('Dev') {
            steps {
               bat 'echo In Development Environment'
            }
        }
        stage('Staging') {
            steps {
                bat 'echo In Stagging'
            }
        }
        stage('Production') {
            steps {
                bat 'echo In Production'
            }
        }
    
    }
    post{
        always{
            bat "This session runs always"
        }
        success{
            bat "This session runs when pipeline success"
        }
        failure{
            bat "This session runs when pipeline failures"
        }
    }
}