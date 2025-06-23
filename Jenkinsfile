pipeline {
    agent any
    // agent{
    //     label 'AGENT-1'
    // }
    options {
        // Timeout counter starts AFTER agent is allocated
        timeout(time: 1, unit: 'MINUTES')
        disableConcurrentBuilds()
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
               // error 'bat failure'
            }
        }
    
    }
    post{
        always{
            bat "echo always :: This session runs always"
            deleteDir()
        }
        success{
            bat "echo success :: This session runs when pipeline success"
        }
        failure{
            bat "echo failure :: This session runs when pipeline failures"
        }
    }
}