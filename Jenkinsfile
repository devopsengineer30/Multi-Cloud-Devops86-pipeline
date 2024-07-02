pipeline {
  agent any
  stages {
    stage('plan') {
      steps {
        echo 'plan the pipeline'
      }
    }

    stage('code') {
      steps {
        echo 'develop the code'
      }
    }

    stage('Build') {
      steps {
        echo 'code will be build'
      }
    }

    stage('Deploy') {
      parallel {
        stage('Deploy') {
          steps {
            echo 'Code will be deploy'
          }
        }

        stage('Test') {
          steps {
            echo 'Code will be tested'
          }
        }

        stage('Operate') {
          steps {
            echo 'Operate the app'
          }
        }

      }
    }

  }
}