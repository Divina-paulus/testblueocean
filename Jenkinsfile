pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'build completed'
      }
    }

    stage('test1') {
      parallel {
        stage('test1') {
          steps {
            echo 'running test1'
          }
        }

        stage('test2') {
          steps {
            echo 'running test2'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deployment'
      }
    }

  }
}