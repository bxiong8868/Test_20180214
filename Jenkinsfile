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
        sleep 2
        echo 'Pass testing 1'
      }
    }
    stage('Stage3-Deploy') {
      steps {
        echo 'Deployed Completed'
      }
    }
  }
}