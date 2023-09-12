pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'build completed'
      }
    }

    stage('Test stages') {
      parallel {
        stage('Test2') {
          steps {
            echo 'Runnung Test2'
          }
        }

        stage('Test1') {
          steps {
            echo 'Runnung Test1'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deploy completed'
      }
    }

  }
}