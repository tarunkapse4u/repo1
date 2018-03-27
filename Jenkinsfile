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
        stage('Ui Test') {
          steps {
            echo 'uitest'
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