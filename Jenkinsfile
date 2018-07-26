pipeline {
  agent any
  stages {
    stage('CheckOut') {
      steps {
        git(url: 'https://github.com/sivakumarvunnam/node-emoji.git', branch: 'master')
      }
    }
  }
  environment {
    Node_ENV = 'Dev'
  }
}