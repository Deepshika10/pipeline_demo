pipeline {
    agent any // Run this pipeline on any available agent
    
    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                // sh 'make' // Example of a shell command
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                // sh 'make check'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying..'
                // sh 'make publish'
            }
        }
    }
    
    post {
        always {
            echo 'Cleaning up workspace...'
            cleanWs()
        }
        success {
            echo 'Pipeline Succeeded!'
        }
        failure {
            echo 'Pipeline Failed!'
        }
    }
}
