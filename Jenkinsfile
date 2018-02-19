pipeline {
  agent any
  stages {
    stage('Stage1-Build') {
      steps {
        echo 'Starting Build stage'
        archiveArtifacts 'target/*.jar'
      }
    }
    stage('Stage2-Test') {
      steps {
        echo 'Starting testing 1'
        sleep 2
        echo 'Pass testing 1'
        junit 'target/**/TEST*.xml'
      }
    }
    stage('Stage3-Deploy') {
      steps {
        echo 'Deployed Completed'
      }
    }
  }
}