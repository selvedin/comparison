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
        checkout scm
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