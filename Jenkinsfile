pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo "Building the pipeline"
      }
    }

    stage('Automation Tests') {
      parallel {
        stage('Test') {
          steps {
            echo "Automation Tests are executing"
          }
        }

        stage('Unit tests') {
          steps {
            echo "Unit tests are building"
          }
        }

      }
    }

    stage('Docker build') {
      steps {
        echo "Building docker image"
      }
    }

  }
}
