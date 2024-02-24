pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''pwd
ls'''
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'test messages'
          }
        }

        stage('test parallel') {
          steps {
            echo 'pararrel msg'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'deploy'
        sleep 10
      }
    }

  }
}