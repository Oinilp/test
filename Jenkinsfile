pipeline {
  agent any
  stages {
    stage('step1') {
      steps {
        git(url: 'https://github.com/Oinilp/test.git', branch: 'main')
      }
    }

    stage('log') {
      steps {
        sh 'ls -la'
      }
    }

  }
}