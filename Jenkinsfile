#!/usr/bin/env groovy

pipeline {
  agent any
  triggers { pollSCM('* * * * *') }
  stages {
    stage('Build') {
      steps {
        sh './mvnw clean package'
      }
    }
  }
}