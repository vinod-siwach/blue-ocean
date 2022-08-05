pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        sh '''pwd
date'''
      }
    }

    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'test msg'
          }
        }

        stage('perlel build') {
          steps {
            echo 'perl build'
          }
        }

      }
    }

    stage('deploye') {
      steps {
        sleep 4
        echo 'deploye'
      }
    }

  }
}