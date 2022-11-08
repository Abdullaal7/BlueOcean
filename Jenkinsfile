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
        input(message: 'are you sure you want to deploy', ok: 'yes iam sure')
        echo 'Deploy Complete'
      }
    }

    stage('New Build') {
      steps {
        echo 'New Build Complete'
      }
    }

  }
}