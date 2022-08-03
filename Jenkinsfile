pipeline {
  agent any
  stages {
    stage('') {
      steps {
        sh '''cpptestcli -data "C:\\Program Files\\Jenkins\\workspace" -bdf "C:\\Program Files\\Jenkins\\Sensor\\cpptestscan.bdf" 
cpptestcli -data "C:\\Program Files\\Jenkins\\workspace" -resource "Sensor" -config "builtin://Recommended Rules" -report %WORKSPACE%/%BUILD_ID%'''
      }
    }

  }
}