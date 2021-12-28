pipeline {
  agent any
  stages {
    stage('stage 01') {
      steps {
        sh 'echo "hi aws "'
      }
    }

    stage('stage 02') {
      parallel {
        stage('stage 02') {
          steps {
            sh 'echo " hello devops"'
          }
        }

        stage('parallel 1') {
          steps {
            sh '''cd /etc/os-release
'''
          }
        }

      }
    }

  }
}