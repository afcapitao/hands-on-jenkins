pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building...'
      }
    }

    stage('Test Firefox') {
      parallel {
        stage('Test Firefox') {
          steps {
            sh 'echo \'Testing firefox\''
          }
        }

        stage('Test Chrome') {
          steps {
            echo 'echo \'Testing chrome\''
          }
        }

        stage('Test edge') {
          steps {
            echo 'echo \'Testing edge\''
          }
        }

      }
    }

    stage('Deploy ') {
      steps {
        echo 'Deploy'
      }
    }

  }
}