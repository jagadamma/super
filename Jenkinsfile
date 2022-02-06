pipeline {
  agent any
  enviorment
  {
    JOB_NAME = bangalore
  }
  stages {
    stage('stage 01') {
      steps {
        sh 'echo "hi aws from ${JOB_NAME}"
      }
    }

    stage('stage 02') {
      parallel {
        stage('stage 1') {
          steps {
            sh 'echo " hello devops ${JOB_NAME}"
          }
        }

        stage(' parallel 001') {
          steps {
            sh '''cat /etc/os-release
'''
          }
        }

      }
    }

  }
}
