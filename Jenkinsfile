pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        git(url: 'https://github.com/myprettygirl1/FlowAnalysis.git', branch: '%branch%')
      }
    }

    stage('MISRA') {
      steps {
        bat 'RunMISRATest.bat'
      }
    }

  }
  environment {
    branch = 'main'
  }
}