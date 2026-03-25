pipeline {
  agent any
  stages {
    stage('Docker check') {
      steps {
        sh 'whoami'
        sh 'docker version'
        sh 'docker ps'
      }
    }
  }
}