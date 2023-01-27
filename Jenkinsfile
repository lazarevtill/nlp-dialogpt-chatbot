pipeline {
  agent any
  stages {
    stage('build docker') {
      steps {
        git(url: 'https://github.com/lazarevtill/nlp-dialogpt-chatbot', branch: 'main', poll: true)
        sh 'docker build -t chat:$BUILD_NUMBER .'
      }
    }

    stage('error') {
      steps {
        sh 'docker login 192.168.1.10 '
      }
    }

  }
}