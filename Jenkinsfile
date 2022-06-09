pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''pwd
ls
date
'''
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'testing'
          }
        }

        stage('test parallel') {
          steps {
            echo 'testing parallel '
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'deploying'
      }
    }

  }
}