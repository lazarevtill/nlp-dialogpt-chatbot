pipeline {
  agent any
  stages {
    stage('build docker') {
      steps {
        sh 'docker build -t chat:$BUILD_NUMBER .'
      }
    }

  }
}