pipeline {
  agent {
    node {
      label 'slave'
    }

  }
  stages {
    stage('step1') {
      parallel {
        stage('step1') {
          steps {
            echo 'B'
            sh 'hostname'
            sh 'date'
          }
        }

        stage('') {
          steps {
            echo 'A'
            sh 'hostname'
            sh 'date'
          }
        }

      }
    }

    stage('Z') {
      steps {
        echo 'ZZZ'
      }
    }

  }
}