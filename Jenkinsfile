pipeline {
  agent any
  stages {
    stage('Compile') {
      steps {
        sh 'echo compile'
      }
    }
    stage('Unit TEst') {
      parallel {
        stage('Unit TEst') {
          steps {
            sh 'echo Unit test'
          }
        }
        stage('Ui Test') {
          steps {
            sh 'echo ui test'
          }
        }
      }
    }
    stage('Deploye') {
      steps {
        sh 'echo deployee'
      }
    }
  }
}