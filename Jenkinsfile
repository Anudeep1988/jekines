pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'i want to build'
      }
    }

    stage('test') {
      steps {
        echo 'i want to test'
      }
    }

    stage('Stage') {
      parallel {
        stage('Stage') {
          steps {
            echo 'i want to stage'
          }
        }

        stage('deploy') {
          steps {
            echo 'i want to operate'
          }
        }

        stage('operate') {
          steps {
            echo 'i want to opertae'
          }
        }

      }
    }

  }
}