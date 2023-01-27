pipeline {
  agent any
  stages {
    stage('build') {
      agent any
      steps {
        sh 'docker build -t chat:$BUILD_NUMBER .'
      }
    }

    stage('push') {
      steps {
        sh '''docker login 192.168.1.10 -u user -p 12345678
'''
      }
    }

  }
}