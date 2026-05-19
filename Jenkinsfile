pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'Build stage'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            sh 'echo \'test stage\''
          }
        }

        stage('test-code') {
          steps {
            echo 'Test source code'
          }
        }

      }
    }

    stage('uat') {
      steps {
        sleep 10
        echo 'after sleep'
      }
    }

  }
}