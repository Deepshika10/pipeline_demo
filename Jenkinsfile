pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building..'
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