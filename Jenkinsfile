pipeline {
  agent any
  stages {
    stage('step1') {
      steps {
        git(url: 'https://github.com/Oinilp/test', branch: 'main')
      }
    }

    stage('log') {
      parallel {
        stage('log') {
          steps {
            sh 'ls -la'
          }
        }

        stage('test') {
          steps {
            sh 'npm install && npm run start %% sleep 15 && exit'
          }
        }

      }
    }

  }
}