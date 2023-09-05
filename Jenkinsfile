pipeline {
  agent any
  stages {
    stage('chekout code') {
      steps {
        git(url: 'https://github.com/Oinilp/test.git', branch: 'main')
      }
    }

    stage('Log') {
      parallel {
        stage('Log') {
          steps {
            sh 'ls -al'
          }
        }

        stage('Front-end Unit Test') {
          steps {
            sh 'apt-get update && npm i && npm run test:unit'
          }
        }

      }
    }

  }
}