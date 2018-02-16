pipeline {
  agent any
  stages {
    stage('Stage1-Build') {
      steps {
        echo 'I am at Build stage'
      }
    }
    stage('Stage2-Test') {
      steps {
        echo 'Pass testing1'
        echo 'Pass testing 2'
      }
    }
    stage('Stage3-Deploy') {
      steps {
        echo 'Deployed'
      }
    }
  }
}