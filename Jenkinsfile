pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build Complete'
      }
    }

    stage('Test Stages') {
      parallel {
        stage('Test1') {
          steps {
            echo 'Test1 Complete'
          }
        }

        stage('Test2') {
          steps {
            echo 'Test2 Complete'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy Complete'
      }
    }

  }
}