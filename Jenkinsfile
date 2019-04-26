pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'Building ...'
      }
    }
    stage('Test') {
      parallel {
        stage('Test Fireforx') {
          steps {
            sh 'echo \'Testing Firefox\''
          }
        }
        stage('Test Chrome') {
          steps {
            sh 'echo \'Testing Chrome\''
          }
        }
        stage('Test Edge') {
          steps {
            sh 'echo \'Testing Edge\''
          }
        }
      }
    }
    stage('Deploy / Print Message') {
      steps {
        echo 'Deploy'
      }
    }
  }
}
