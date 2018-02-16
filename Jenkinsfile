pipeline {
  agent any
  stages {
    stage('Stage1-Build') {
      steps {
        echo 'Starting Build stage'
      }
    }
    stage('Stage2-Test') {
      steps {
        echo 'Starting testing 1'
        sh 'sleep 5'
        sh 'echo Success!'
      }
    }
    stage('Stage3-Deploy') {
      steps {
        echo 'Deployed'
      }
    }
  }
}