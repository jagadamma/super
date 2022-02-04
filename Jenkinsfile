pipeline {
  agent any
  enviorment
  {
    JOB_NAME = bangalore
  }
  stages {
    stage('stage 01') {
      steps {
        sh 'echo "hi aws from ${JOB_NAME}"'
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
