pipeline {
  agent any
  stages {
    stage('Stage1-Build') {
      steps {
        echo 'Starting Build stage'
        archiveArtifacts(artifacts: 'target/*.jar', allowEmptyArchive: true)
      }
    }
    stage('Stage2-Test') {
      parallel {
        stage('Stage2-Test') {
          steps {
            echo 'Starting testing 1'
            sleep 2
            echo 'Pass testing 1'
          }
        }
        stage('Test 2 in parallel') {
          steps {
            echo 'test 2'
            junit(testResults: 'target/test-results/**/TEST*.xml', allowEmptyResults: true)
          }
        }
      }
    }
    stage('Stage3-Deploy') {
      steps {
        echo 'Deployed Completed'
      }
    }
  }
}