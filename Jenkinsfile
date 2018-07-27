pipeline {
  agent any
  stages {
    stage('development') {
      parallel {
        stage('development') {
          steps {
            sh 'echo "hello development" '
          }
        }
        stage('qa') {
          steps {
            sh 'echo "hello qa"'
          }
        }
      }
    }
    stage('master') {
      steps {
        sh 'ip a'
      }
    }
  }
}