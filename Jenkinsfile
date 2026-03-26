pipeline {
  agent any

  stages {
    stage('Clean') {
      steps {
        deleteDir()
      }
    }

    stage('Checkout') {
      steps {
        git url: 'https://github.com/selvedin/comparison.git', branch: 'main'
      }
    }

    stage('Docker check') {
      steps {
        sh 'whoami'
        sh 'docker version'
        sh 'docker ps'
      }
    }

    stage('Build') {
      steps {
        echo 'Building...'
        sh 'pwd'
        sh 'ls -la'
      }
    }
  }
}