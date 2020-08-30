pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo \'hello world\''
      }
    }

    stage('Automation Tests') {
      parallel {
        stage('Test') {
          steps {
            sh 'echo "Automation Tests are executing"'
          }
        }

        stage('Unit tests') {
          steps {
            sh 'echo "Unit tests are building"'
          }
        }

      }
    }

    stage('Docker build') {
      steps {
        sh 'echo "Building docker image"'
      }
    }

  }
}