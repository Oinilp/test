pipeline {
  agent any
  stages {
    stage('chekout code') {
      steps {
        git(url: 'https://github.com/Oinilp/test.git', branch: 'main')
      }
    }

    stage('Log') {
      steps {
        sh 'ls -al'
      }
    }

  }
}