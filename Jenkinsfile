pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building...'
      }
    }

    stage('Testing Browsers') {
      parallel {
        stage('Test Chrome') {
          steps {
            sh 'echo \'Testing Chrome\'; exit 1'
          }
        }

        stage('Test Edge') {
          steps {
            sh 'echo \'Testing Edge\''
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy'
      }
    }

  }
}
