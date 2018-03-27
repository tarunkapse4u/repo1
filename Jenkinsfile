pipeline {
  agent any
  stages {
    stage('Compile') {
      steps {
        echo 'compile'
      }
    }
    stage('Unit TEst') {
      parallel {
        stage('Unit TEst') {
          steps {
            sh 'echo Unit test'
          }
        }
        stage('UI TEST') {
          steps {
            echo 'Print UI TEst'
          }
        }
      }
    }
    stage('Deploye') {
      steps {
        echo 'Deployee'
      }
    }
  }
}