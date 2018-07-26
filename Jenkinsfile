pipeline {
  agent any
  stages {
    stage('CheckOut') {
      steps {
        git(url: 'https://github.com/sivakumarvunnam/node-emoji.git', branch: 'master')
      }
    }
    stage('Initialize ') {
      steps {
        sh '''curl https://raw.githubusercontent.com/isaacs/nave/master/nave.sh | sudo bash -s -- usemain lts
node -v
npm -v
npm install '''
      }
    }
  }
  environment {
    Node_ENV = 'Dev'
  }
}