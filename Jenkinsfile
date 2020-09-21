pipeline {
  agent any
  stages {
    stage('install npm') {
      steps {
        sh 'npm install'
      }
    }

    stage('test') {
      steps {
        sh './jenkins/scripts/test.sh'
      }
    }

  }
  environment {
    CI = 'true'
  }
}