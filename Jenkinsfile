pipeline {
  agent {
    docker {
      image 'node:18'
    }
  }

  stages {
    stage('Checkout') {
      steps {
        checkout scm
      }
    }

    stage('Inspect') {
      steps {
        sh 'node -v'
        sh 'npm -v'
      }
    }
  }
}