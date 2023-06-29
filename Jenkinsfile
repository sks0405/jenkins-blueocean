pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh "pwd"
        sh "Hello to jenkins"

      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'test step'
          }
        }

        stage('Test par') {
          steps {
            echo 'test par'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        sleep 10
      }
    }

  }
}
