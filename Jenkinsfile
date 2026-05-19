pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'Build stage'
      }
    }
    stage('test') {
        steps {
          echo 'test stage'
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
