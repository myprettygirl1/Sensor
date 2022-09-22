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
        bat 'cpptesttrace make cpptestcli -data "%workspace%/cpptest_workspace" -bdf "%workspace%/cpptestscan.bdf" -resource "Sensor" -config "builtin://Recommended Rules" -report "%workspace%/report"'
      }
    }

  }
}