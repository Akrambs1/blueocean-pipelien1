pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'build completed'
        retry(count: 3) {
          sh 'wwwwwwwww'
        }

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
        input(message: 'Are you sur to deploy ', ok: 'Yes, I am sure')
        echo 'deploy completed'
      }
    }

    stage('Notify for new build') {
      steps {
        echo 'New build completed successfuly'
      }
    }

  }
}