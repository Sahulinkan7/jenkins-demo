pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh '''pwd
              date'''
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'test'
          }
        }

        stage('test2') {
          steps {
            sh 'pwd'
          }
        }

      }
    }

    stage('last') {
      steps {
        sh 'pwd'
        echo 'kkk'
      }
    }

  }
}