pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        git(url: 'https://github.com/myprettygirl1/FlowAnalysis.git', branch: '%branch%')
      }
    }

    stage('Tests') {
      steps {
        bat 'cd %workspace" make clean cpptesttrace make cpptestcli -data "%workspace%/cpptest_workspace" -bdf "%workspace%/cpptestscan.bdf" -resource "FlowAnalysisi" -config "builtin://Recommended Rules" -report "%workspace%/report"'
      }
    }

  }
  environment {
    branch = 'main'
  }
}