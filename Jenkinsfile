pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building...'
      }
    }

    stage('Test') {  
      parallel {
        stage('Test Firefox') {
          steps {
            sh 'echo \'Testing firefox\''
          }
        }

        stage('Test Chrome') {
          steps {
            sh 'echo \'Testing chrome\'; exit 1'
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