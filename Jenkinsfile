pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        echo 'Hello Jenkins!'
      }
    }
    stage('Build') {
      steps {
        echo 'Hello Jenkins!'
      }
    }
    stage('Test') {
      steps {
        echo 'Hello Jenkins!'
      }
    }
    stage('Deploy') {
      steps {
        echo 'Hello Jenkins!'
      }
    }
    stage('run-parallel-branches') {
      parallel {
        stage('a') {
          steps {
            echo 'Tests on Linux'
            sleep 10
          }
        }
        stage('b') {
          steps {
            echo 'Tests on Windows'
            sleep 10
          }
        }
      }
    }
  }
  options {
    timestamps()
  }
}