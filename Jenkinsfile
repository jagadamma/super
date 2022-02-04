pipeline {
  agent any
  enviorment
  {
    place = bangalore
  }
  stages {
    stage('stage 01') {
      steps {
        sh 'echo "hi aws from ${place}"'
      }
    }

    stage('stage 02') {
      parallel {
        stage('stage 002') {
          steps {
            sh 'echo " hello devops"'
          }
        }

        stage('parallel 01') {
          steps {
            sh '''cat /etc/os-release
'''
          }
        }

      }
    }

  }
}
