pipeline {
  agent any
  stages {
    stage('Dev') {
      steps {
        sh 'sh mvn clean build'
        echo 'print status'
      }
    }
    stage('Test') {
      steps {
        sh 'run mvn clean install'
      }
    }
  }
  environment {
    Dev = 'Dev'
    Test = 'Test'
  }
}