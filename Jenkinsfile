#!groovy

pipeline {
  agent none
  stages {
    stage('Maven Install') {
      agent {
        docker {
          image 'maven:3.0.5'
        }
      }
      steps {
        sh 'mvn clean install'
      }
    } 
  }
}
