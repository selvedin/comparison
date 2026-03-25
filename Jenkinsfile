pipeline {
  agent any

  stages {
    stage('Checkout') {
      steps {
        checkout scm
      }
    }

    stage('Build') {
      steps {
        echo 'Preparing app...'
        sh 'ls -la'
      }
    }

    stage('Test') {
      steps {
        echo 'Running checks...'
        sh 'grep -i vue index.html || true'
      }
    }
  }
}