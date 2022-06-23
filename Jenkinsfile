pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build completed'
      }
    }

    stage('Test Stages') {
      parallel {
        stage('Test2') {
          steps {
            echo 'running test2'
          }
        }

        stage('Test1') {
          steps {
            echo 'running test1'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'deployment completed'
      }
    }

  }
}