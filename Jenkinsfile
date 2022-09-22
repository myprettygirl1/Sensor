pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        git(url: 'https://github.com/myprettygirl1/Juliet.git', branch: 'main')
      }
    }

    stage('Tests') {
      steps {
        bat '.bat'
      }
    }

  }
}