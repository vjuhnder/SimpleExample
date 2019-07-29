pipeline {
  agent any
  stages {
    stage('stage1') {
      parallel {
        stage('stage1') {
          steps {
            echo 'This is stage1'
          }
        }
        stage('test') {
          steps {
            echo 'This is test stage'
          }
        }
      }
    }
    stage('Deploy') {
      parallel {
        stage('Deploy') {
          steps {
            echo 'This is deploy stage'
          }
        }
        stage('test stage 1') {
          steps {
            echo 'this is test stage 1'
          }
        }
      }
    }
  }
}