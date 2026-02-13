pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building..'
        echo 'added line'
      }
    }

    stage('Test') {
      steps {
        echo 'Testing..'
      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying..'
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