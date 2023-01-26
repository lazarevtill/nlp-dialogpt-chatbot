pipeline {
  agent any
  stages {
    stage('build docker') {
      steps {
        sh 'docker build -t chat:$BUILD_NUMBER .'
      }
    }

    stage('') {
      steps {
        sh 'docker login 192.168.1.10 '
      }
    }

  }
}