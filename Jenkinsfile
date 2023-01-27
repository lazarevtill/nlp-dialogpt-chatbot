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
        sh '''docker login nexus.lazarev.gq:14587 -u user -p 12345678
'''
      }
    }

  }
}