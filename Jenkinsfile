pipeline {
  agent any
  stages {
    stage('build docker') {
      agent any
      steps {
        sh 'docker build -t chat:$BUILD_NUMBER .'
      }
    }

  }
}